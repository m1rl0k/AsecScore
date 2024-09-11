# Application Security Scoring System

Total Points: 100

## Static Code Analysis and Secret Detection (20 points)
1. Sonarqube implemented (10 points)
2. Gitleaks or similar secret detection tool implemented (10 points)

## Repository Coverage (10 points)
3. All repositories covered by security checks (5 points)
4. All branches covered by static analysis (5 points)

## Deployment and Pipeline (25 points)
5. Runner/Agent Security (10 points)
   - Self-hosted runners/agents used (10 points)
   - Public runners used with appropriate security measures (5 points)
   - Public runners used without additional security measures (0 points)
6. Repository and Pipeline Location (5 points)
   - GitHub: 2.5 points
   - Azure DevOps: 2.5 points
7. Secrets management in Azure/AWS with OIDC implemented (5 points)
   - Azure: Service Principal with OIDC (2.5 points)
   - AWS: GitHub IDP in IAM with ARN/branch scoped role (2.5 points)
8. Use of Secure Secret Management Services (5 points)
   - Azure Key Vault or AWS Secrets Manager implemented (5 points)
   - Partial implementation or alternative service used (3 points)
   - No secure secret management service used (0 points)

## Code Nature and Analysis (15 points)
9. Appropriate analysis based on language and potential vulnerabilities (SSRF, Certs, XSS, Injection, WebSockets, etc.) (10 points)
10. Combination of static analysis and human observation (5 points)

## Historical Security (5 points)
11. No prior data breaches (5 points)

## Network Security (15 points)
12. Private endpoints implemented (5 points)
13. Security groups / ACL reviewed (5 points)
14. Web Application Firewall (WAF) implemented (5 points)

## Additional Security Measures (10 points)
15. Security headers implemented (3 points)
16. Storage (S3/Blob) reviewed, Shared Access Key (SAK) properly managed (4 points)
17. Account secret rotation implemented (3 points)

## Scoring Guide
- 90-100: Excellent security posture
- 80-89: Good security posture, minor improvements needed
- 70-79: Moderate security posture, several improvements required
- 60-69: Fair security posture, significant improvements needed
- Below 60: Poor security posture, urgent improvements required

To use this scoring system:
1. Evaluate each item and assign the corresponding points if the security measure is properly implemented.
2. Sum up the total points.
3. Compare the total to the scoring guide to assess the overall security posture.
4. Use the results to prioritize areas for improvement in the application's security.
