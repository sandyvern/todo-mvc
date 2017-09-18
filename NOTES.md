# Step 1: Integrate Basic Theme to Asset Pipeline

[X] / - And see a stubbed out, non-dynamic, page with the theme.

# Step 2: Allow people to CRUD lists.

[]List Controller
  - see all their lists
  - doubling as my #new action in that it is presenting the person witha form to create a new list
  / - Index all the lists...
  - create a lists

  - show a list

  - need a model
  - need a Controller
  - should a generate a resource

  Does it impact the DB?
  Does it impact my URLS?

  # Step 3: Add Items to a List

  - Make the items in my list real
    - a list has many items and an item belongs to a list
  - Does it impact my URLS? -
      CREATE ACTION for an ITEM in a LIST. What is the URL/HTTP method for that?
      - The form is already present in the list show page
      - What URL does this form imply?

      POST /items => this doesn't describe which list we are adding an item to
        Should be a NESTED RESOURCE - items are nested in terms of URLs under their parent list =>
          POST /lists/:id/items

      An item doesn't exist in our application outside of the context of the list it belongs to

  - Does it impact the DB? -
      I probably need an ITEMS table, associated with a particular list

  # Step 4: Adding Validations
    - Validate that lists have a name
    - Validate that items have a description

  # Step 5: I want to add state (complete, incomplete) to Items in a List

    - Marking items as complete or incomplete

  # Step 6: Deleting Items from a list

  # Step Whatever: Fix down arrow on Make a List Form

I want people to be able to create lists. Then they should be able to add items to those lists. They should be able to navigate to many lists and see each others lists items.

lists
  has many items

items
  belongs to a list
