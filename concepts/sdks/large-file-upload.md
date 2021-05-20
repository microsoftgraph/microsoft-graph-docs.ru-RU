---
title: Upload большие файлы с помощью Microsoft Graph SDKs
description: Предоставляет рекомендации по загрузке больших файлов с помощью microsoft Graph SDKs.
localization_priority: Normal
author: DarrelMiller
ms.openlocfilehash: b1a87c142f70f81b9e726727c6570f2cbce0f357
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579706"
---
# <a name="upload-large-files-using-the-microsoft-graph-sdks"></a><span data-ttu-id="25818-103">Upload большие файлы с помощью Microsoft Graph SDKs</span><span class="sxs-lookup"><span data-stu-id="25818-103">Upload large files using the Microsoft Graph SDKs</span></span>

<span data-ttu-id="25818-104">Ряд организаций в microsoft Graph возобновление [загрузки файлов, чтобы](/graph/api/driveitem-createuploadsession?view=graph-rest-1.0&preserve-view=true) облегчить загрузку больших файлов.</span><span class="sxs-lookup"><span data-stu-id="25818-104">A number of entities in Microsoft Graph support [resumable file uploads](/graph/api/driveitem-createuploadsession?view=graph-rest-1.0&preserve-view=true) to make it easier to upload large files.</span></span> <span data-ttu-id="25818-105">Вместо того, чтобы загружать весь файл в один запрос, файл нарезается на более мелкие части и запрос используется для загрузки одного среза.</span><span class="sxs-lookup"><span data-stu-id="25818-105">Instead of trying to upload the entire file in a single request, the file is sliced into smaller pieces and a request is used to upload a single slice.</span></span> <span data-ttu-id="25818-106">Чтобы упростить этот процесс, Microsoft Graph SDKs реализует большую задачу загрузки файлов, которая управляет загрузкой фрагментов.</span><span class="sxs-lookup"><span data-stu-id="25818-106">In order to simplify this process, the Microsoft Graph SDKs implement a large file upload task that manages the uploading of the slices.</span></span>

## <a name="c"></a>[<span data-ttu-id="25818-107">C#</span><span class="sxs-lookup"><span data-stu-id="25818-107">C#</span></span>](#tab/csharp)

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

## <a name="typescript"></a>[<span data-ttu-id="25818-108">TypeScript</span><span class="sxs-lookup"><span data-stu-id="25818-108">TypeScript</span></span>](#tab/typescript)

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

## <a name="java"></a>[<span data-ttu-id="25818-109">Java</span><span class="sxs-lookup"><span data-stu-id="25818-109">Java</span></span>](#tab/java)

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

## <a name="resuming-a-file-upload"></a><span data-ttu-id="25818-110">Возобновление загрузки файла</span><span class="sxs-lookup"><span data-stu-id="25818-110">Resuming a file upload</span></span>

<span data-ttu-id="25818-111">Microsoft Graph SDKs [поддержку возобновления в прогресс загрузки](/graph/api/driveitem-createuploadsession?view=graph-rest-1.0&preserve-view=true#resuming-an-in-progress-upload).</span><span class="sxs-lookup"><span data-stu-id="25818-111">The Microsoft Graph SDKs support [resuming in-progress uploads](/graph/api/driveitem-createuploadsession?view=graph-rest-1.0&preserve-view=true#resuming-an-in-progress-upload).</span></span> <span data-ttu-id="25818-112">Если во время загрузки у приложения произок перерыв в подключении или статус 5.x.x HTTP, вы можете возобновить загрузку.</span><span class="sxs-lookup"><span data-stu-id="25818-112">If your application encounters a connection interruption or a 5.x.x HTTP status during upload, you can resume the upload.</span></span>

<!-- markdownlint-disable MD024 -->
### <a name="c"></a>[<span data-ttu-id="25818-113">C#</span><span class="sxs-lookup"><span data-stu-id="25818-113">C#</span></span>](#tab/csharp)

```csharp
fileUploadTask.ResumeAsync(progress);
```

### <a name="typescript"></a>[<span data-ttu-id="25818-114">TypeScript</span><span class="sxs-lookup"><span data-stu-id="25818-114">TypeScript</span></span>](#tab/typescript)

```typescript
const resumedFile: DriveItem = await uploadTask.resume();
```

### <a name="java"></a>[<span data-ttu-id="25818-115">Java</span><span class="sxs-lookup"><span data-stu-id="25818-115">Java</span></span>](#tab/java)

> [!NOTE]
> <span data-ttu-id="25818-116">Java SDK в настоящее время не поддерживает возобновление загрузки в процессе.</span><span class="sxs-lookup"><span data-stu-id="25818-116">The Java SDK does not currently support resuming in-progress downloads.</span></span>

---
<!-- markdownlint-enable MD024 -->
