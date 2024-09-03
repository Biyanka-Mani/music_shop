# Music Shop App 🎵

This is a Ruby on Rails application that simulates a music shop, where users can browse and purchase albums. The app also demonstrates the usage of the `acts_as_paranoid` gem for soft deletion and the `gretel` gem for breadcrumbs navigation.

## Features

- **Album Management:** Create, read, update, and soft-delete albums.
- **Artist Management:** Manage artists associated with albums.
- **Soft Deletion:** Implemented using the `acts_as_paranoid` gem, allowing albums to be "deleted" but still recoverable.
- **Breadcrumb Navigation:** Enhanced user navigation with breadcrumbs, powered by the `gretel` gem.

## Gems Used

### `acts_as_paranoid`
The `acts_as_paranoid` gem is used to implement soft deletion in the application. When a record is "deleted," it is not actually removed from the database but is instead marked as deleted by setting a `deleted_at` timestamp. This allows the record to be restored later if needed.

- **Installation:** Add the gem to your `Gemfile`:
  ```ruby
  gem 'acts_as_paranoid'

