# Expert Ruby & Ruby on Rails Software Engineer

- You are an expert Ruby and Ruby on Rails software engineer.
- You have a deep understanding of the Ruby language, its various libraries and gems.
- You have a deep understanding of the Ruby on Rails framework, including its conventions and best practices.
- You excel at writing clean, efficient, and maintainable code.
- You are also familiar with best practices for Ruby and Ruby on Rails development, including proper use of libraries, gems, code organization, testing, and documentation.

# Refactoring Ruby & Rails Code

- I want you to review this code and provide feedback on its readability, maintainability, and adherence to best practices.
- Please provide specific suggestions with examples on how the code can be improved.
- All functions should have type annotations and docstrings.
- The code should have sufficient unit test coverage.
- The code should have proper error handling and logging.
- If a function is doing too much, it should be refactored into two or more smaller functions.

## Prompt





# Expert Ruby & Ruby on Rails Software Engineer

- You are an expert Ruby and Ruby on Rails software engineer.
- You have a deep understanding of the Ruby language, its various libraries and gems.
- You have a deep understanding of the Ruby on Rails framework, including its conventions and best practices.
- You excel at writing clean, efficient, and maintainable code.
- You are also familiar with best practices for Ruby and Ruby on Rails development, including proper use of libraries, gems, code organization, testing, and documentation.

- I want to consume data from a third part API and save it's contents into the database for my Rails app.
- The URL looks like this: https://wts.populiweb.com/api2/{academic_term_id}/enrollments where {academic_term_id} is the id of the academic term. I have several academic term ids.

- Here is an example of the response:

```json
{
  "object": "list",
  "count": 200,
  "results": 987,
  "results_per_page": 200,
  "pages": 5,
  "page": 1,
  "offset": 0,
  "has_more": true,
  "data": [
    {
      "object": "person",
      "id": 24544524,
      "first_name": "Jennifer",
      "last_name": "Adams",
      "middle_name": "",
      "prefix": null,
      "suffix": null,
      "preferred_name": null,
      "display_name": "Jennifer Adams",
      "gender": "female",
      "other_gender": null,
      "raceid": 0,
      "image_file_id": 90548201,
      "birth_date": "1973-12-18",
      "status": "active",
      "social_security_number": "280781865",
      "alien_registration_number": null,
      "social_insurance_number": null,
      "home_city": null,
      "home_state": null,
      "home_country": null,
      "former_name": null,
      "license_plate": null,
      "bio": null,
      "updated_at": "2024-06-03T14:23:36+00:00",
      "hispanic_latino": false,
      "resident_alien": false,
      "localization_id": null,
      "notification_email_id": null,
      "deceased_date": null,
      "added_by_id": 15642134,
      "added_at": "2021-12-03T18:16:28+00:00",
      "import_id": null,
      "report_data": {
        "student_person_id": 24544524,
        "student_name": "Jennifer Adams",
        "academic_term_id": 302412,
        "academic_term_name": "2023-2024: March",
        "catalog_course_abbrv": "PRAX Mentor",
        "course_offering_id": 10737689,
        "full_course_offering_name": "PRAX Mentor-1: PRAX Mentorship",
        "course_student_status": "ENROLLED",
        "status_mapid": null,
        "status_map_abbrv": null,
        "programid": 0,
        "program_name": null,
        "grade_abbrv": "P",
        "grade": "100.00",
        "enrollment_id": 78503506,
        "course_offering_student_program_id": null,
        "pass_fail": 1,
        "student_middle_name": "",
        "student_preferred_name": "",
        "academic_term_start_date": "2024-03-18",
        "course_campus_id": 6740,
        "academic_term_end_date": "2024-05-25",
        "student_first_name": "Jennifer",
        "student_last_name": "Adams",
        "course_offering_section": "1",
        "course_offering_name": "PRAX Mentorship",
        "credits": "0.00",
        "hours": "0.00",
        "retake": null,
        "course_campus_name": "Online Campus",
        "finalized": 1,
        "program_units": "CREDITS",
        "catalog_course_id": 1844020,
        "row_id": "24544524_0_10737689"
      },
      "student_degrees": [
        {
          "object": "student_degree",
          "id": 4610863,
          "student_id": 24544524,
          "degree_id": 37814,
          "status": "active",
          "graduation_date": null,
          "active_date": "2022-01-03",
          "inactive_date": null,
          "catalog_year_id": 74209,
          "anticipated_completion_date": null,
          "show_on_transcript": true,
          "degree": {
            "object": "degree",
            "id": 37814,
            "program_id": 25214,
            "department_id": 0,
            "name": "Master of Arts in Counseling",
            "description": "Online",
            "abbrv": "MAC",
            "diploma": 1,
            "status": "active",
            "cip_code": "39.0705",
            "degree_level_id": 3,
            "unit": "credits",
            "distance_education": true,
            "length": 2,
            "length_unit": "years",
            "external_id": null
          }
        }
      ],
      "private_profile": false,
      "is_user": true
    }
  ],
  "sandbox": false
}
```

An an expert Ruby and Ruby on Rails software engineer, I want you to design and architect the best solution for what I am trying to do. I am not sure how to handle the relationships in the response.

- I want to create a rake task that will import the data from the API into my database.
- I want to create a service object that will handle the import of the data from the API into my database.
- I want to create a model that will handle the relationships in the response.
- I want to create a migration that will handle the creation of the tables in the database.
- I want to create a seed file that will handle the seeding of the database with the data from the API.