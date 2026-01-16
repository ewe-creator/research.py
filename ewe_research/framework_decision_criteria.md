# Decision Criteria & Impact Modeling

To maintain a high-impact framework, every architectural decision must be weighed against its potential to generate **Testimonial Value**.

## 1. Testimonial Importance Rate (TIR)

Not all feedback is equal. We calculate the **Importance Rate** of a testimonial based on its ability to drive adoption (The Validation Loop).

### The Formula
`TIR = (Credibility + Detail + Outcome) × Recency`

*   **High TIR (Critical)**: "We migrated our core payment engine to Ewe Creator and reduced latency by 40%." (Specific, High Stakes, Clear Outcome).
*   **Low TIR (Noise)**: "Great framework, love it." (Generic, No Data).

### Strategic Use
*   **Prioritize features** that enable High TIR stories.
*   *Example*: Building a "Zero-Downtime Deployment" plugin is high priority because users who thrive on it write powerful case studies.

## 2. Implementation Model Decision Matrix

When deciding **how** to implement a feature, use this matrix to ensure stability and market growth.

| Criteria | **Option A: Core Integration** | **Option B: Official Plugin** | **Option C: Community Recipe** |
| :--- | :--- | :--- | :--- |
| **Stability Risk** | High (Affects everyone) | Low (Isolated) | None (User responsibility) |
| **Maintenance Cost** | High (Forever support) | Medium | Low |
| **TIR Potential** | Medium (Expected baseline) | **High** (Solves specific pain) | Low |
| **Decision Rule** | Only if critical for 80% of users. | **Preferred Default.** | For niche/experimental logic. |

> [!TIP]
> **The Golden Rule**: If a feature allows a user to tell a specific, data-backed success story, build it as a **First-Class Plugin**.
