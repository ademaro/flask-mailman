# Release Notes

## 0.2.3

### Added

- Add support for Flask 2.0

### Removed

- Drop support for Python 3.5(due to flask upgrade).

## 0.2.2

### Changed

- Set `None` as the default value for the `from_email` and `recipient_list` of `send_mail()` function.

## 0.2.0

A few breaking changes have been made in this version to ensure that API of this extension is basically the same as Django. 
Users migrating from Flask-Mail should upgrade with caution.

### Added

- Add documentation site hosted in GitHub Pages.

### Changed

- Set configuration value of in-memory backend to 'locmem'.
- Set MAIL_SERVER default value to 'locaohost'.
- Set MAIL_USE_LOCALTIME default value to False.

### Removed

- Remove `Mail.send()` method and `Message()` class which borrowing from Flask-Mail.
- Remove `mail_admins()` and `mail_managers()` method that come from Django.