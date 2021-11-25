# My_AsyncTask1
Async Task, Dynamic url based image downloader
* Sample app to demonstrate the communication between the Main thread and the Worker thread.
* The long running operations are done in the background in android. This is because, such operations make the UI to be freezed until the operation is complete. To have the better UI interaction, such operation are done in the background and the result is updated to the main UI.
* The main UI runs in the main thread and the background operations are done in the worker threads.
* The long running operation could be network operations like downloads, playing music etc,.
* In our application, the AsyncTask service is used as the background thread.
1) onPreExecute() - All the initializations (like setting up progress bar) are done here before starting the actual background task.
2) doInBackground() - Actual background task is implemented here (In our case downloading the image from the url)
4) onPostExecute() - After the background task completes (can be success or failure), this is further updated to the main UI (Main Thread).
* User can enter the valid image URL and search, the downloaded image is displyed on the screen
