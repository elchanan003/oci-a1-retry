# oci-a1-retry

Scheduled GitHub Actions workflow that keeps trying to launch an Oracle Cloud
free-tier Ampere (A1) instance when the region reports "Out of host capacity".
Runs every ~10 minutes, 9 attempts per run, and auto-stops once the instance
is created. All credentials are stored as encrypted repository secrets, never
in the code.
