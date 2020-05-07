---
title: Отправка больших файлов с помощью пакетов SDK Microsoft Graph
description: Предоставляет рекомендации по отправке больших файлов с помощью пакетов SDK Microsoft Graph.
localization_priority: Normal
author: DarrelMiller
ms.openlocfilehash: 04d9591350e620f92cd7d699b88371ae05c3634f
ms.sourcegitcommit: df2c52f84aae5d4fed641d7411ba547371f0eaad
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2020
ms.locfileid: "44052550"
---
# <a name="upload-large-files-using-the-microsoft-graph-sdks"></a><span data-ttu-id="80b7e-103">Отправка больших файлов с помощью пакетов SDK Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="80b7e-103">Upload large files using the Microsoft Graph SDKs</span></span>

<span data-ttu-id="80b7e-104">Несколько сущностей в Microsoft Graph поддерживают [возобновляемую отправку файлов](/graph/api/driveitem-createuploadsession?view=graph-rest-1.0) , чтобы упростить отправку больших файлов.</span><span class="sxs-lookup"><span data-stu-id="80b7e-104">A number of entities in Microsoft Graph support [resumable file uploads](/graph/api/driveitem-createuploadsession?view=graph-rest-1.0) to make it easier to upload large files.</span></span> <span data-ttu-id="80b7e-105">Вместо того чтобы отправлять весь файл в отдельном запросе, файл разбивается на небольшие фрагменты, а запрос используется для отправки одного фрагмента.</span><span class="sxs-lookup"><span data-stu-id="80b7e-105">Instead of trying to upload the entire file in a single request, the file is sliced into smaller pieces and a request is used to upload a single slice.</span></span> <span data-ttu-id="80b7e-106">Чтобы упростить этот процесс, в пакет SDK Microsoft Graph внедрена задача по передаче больших файлов, которая управляет отправкой фрагментов.</span><span class="sxs-lookup"><span data-stu-id="80b7e-106">In order to simplify this process, the Microsoft Graph SDKs implement a large file upload task that manages the uploading of the slices.</span></span>

## <a name="c"></a>[<span data-ttu-id="80b7e-107">C#</span><span class="sxs-lookup"><span data-stu-id="80b7e-107">C#</span></span>](#tab/csharp)

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
    IProgress<long> progress = new Progress<long>(progress => {
        Console.WriteLine($"Uploaded {progress} bytes of {fileStream.Length} bytes");
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

## <a name="typescript"></a>[<span data-ttu-id="80b7e-108">TypeScript</span><span class="sxs-lookup"><span data-stu-id="80b7e-108">TypeScript</span></span>](#tab/typescript)

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

## <a name="java"></a>[<span data-ttu-id="80b7e-109">Java</span><span class="sxs-lookup"><span data-stu-id="80b7e-109">Java</span></span>](#tab/java)

```java
// Get an input stream for the file
InputStream fileStream = new FileInputStream(localFilePath);
long streamSize = (long)fileStream.available();

// Create a callback used by the upload provider
IProgressCallback<DriveItem> callback = new IProgressCallback<DriveItem>() {
    @Override
    // Called after each slice of the file is uploaded
    public void progress(final long current, final long max) {
        System.out.println(
            String.format("Uploaded %d bytes of %d total bytes", current, max)
        );
    }

    @Override
    public void success(final DriveItem result) {
        System.out.println(
            String.format("Uploaded file with ID: %s", result.id)
        );
    }

    public void failure(final ClientException ex) {
        System.out.println(
            String.format("Error uploading file: %s", ex.getMessage())
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

ChunkedUploadProvider<DriveItem> chunkedUploadProvider =
    new ChunkedUploadProvider<DriveItem>
        (uploadSession, graphClient, fileStream, streamSize, DriveItem.class);

// Config parameter is an array of integers
// customConfig[0] indicates the max slice size
// Max slice size must be a multiple of 320 KiB
int[] customConfig = { 320 * 1024 };

// Do the upload
chunkedUploadProvider.upload(callback, customConfig);
```

---

## <a name="resuming-a-file-upload"></a><span data-ttu-id="80b7e-110">Возобновление отправки файла</span><span class="sxs-lookup"><span data-stu-id="80b7e-110">Resuming a file upload</span></span>

<span data-ttu-id="80b7e-111">Пакеты SDK Microsoft Graph поддерживают [возобновление выполняемых отправок](/graph/api/driveitem-createuploadsession?view=graph-rest-1.0#resuming-an-in-progress-upload).</span><span class="sxs-lookup"><span data-stu-id="80b7e-111">The Microsoft Graph SDKs support [resuming in-progress uploads](/graph/api/driveitem-createuploadsession?view=graph-rest-1.0#resuming-an-in-progress-upload).</span></span> <span data-ttu-id="80b7e-112">Если во время отправки приложение обнаруживает прерывание подключения или состояние 5. x. x HTTP, можно возобновить отправку.</span><span class="sxs-lookup"><span data-stu-id="80b7e-112">If your application encounters a connection interruption or a 5.x.x HTTP status during upload, you can resume the upload.</span></span>

<!-- markdownlint-disable MD024 -->
### <a name="c"></a>[<span data-ttu-id="80b7e-113">C#</span><span class="sxs-lookup"><span data-stu-id="80b7e-113">C#</span></span>](#tab/csharp)

```csharp
fileUploadTask.ResumeAsync(progress);
```

### <a name="typescript"></a>[<span data-ttu-id="80b7e-114">TypeScript</span><span class="sxs-lookup"><span data-stu-id="80b7e-114">TypeScript</span></span>](#tab/typescript)

```typescript
const resumedFile: DriveItem = await uploadTask.resume();
```

### <a name="java"></a>[<span data-ttu-id="80b7e-115">Java</span><span class="sxs-lookup"><span data-stu-id="80b7e-115">Java</span></span>](#tab/java)

> [!NOTE]
> <span data-ttu-id="80b7e-116">В настоящее время пакет SDK Java не поддерживает восстановление выполняемой загрузки.</span><span class="sxs-lookup"><span data-stu-id="80b7e-116">The Java SDK does not currently support resuming in-progress downloads.</span></span>

---
<!-- markdownlint-enable MD024 -->
