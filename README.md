# A simplified version of Fast File Log

Original assets in unity assetstore https://www.assetstore.unity3d.com/cn/#!/content/73210.

1. put this repo into Assets folder in unity project.
2. add script LogManager.cs onto a gameobject and modify the string variable subFolder. The root folder is Application.StreamingAssets. The Subfolder is only the folder name, its default value is empty.
3. register logger using:

	LogManager.Register(gameObject.name, filename, false, true);

	gameObject.name is the key of logger and filename is the filename without path.
	
4. write to log:


	LogManager.Log(gameObject.name, logString);



