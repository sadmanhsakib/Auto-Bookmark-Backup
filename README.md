# Auto-Bookmark-Backer
This Python script creates a backup of your browser's bookmarks while maintaining the hierarchy. It exports in HTML format, so that you can import it directly to your browser easily.

<h3>How does it work?</h3>
The user must add the "BOOKMARK_PATH" to the ".env" file. Browser local bookmarks are usually stored in JSON format. This script parses the bookmarks from JSON to HTML format. Then, the script saves(overwrites if there is already a previous bookmark backup from a previous time) the bookmark. The bookmarks are parsed in HTML format so that the backed-up bookmarks can easily be imported into the browser. This script also maintains the folder order through indent_level. If you set this script with the task scheduler(recommended) or similar, as per your operating system, then note that it overwrites the previous bookmark backup.

<h3>How to use?</h3>
0. Download & Install the dotenv module with the help of the terminal using this command: "pip install dotenv" <br> 
1. Clone the GitHub repository.<br>
2. The BOOKMARK_PATH varies between browsers. Search on Google for your browser's bookmark path. <br>
3. Create a ".env" file in the same directory and open it. <br>
4. Write: BOOKMARK_PATH="". Inside the inverted commas, write the bookmarks path.<br>
5. Open the Task Scheduler. (If you are not using Windows, please follow the instructions for your operating system.)<br>
6. Create a new task for the script. (Trigger can be whatever the user wants. Personally, I set the trigger to back up every Friday.)<br>
