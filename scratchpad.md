# Expert Rust

- You are an expert Rust software engineer.
- You have a deep understanding of the Rust language, cargo and its various libraries and packages.
- You excel at writing clean, efficient, and maintainable code.
- You are also familiar with best practices for Rust development, including proper use of libraries, packages, code organization, testing, and documentation.
- You also practice test-driven development and write unit tests.
- I want you to review the code I have so far and improve upon it.
- Please help with modeling the data structures and writing the code to consume the API and save the data to the database.
- Please reference and use the environment variables in the .env file.
- Please also provide proper error handling and logging.
- The api also uses pagination. You will need to handle the pagination for the api.

- Here is the URL to the API: `{BASE_URL}/academicterms`. {BASE_URL} is an environment variable and is located in the .env file.

- Here is an example of the response:

```json
{
  "object": "list",
  "count": 418,
  "results": 418,
  "results_per_page": null,
  "pages": 1,
  "page": 1,
  "offset": 0,
  "has_more": false,
  "data": [
    {
      "object": "academic_term",
      "id": 302460,
      "academic_year_id": 74212,
      "name": "Fall",
      "display_name": "2025-2026: Fall",
      "start_date": "2025-09-11",
      "end_date": "2025-11-20",
      "grades_date": "2025-12-04",
      "add_drop_time": "2025-09-25T04:00:00+00:00",
      "enrollment_start_time": null,
      "enrollment_end_time": null,
      "max_enrolled_credits": null,
      "max_enrolled_hours": null,
      "max_audit_credits": null,
      "max_audit_hours": null,
      "non_standard": false,
      "type": "standard",
      "evaluations_available_from": null,
      "evaluations_available_to": null,
      "evaluations_lock_grades_at": null,
      "online_registration_delay_until": null,
      "online_registration_randomization_seconds": 0,
      "evaluations_lock_grades_until": null,
      "evaluations_available_to_faculty": null,
      "lms_sync": null,
      "external_id": null,
      "added_at": "2024-07-11T20:27:25+00:00",
      "added_by_id": 13160768,
      "start_year": 2025,
      "end_year": 2026
    }
  ],
  "sandbox": false
}

```

I want to write the data located in the `data` array to a csv file. The csv file should have a header row and each row should contain the corresponding data from the `data` array.