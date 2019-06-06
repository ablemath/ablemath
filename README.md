# Able Math Website

## Maintenance

### Adding a New Year
Four files need to be provided (you can always symlink to another one from a
previous year if needed):
* calendar.pdf
* curriculum.pdf
* regform.pdf
* summer.pdf

Create a new folder for the year in the `docs/` folder, and move the four files
in place.

Update `_config.yml` with the following values:
* Registration Date: `registrationdate` (yyyy-MM-dd format)
* First Day of Classes: `classdate` (yyyy-MM-dd format)

Test the changes. Run `jekyll serve [-H 0.0.0.0 -P 30000]` and check:
* `/program/` has correct curriculum and calendar.
* `/registration/` has correct date and registration form.
* `/` has correct dates

Additionally, you will need to create a new announcement.

### Create New Announcement

Copy the most recent entry in `/_posts/` to a new version.
