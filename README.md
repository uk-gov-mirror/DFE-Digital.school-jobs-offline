# Offline page for Teaching Vacancies
- uses the generated HTML version of the [GOV.UK template](https://alphagov.github.io/govuk_template/)
- govuk-elements-sass compiled from the command line (`sass --style expanded --line-numbers --load-path node_modules/govuk_frontend_toolkit/stylesheets assets/stylesheets/styles.scss assets/stylesheets/styles.css`)

# Contributing
We use GitHub and pull requests into master that required 1 person to review.

# Deployment
1. Open a browser and navigate to the source files in the AWS S3 bucket https://s3.console.aws.amazon.com/s3/buckets/tvs-offline/?region=eu-west-2&tab=overview
2. You should see a single folder called 'school-jobs-offline', click upload
3. Clone this repository locally
4. Checkout master and ensure you're up to date with the remote master branch
5. Drag the whole repository folder into the AWS web console
6. 'Manage public permissions' should be set to public. The rest can remain as default. Next
7. Choose 'Standard-IA' as the storage class. Next
8. Upload - you should see the contents of the file change and be able to view them via Teaching Vacancies here https://teaching-jobs.service.gov.uk/school-jobs-offline/index.html
