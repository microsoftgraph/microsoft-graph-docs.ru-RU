---
title: Отправка больших файлов с помощью SDKs Microsoft Graph
description: Предоставляет рекомендации по отправке больших файлов с помощью SDKs Microsoft Graph.
localization_priority: Normal
author: DarrelMiller
ms.openlocfilehash: 54ff14071a81ac286cebbd785216c02dc9cf6c23
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50948639"
---
# <a name="upload-large-files-using-the-microsoft-graph-sdks"></a>Отправка больших файлов с помощью SDKs Microsoft Graph

Несколько сущностям в Microsoft Graph поддерживают [повторное](/graph/api/driveitem-createuploadsession?view=graph-rest-1.0&preserve-view=true) загрузку файлов, чтобы упростить отправку больших файлов. Вместо того, чтобы пытаться загрузить весь файл в одном запросе, файл нарезается на мелкие части, и для отправки одного среза используется запрос. Чтобы упростить этот процесс, SDKs Microsoft Graph реализует большую задачу загрузки файлов, которая управляет загрузкой срезов.

## <a name="c"></a>[C#](#tab/csharp)

```csharp
using (var fileStream = System.IO.File.OpenRead(filePath))
{
    // Use properties to specify the conflict behavior
    // in this case, replace
    var uploadProps = new DriveItemUploadableProperties
    {
        ODataType = null,
        AdditionalData = new Dictionary<string, object>
        {
            { "@microsoft.graph.conflictBehavior", "replace" }
        }
    };

    // Create the upload session
    // itemPath does not need to be a path to an existing item
    var uploadSession = await graphClient.Me.Drive.Root
        .ItemWithPath(itemPath)
        .CreateUploadSession(uploadProps)
        .Request()
        .PostAsync();

    // Max slice size must be a multiple of 320 KiB
    int maxSliceSize = 320 * 1024;
    var fileUploadTask =
        new LargeFileUploadTask<DriveItem>(uploadSession, fileStream, maxSliceSize);

    // Create a callback that is invoked after each slice is uploaded
    IProgress<long> progress = new Progress<long>(prog => {
        Console.WriteLine($"Uploaded {prog} bytes of {fileStream.Length} bytes");
    });

    try
    {
        // Upload the file
        var uploadResult = await fileUploadTask.UploadAsync(progress);

        if (uploadResult.UploadSucceeded)
        {
            // The ItemResponse object in the result represents the
            // created item.
            Console.WriteLine($"Upload complete, item ID: {uploadResult.ItemResponse.Id}");
        }
        else
        {
            Console.WriteLine("Upload failed");
        }
    }
    catch (ServiceException ex)
    {
        Console.WriteLine($"Error uploading: {ex.ToString()}");
    }
}
```

## <a name="typescript"></a>[TypeScript](#tab/typescript)

```typescript
const options: any = {
    // Relative path from root to destination folder
    path: itemPath,
    // file is a File object, typically from an <input type="file"/>
    fileName: file.name,
    rangeSize: 320 * 1024
  }

  try {
    const uploadTask: MicrosoftGraph.OneDriveLargeFileUploadTask =
      await MicrosoftGraph.OneDriveLargeFileUploadTask.create(client, file, options);

    const uploadedFile: DriveItem = await uploadTask.upload();

    console.log(JSON.stringify(`Uploaded file with ID: ${uploadedFile.id}`));
    return `Uploaded file with ID: ${uploadedFile.id}`;
  } catch (err) {
    console.log(`Error uploading file: ${JSON.stringify(err)}`);
    return `Error uploading file: ${JSON.stringify(err)}`;
  }
}
```

## <a name="java"></a>[Java](#tab/java)

```java
// Get an input stream for the file
File file = new File(localFilePath);
InputStream fileStream = new FileInputStream(file);
long streamSize = file.length();

// Create a callback used by the upload provider
IProgressCallback<DriveItem> callback = new IProgressCallback<DriveItem>() {
    @Override
    // Called after each slice of the file is uploaded
    public void progress(final long current, final long max) {
        System.out.println(
            String.format("Uploaded %d bytes of %d total bytes", current, max)
        );
    }
};

// Create an upload session
UploadSession uploadSession = graphClient
    .me()
    .drive()
    .root()
    // itemPath like "/Folder/file.txt"
    // does not need to be a path to an existing item
    .itemWithPath(itemPath)
    .createUploadSession(new DriveItemUploadableProperties())
    .buildRequest()
    .post();

LargeFileUploadTask<DriveItem> largeFileUploadTask =
    new LargeFileUploadTask<DriveItem>
        (uploadSession, graphClient, fileStream, streamSize, DriveItem.class);

// Config parameter is an array of integers
// customConfig[0] indicates the max slice size
// Max slice size must be a multiple of 320 KiB
int[] customConfig = { 320 * 1024 };

// Do the upload
largeFileUploadTask.upload(callback, customConfig);
```

---

## <a name="resuming-a-file-upload"></a>Повторное загрузка файла

SDKs Microsoft Graph поддерживают [повторное](/graph/api/driveitem-createuploadsession?view=graph-rest-1.0&preserve-view=true#resuming-an-in-progress-upload)загрузку в процессе выполнения. Если во время загрузки приложение сталкивается с прерываемой связью или состоянием HTTP 5.x.x, вы можете возобновить отправку.

<!-- markdownlint-disable MD024 -->
### <a name="c"></a>[C#](#tab/csharp)

```csharp
fileUploadTask.ResumeAsync(progress);
```

### <a name="typescript"></a>[TypeScript](#tab/typescript)

```typescript
const resumedFile: DriveItem = await uploadTask.resume();
```

### <a name="java"></a>[Java](#tab/java)

> [!NOTE]
> В настоящее время SDK Java не поддерживает повторное скачивание в процессе выполнения.

---
<!-- markdownlint-enable MD024 -->
