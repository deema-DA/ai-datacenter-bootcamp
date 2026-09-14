# Service report


Team:Lihyan
Use case: Baseline chat completion service serving chat requests to users
Service and model: Qwen/Qwen2.5-1.5B-Instruct-AWQ, /v1/chat/completions
Measured requests or tasks: 120 chat completion requests
Indicator and unit: p95 time to first token (TTFT), seconds
SLO target and window: < 1.0 second over a 5-minute window
Measurement start and end: 2026-09-13T12:47:53+00:00 to 2026-09-13T12:50:53+00:00
Workload: Artificial chat traffic with max_tokens=64, using one caller followed by four concurrent callers
Observed result and sample count: 0.039 seconds (39 ms) p95 TTFT; 120 requests generated
Evidence: Grafana p95 Time to First Token panel and traffic.py output
Conclusion: MET — observed p95 TTFT was below the provisional 1.0-second SLO target during the measured workload
Limitations: The workload was short and artificial, so it does not establish compliance over a longer SLO window. Output quality and HTTP status outcomes were not measured.
Follow-up action: Repeat the measurement with longer and more representative traffic before treating this target as a production SLO.


## Measurement query

Paste the expression used to produce the reported value. Give its evaluation
time or range. Explain where the measurement is taken and what it excludes.

## Service alert

Condition and unit:
Evaluation interval:
Pending period:
Relationship to the SLO:
First response to a notification:

## Notification test

Firing received at:
Resolved received at:
What the test establishes:
