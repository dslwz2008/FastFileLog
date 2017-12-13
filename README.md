# A simplified version of Fast File Log

Original assets in unity assetstore https://www.assetstore.unity3d.com/cn/#!/content/73210.

1. put this repo into Assets folder in unity project.
2. add script LogManager.cs onto a gameobject and modify the savepath.
3. register logger using:

	LogManager.Register(gameObject.name, filename, false, true);

4. write to log:

	LogManager.Log(gameObject.name, logString);



