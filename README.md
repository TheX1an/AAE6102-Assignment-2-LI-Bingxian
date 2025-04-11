# AAE6102-Assignment-2-LI-Bingxian
# Comparative Evaluation of GNSS Techniques for Smartphone Navigation

This project provides a comparative analysis of key Global Navigation Satellite System (GNSS) enhancement techniques for smartphone-based navigation. It evaluates four major approaches—**Differential GNSS (DGNSS)**, **Real-Time Kinematic (RTK)**, **Precise Point Positioning (PPP)**, and **PPP-RTK**—in terms of accuracy, infrastructure requirements, and compatibility with modern smartphones.

## Overview

Modern GNSS solutions enhance positioning accuracy using a variety of error-mitigation strategies. As smartphones increasingly rely on precise location data for navigation, AR, and micro-mobility, understanding these techniques is essential for both developers and system designers.

## Enhancement Techniques

### 1. Differential GNSS (DGNSS)
- **Method**: Uses code-phase corrections from a nearby reference station.
- **Accuracy**: ~0.5–5 m
- **Best For**: Low-cost, general navigation with minimal hardware requirements.

### 2. Real-Time Kinematic (RTK)
- **Method**: Utilizes carrier-phase measurements and double-differencing.
- **Accuracy**: ~1–3 cm
- **Limitations**: Requires dual-frequency receiver and proximity (<20 km) to base station.

### 3. Precise Point Positioning (PPP)
- **Method**: Applies global satellite corrections without local base stations.
- **Accuracy**: ~2–10 cm
- **Drawback**: Long convergence time (20–40 mins), power-intensive.

### 4. PPP-RTK
- **Method**: Combines PPP with regional RTK-like atmospheric models.
- **Accuracy**: ~2–5 cm
- **Benefit**: Fast convergence (1–5 mins) and wide coverage.

## Smartphone Considerations

| Technique | Accuracy       | Convergence Time | Hardware Requirements         | Suitability for Smartphones |
|----------|----------------|------------------|-------------------------------|-----------------------------|
| DGNSS    | 1–3 m          | Instant          | Basic GNSS, cellular modem     | ✅ Most compatible           |
| RTK      | 1–3 cm         | Seconds          | Dual-frequency GNSS, high CPU  | ⚠️ Limited support           |
| PPP      | 2–10 cm        | 20–40 minutes    | High-end GNSS, good processing | ❌ Not real-time             |
| PPP-RTK  | 2–5 cm         | 1–5 minutes      | Dual-frequency, regional data  | ⚠️ Emerging in flagship phones |

## Urban Environment Performance

| Metric            | Best Performer        |
|------------------|-----------------------|
| Urban Resilience | **PPP-RTK**           |
| Multipath Handling | **PPP / PPP-RTK**    |
| Signal Recovery  | **PPP-RTK**           |
| Real-Time Use    | **RTK / DGNSS**       |

## Outlook

PPP-RTK is positioned to become the future standard for high-accuracy smartphone navigation, driven by:
- **Hardware advancements**: Dual-frequency GNSS chipsets in smartphones.
- **Expanded correction networks**: Greater availability of regional correction services.
- **Application demands**: AR, autonomous transport, and precision mapping.

---

### 📌 Conclusion

While DGNSS remains dominant for mainstream use, **PPP-RTK** is expected to lead advanced navigation use cases within the next 5–7 years, as mobile hardware and data infrastructure continue to evolve.

## License

This project is provided for educational purposes. Feel free to fork and build upon it for further research.

