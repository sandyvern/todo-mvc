# Step 1: Integrate Basic Theme to Asset Pipeline

[X] / - And see a stubbed out, non-dynamic, page with the theme.

# Step 2: Allow people to CRUD lists.

[]List Controller
  - see all their lists
  - doubling as my #new action in that it is presenting the person witha form to create a new list
  / - Index all the lists...
  - create a lists

  - show a list

I want people to be able to create lists. Then they should be able to add items to those lists. They should be able to navigate to many lists and see each others lists items.

lists
  has many items

items
  belongs to a list
