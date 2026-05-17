## A. Executive Summary
Veridi Logistics delivers ~99,441 orders across Brazil. Our audit found that 
8.1% of delivered orders arrive later than the estimated date, with Cross states (AL, MA, PI) experiencing late rates exceeding 20%. Late 
deliveries directly correlate with poor reviews — on-time orders average 4.38/5 
while super-late orders average 2.04/5, confirming the CEO's hypothesis that 
over-promising on delivery dates is driving customer dissatisfaction.

## B. Project Links
- **Notebook:** https://colab.research.google.com/drive/1ows_OfVu5l4dB5ifvHNYoylkom6zoj23?usp=sharing
- **Dashboard:** https://datastudio.google.com/reporting/47032c53-1782-4edb-b18c-5b76d74e1554
- **Presentation:** [/Amalitech Bobs Presentation.pdf](https://github.com/bob-aila/Amalitech-Project-BOB/blob/main/Amalitech%20Bobs%20presentation.pdf)

## C. Technical Explanation
**Data Cleaning:** Deduplicated reviews (kept latest per order), separated 
non-delivered orders before calculating delay metrics, filled categorical nulls 
with "Uncategorized"/"Unknown", and left numeric delay/review nulls as NaN to 
avoid corrupting averages.

**Candidate's Choice:** Cross-State vs Same-State shipment analysis. Same-state 
orders achieve 93.9% on-time rate vs 90.7% for cross-state, with a 0.3-point 
review score gap. This tells Veridi that regional fulfilment centre expansion 
would have more impact than carrier-level negotiations.
