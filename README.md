## item editor (non-relational DB)
Enter each item for compiling an item bank (i.e., a group of multiple choice questions) and save it as json format.

## code review
This Python code defines a graphical user interface (GUI) application using the tkinter library for managing and editing items.
The application allows users to add, update, delete, and display items.
The items are stored in a JSON file and are loaded into the GUI for easy management.

Here's a breakdown of the key components and functionalities in the code:

Importing Libraries:
- The code imports necessary modules from the tkinter library for GUI components, `ttk` for themed widgets, and other required modules such as `uuid`, `json`, `os`, and `io`.

Global Variables and File Path:
- Defines a global list variable my_data_list to store item data.
- Defines a file path (FilePath) for storing item data in a JSON file (item.json).

Functions:
- `startup_check()`: Checks if the data file exists and is readable. If not, it creates a new file and writes an empty JSON array.
- `load_json_from_file()`: Loads item data from the JSON file into my_data_list.
- `save_json_to_file()`: Writes my_data_list to the JSON file.
- Various other functions for managing the GUI components, handling button actions, and processing item data.

GUI Layout:
- Creates the GUI layout using tkinter components like Labels, Entries, Buttons, Treeview (for displaying items), and Scrollbar.

Event Handling:
- Binds events to the Treeview to handle mouse clicks and selection of items.
- Defines functions to handle button clicks and update the GUI based on user actions.

Main Execution:
- Starts the main GUI event loop using `root.mainloop()`.

Overall, this code creates a simple item editor GUI that interacts with a JSON file to manage itemset data.
