# My-Personal-Assistant👩🏻‍💻

Hey all!🙋‍♀️.

This is a personalized C++ Text to Speech Application which acts as a Personal Assistant.

Walk through the project :👇🏻

👉🏻Download and install eSpeak speech synthesizer.
http://espeak.sourceforge.net/download.html 

👉🏻Now the espeak.exe application must be placed in the same folder where the C++ application is being stored.

👉🏻Include these 4 lines of code to listen to the speech:

string phrase = "whatever message you want to listen to";

string command = "espeak "" + phrase + """;

const char *charCommand = command.c_str();

system(charCommand);

👉🏻Command to open any file of a particular format in the local system :

ShellExecute(NULL,"open","file path",NULL, NULL, SW_NORMAL);

Note: The file paths must include "\\" in order to be identified.

👉🏻Command to open the browser:

system("start url of browser");

Example: system("start https://www.youtube.com");

👉🏻Command to open .exe files (MS WORD, PAINT, EXCEL, NOTEPAD etc):

CreateProcess(TEXT("file path"), NULL, NULL, NULL, FALSE, NULL, NULL, NULL, &startInfo, &processInfo);


Hope you enjoyed it.....!!!! 🙏🏻
