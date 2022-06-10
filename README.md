# Query Statistic for Specific Subdistrict

This function is meant to be deployed as a serverless function via GCP's cloud run. run the function locally with npm start, and then do a

```bash
curl -X POST http://localhost:8080 -H "Content-Type:application/json"  -d '{"sub
district":"Tanjung Priok"}'
```

to get a response like

```bash
{
  "subdistrict": "Tanjung Priok",
  "total_crime": 80,
  "crime_info": {
    "Aggravated Assault": 2,
    "Aiding and Abetting / Accessory": 1,
    "Arson": 2,
    "Assault / Battery": 2,
    "Attempt": 6,
    "Child Abandonment": 2,
    "Conspiracy": 1,
    "Cyberbullying": 2,
    "Disorderly Conduct": 4,
    "Disturbing the Peace": 1,
    "Forgery": 2,
    "Fraud": 1,
    "Harassment": 5,
    "Homicide": 3,
    "Kidnapping": 4,
    "Manslaughter: Involuntary": 2,
    "Manslaughter: Voluntary": 5,
    "Murder: First-degree": 4,
    "Murder: Second-degree": 3,
    "Open Container (of alcohol)": 1,
    "Pyramid Schemes": 1,
    "Rape": 4,
    "Robbery": 5,
    "Securities Fraud": 1,
    "Sexual Assault": 3,
    "Solicitation": 1,
    "Stalking": 6,
    "Statutory Rape": 3,
    "Theft": 3
  }
}
```

## Docker Support

run build_image.sh to build a docker file (make sure you have docker with pack tool installed)