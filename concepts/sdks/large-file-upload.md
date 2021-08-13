---
title: Upload больших файлов с помощью SDKs Graph Microsoft
description: Предоставляет рекомендации по отправке больших файлов с помощью SDKs Graph Microsoft.
localization_priority: Normal
author: DarrelMiller
ms.openlocfilehash: 62949c1a309d307853443a898f2e39c6f2e8cc66a280367c418bfac67f6a702a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54211698"
---
# <a name="upload-large-files-using-the-microsoft-graph-sdks"></a>Upload больших файлов с помощью SDKs Graph Microsoft

Несколько сущностям в Microsoft [](/graph/api/driveitem-createuploadsession?view=graph-rest-1.0&preserve-view=true) Graph поддерживают повторное загрузку файлов, чтобы упростить отправку больших файлов. Вместо того, чтобы пытаться загрузить весь файл в одном запросе, файл нарезается на мелкие части, и для отправки одного среза используется запрос. Чтобы упростить этот процесс, корпорация Майкрософт Graph SDKs реализует задачу загрузки больших файлов, которая управляет загрузкой срезов.

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
IProgressCallback callback = new IProgressCallback() {
    @Override
    // Called after each slice of the file is uploaded
    public void progress(final long current, final long max) {
        System.out.println(
            String.format("Uploaded %d bytes of %d total bytes", current, max)
        );
    }
};

DriveItemCreateUploadSessionParameterSet uploadParams =
    DriveItemCreateUploadSessionParameterSet.newBuilder()
        .withItem(new DriveItemUploadableProperties()).build();

// Create an upload session
UploadSession uploadSession = graphClient
    .me()
    .drive()
    .root()
    // itemPath like "/Folder/file.txt"
    // does not need to be a path to an existing item
    .itemWithPath(itemPath)
    .createUploadSession(uploadParams)
    .buildRequest()
    .post();

LargeFileUploadTask<DriveItem> largeFileUploadTask =
    new LargeFileUploadTask<DriveItem>
        (uploadSession, graphClient, fileStream, streamSize, DriveItem.class);

// Do the upload
largeFileUploadTask.upload(0, null, callback);
```

---

## <a name="resuming-a-file-upload"></a>Повторное загрузка файла

Служба поддержки Graph Майкрософт поддерживает [повторное](/graph/api/driveitem-createuploadsession?view=graph-rest-1.0&preserve-view=true#resuming-an-in-progress-upload)загрузку в процессе выполнения. Если во время загрузки приложение сталкивается с прерываемой связью или состоянием HTTP 5.x.x, вы можете возобновить отправку.

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
