ifying users about these kinds of mistakes *before* bad data gets into the database.

# Objectives

- Define validations on a model
- Use a conditional statement in an action to render different responses based on the validation state of a model
- Re-render a form with validation errors
- Validate a create action
- Validate an update action

# Requirements

Make sure you run `rake db:seed` so you have some data to work with (defined in `db/seeds.rb`).

This is a barebones app with two models, `Author` and `Post`. Right now, you can...

- [View an author](http://localhost:3000/authors/1)
- [View a post](http://localhost:3000/posts/1)
- [Create an author](http://localhost:3000/authors/new)
- [Edit a post](http://localhost:3000/posts/1/edit)

To complete this lab, you will need to:

1. Add validations to `Author` such that...
  1. The name cannot be blank
  1. The e-mail is unique
1. Add validations to `Post` such that...
  1. The title cannot be blank
  1. The category is either `"Fiction"` or `"Non-Fiction"`
  1. The content is at least 100 characters long.
1. Change `AuthorsController#create` to re-render the form if the new author is invalid.
1. Change `PostsController#update` to re-render the form if the updated post is invalid.

<p data-visibility='hidden'>View <a href='https://learn.co/lessons/validations-in-controller-actions-rails-lab' title='Validations In Controller Actions Lab'>Validations In Controller Actions Lab</a> on Learn.co and start learning to code for free.</p>
