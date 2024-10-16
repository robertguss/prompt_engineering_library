# Finance Integration Documentation

You are an expert at Python and Django, and you are helping me document this project.

## Project Description

This Django-based project is a financial integration system designed to automate and synchronize financial processes across multiple platforms, including Intacct (accounting software), Stripe (payment processing), and Populi (student information system).

## Project Structure

```console
.
├── Makefile
├── Procfile
├── README.md
├── Vagrantfile
├── app.json
├── docs
│   ├── finance_integration.md
│   ├── intacct.md
│   ├── integration.md
│   ├── overview.md
│   └── stripe_event_handler.md
├── finance_integration
│   ├── __init__.py
│   ├── celery.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
├── functional_tests
│   ├── __init__.py
│   ├── data
│   │   ├── getPerson.xml
│   │   ├── transactions.singleton.response.failure.xml
│   │   ├── transactions.singleton.response.xml
│   │   ├── transactions.singleton.xml
│   │   └── transactions.xml
│   ├── test_commands.py
│   └── test_webhooks.py
├── intacct
│   ├── __init__.py
│   ├── admin.py
│   ├── api.xsd
│   ├── apps.py
│   ├── exceptions.py
│   ├── migrations
│   │   └── __init__.py
│   ├── models.py
│   ├── templates
│   │   ├── address.xml
│   │   ├── apbill.xml
│   │   ├── apbillitem.xml
│   │   ├── base.xml
│   │   ├── contact.xml
│   │   ├── contactlistinfo.xml
│   │   ├── contactname.xml
│   │   ├── customfield.xml
│   │   ├── delete.xml
│   │   ├── glbatch.xml
│   │   ├── glentry.xml
│   │   ├── legacycontactname.xml
│   │   ├── lineitem.xml
│   │   ├── potransaction.xml
│   │   ├── readbyquery.xml
│   │   ├── record_otherreceipt.xml
│   │   ├── request.xml
│   │   ├── split.xml
│   │   ├── test
│   │   │   ├── create_vendor_success.response
│   │   │   ├── create_vendor_success_and_failure.response
│   │   │   ├── function_level_error.response
│   │   │   ├── generate_api_session.response
│   │   │   ├── invalid_web_services_authorization.response
│   │   │   └── invalid_web_services_sender_id_or_password.response
│   │   ├── vendor.xml
│   │   └── vendoracctnolochead.xml
│   ├── tests
│   │   ├── __init__.py
│   │   ├── test_exceptions.py
│   │   ├── test_full_route.py
│   │   ├── test_models.py
│   │   └── test_templates.py
│   └── views.py
├── integration
│   ├── __init__.py
│   ├── actions.py
│   ├── admin.py
│   ├── apps.py
│   ├── base.py
│   ├── intacct.py
│   ├── ledger.py
│   ├── management
│   │   └── commands
│   │       ├── integration.py
│   │       ├── invoices.py
│   │       ├── receipts.py
│   │       ├── refund_invoices.py
│   │       └── refunds.py
│   ├── migrations
│   │   ├── 0001_create_task_model.py
│   │   └── __init__.py
│   ├── models.py
│   ├── populi.py
│   ├── support
│   │   ├── api.xsd
│   │   ├── conversion.csv
│   │   └── conversion_v2.csv
│   ├── tasks.py
│   ├── templates
│   │   ├── base.request
│   │   ├── create_vender.failure.response
│   │   ├── create_vender.success.response
│   │   ├── function_level_error.response
│   │   ├── generate_api_session.response
│   │   ├── intacct_objects
│   │   │   ├── address.xml
│   │   │   ├── contact.xml
│   │   │   ├── contactlistinfo.xml
│   │   │   ├── contactname.xml
│   │   │   ├── glbatch.xml
│   │   │   ├── glentry.xml
│   │   │   ├── request.xml
│   │   │   ├── split.xml
│   │   │   ├── vendor.xml
│   │   │   └── vendoracctnolochead.xml
│   │   ├── integration.txt
│   │   ├── invalid_web_services_authorization.response
│   │   └── invalid_web_services_sender_id_or_password.response
│   ├── temporary.py
│   └── tests
│       ├── __init__.py
│       ├── data
│       │   ├── Condo_Electricity_Bug.xml
│       │   ├── UnMatchedEntriesException_Bug.xml
│       │   ├── getPerson.xml
│       │   ├── getStudentInfo.xml
│       │   ├── transactions.wtsio_89.bug.xml
│       │   └── transactions.xml
│       ├── test_actions.py
│       ├── test_automate_invoices.py
│       ├── test_automate_receipts.py
│       ├── test_automate_refund.py
│       ├── test_automate_refund_invoices.py
│       ├── test_base.py
│       ├── test_intacct.py
│       ├── test_integration.py
│       ├── test_ledger.py
│       ├── test_populi.py
│       ├── test_program_inclusion.py
│       ├── test_tasks.py
│       └── test_wtsio_89.py
├── manage.py
├── provision.sh
├── requirements.txt
├── runtime.txt
└── stripe_event_handler
    ├── __init__.py
    ├── admin.py
    ├── apps.py
    ├── management
    │   └── commands
    │       └── environment.py
    ├── migrations
    │   └── __init__.py
    ├── models.py
    ├── templates
    │   └── email.txt
    ├── templatetags
    │   ├── __init__.py
    │   ├── datetime.py
    │   ├── divide.py
    │   ├── strformat.py
    │   └── xpath.py
    ├── tests
    │   ├── __init__.py
    │   ├── test_populi_api_requests.py
    │   ├── test_stripe_api_requests.py
    │   ├── test_stripe_endpoint.py
    │   └── test_stripe_template_tags.py
    └── views.py

26 directories, 143 files
```
