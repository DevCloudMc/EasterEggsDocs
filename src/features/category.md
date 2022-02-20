# Categories

You can create several easter egg categories and assign different access rights to them for users.
For example, you have two categories, one of which is accessible to player A and one of which is not.
The access to the category is configured through the permissions `ee.type.<category_name>`

To create a new category type `/ee category create <category_name>`.

To delete any category type `/ee category delete <category_name>`. _If easter eggs from this category were already found by someone
they will be deleted from the database._
