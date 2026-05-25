job_records = ["J101", "J102", "J102", "J103", "J101", "J104"]

unique_jobs = []

for record in job_records:
    is_duplicate = False

    for item in unique_jobs:
      if record == item:
    # duplicate record detected
    print(record, "is duplicate and skipped")
    is_duplicate = True
    break

    if is_duplicate == False:
        unique_jobs.append(record)

print("Original Records:", job_records)
print("Unique Records:", unique_jobs)
