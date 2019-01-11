---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Возобновляемая отправка файлов
localization_priority: Normal
ms.openlocfilehash: c8ab45f9915b16f75e8b44ad50215c4e73c13fff
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27865182"
---
# <a name="upload-large-files-with-an-upload-session"></a><span data-ttu-id="32fe3-102">Отправка больших файлов с помощью сеанса отправки</span><span class="sxs-lookup"><span data-stu-id="32fe3-102">Upload large files with an upload session</span></span>

> <span data-ttu-id="32fe3-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="32fe3-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="32fe3-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32fe3-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="32fe3-p102">Создайте сеанс отправки, чтобы приложение могло отправлять файлы, размер которых не превышает максимальный. С помощью сеанса отправки приложение может отправлять диапазоны файла при последовательных запросах API, что позволяет возобновить передачу, если во время отправки соединение будет разорвано.</span><span class="sxs-lookup"><span data-stu-id="32fe3-p102">Create an upload session to allow your app to upload files up to the maximum file size. An upload session allows your app to upload ranges of the file in sequential API requests, which allows the transfer to be resumed if a connection is dropped while the upload is in progress.</span></span>

<span data-ttu-id="32fe3-107">Процесс отправки файла с помощью сеанса отправки состоит из двух этапов:</span><span class="sxs-lookup"><span data-stu-id="32fe3-107">To upload a file using an upload session, there are two steps:</span></span>

1. <span data-ttu-id="32fe3-108">[Создание сеанса отправки](#create-an-upload-session).</span><span class="sxs-lookup"><span data-stu-id="32fe3-108">[Create an upload session](#create-an-upload-session)</span></span>
2. <span data-ttu-id="32fe3-109">[Отправка байтов в сеанс отправки](#upload-bytes-to-the-upload-session).</span><span class="sxs-lookup"><span data-stu-id="32fe3-109">[Upload bytes to the upload session](#upload-bytes-to-the-upload-session)</span></span>

## <a name="permissions"></a><span data-ttu-id="32fe3-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="32fe3-110">Permissions</span></span>

<span data-ttu-id="32fe3-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32fe3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32fe3-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="32fe3-113">Permission type</span></span>      | <span data-ttu-id="32fe3-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="32fe3-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="32fe3-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="32fe3-115">Delegated (work or school account)</span></span> | <span data-ttu-id="32fe3-116">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32fe3-116">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="32fe3-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="32fe3-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32fe3-118">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32fe3-118">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="32fe3-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="32fe3-119">Application</span></span> | <span data-ttu-id="32fe3-120">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32fe3-120">Sites.ReadWrite.All</span></span> |

## <a name="create-an-upload-session"></a><span data-ttu-id="32fe3-121">Создание сеанса отправки</span><span class="sxs-lookup"><span data-stu-id="32fe3-121">Create an upload session</span></span>

<span data-ttu-id="32fe3-122">Для начала загрузки большого файла, ваше приложение должно первого запроса нового сеанса передачи.</span><span class="sxs-lookup"><span data-stu-id="32fe3-122">To begin a large file upload, your app must first request a new upload session.</span></span>
<span data-ttu-id="32fe3-123">В этом создается временная папка байт файла сохранения только после отправки файла завершена.</span><span class="sxs-lookup"><span data-stu-id="32fe3-123">This creates a temporary storage location where the bytes of the file will be saved until the complete file is uploaded.</span></span>
<span data-ttu-id="32fe3-124">После получения последнего байта файла будет отправлен окончания сеанса передачи и последний файл отображается в папке назначения.</span><span class="sxs-lookup"><span data-stu-id="32fe3-124">Once the last byte of the file has been uploaded the upload session is completed and the final file is shown in the destination folder.</span></span>
<span data-ttu-id="32fe3-125">Кроме того, можно отложить окончательный Создание файла в месте назначения до явным образом сделать запрос для завершения обновления, задав `deferCommit` свойство в аргументы запроса.</span><span class="sxs-lookup"><span data-stu-id="32fe3-125">Alternatively, you can defer final creation of the file in the destination until you explicitly make a request to complete the upload, by setting the `deferCommit` property in the request arguments.</span></span>

### <a name="http-request"></a><span data-ttu-id="32fe3-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="32fe3-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/createUploadSession
POST /groups/{groupId}/drive/items/{itemId}/createUploadSession
POST /me/drive/items/{itemId}/createUploadSession
POST /sites/{siteId}/drive/items/{itemId}/createUploadSession
POST /users/{userId}/drive/items/{itemId}/createUploadSession
```

### <a name="request-body"></a><span data-ttu-id="32fe3-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="32fe3-127">Request body</span></span>

<span data-ttu-id="32fe3-128">Тело запроса не требуется.</span><span class="sxs-lookup"><span data-stu-id="32fe3-128">No request body is required.</span></span>
<span data-ttu-id="32fe3-129">Тем не менее можно указать свойства в тексте запроса, предоставляя дополнительные данные о выгружаемого файла и настройка семантика операции отправки.</span><span class="sxs-lookup"><span data-stu-id="32fe3-129">However, you can specify properties in the request body providing additional data about the file being uploaded and customizing the semantics of the upload operation.</span></span>

<span data-ttu-id="32fe3-130">Например `item` свойство позволяет настройки следующих параметров:<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.driveItemUploadableProperties" } --></span><span class="sxs-lookup"><span data-stu-id="32fe3-130">For example, the `item` property allows setting the following parameters: <!-- { "blockType": "resource", "@odata.type": "microsoft.graph.driveItemUploadableProperties" } --></span></span>
```json
{
  "@microsoft.graph.conflictBehavior": "rename | fail | overwrite",
  "description": "description",
  "name": "filename.txt"
}
```

<span data-ttu-id="32fe3-131">Следующий пример управляет поведением уведомлений, если имя файла уже используется, а также указывает не создавать последний файл до явные завершения запроса:</span><span class="sxs-lookup"><span data-stu-id="32fe3-131">The following example controls the behavior if the filename is already taken, and also specifies that the final file should not be created until an explicit completion request is made:</span></span>

<!-- { "blockType": "ignored" } -->
```json
{
  "item": {
    "@microsoft.graph.conflictBehavior": "rename"
  },
  "deferCommit": true
}
```

### <a name="optional-request-headers"></a><span data-ttu-id="32fe3-132">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="32fe3-132">Optional request headers</span></span>

| <span data-ttu-id="32fe3-133">Имя</span><span class="sxs-lookup"><span data-stu-id="32fe3-133">Name</span></span>       | <span data-ttu-id="32fe3-134">Значение</span><span class="sxs-lookup"><span data-stu-id="32fe3-134">Value</span></span> | <span data-ttu-id="32fe3-135">Описание</span><span class="sxs-lookup"><span data-stu-id="32fe3-135">Description</span></span>                                                                                                                                                            |
|:-----------|:------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="32fe3-136">*if-match*</span><span class="sxs-lookup"><span data-stu-id="32fe3-136">*if-match*</span></span> | <span data-ttu-id="32fe3-137">etag</span><span class="sxs-lookup"><span data-stu-id="32fe3-137">etag</span></span>  | <span data-ttu-id="32fe3-138">Если указан заголовок запроса, а предоставленное значение eTag (или cTag) не совпадает с текущим значением eTag элемента, то возвращается ошибка `412 Precondition Failed`.</span><span class="sxs-lookup"><span data-stu-id="32fe3-138">If this request header is included and the eTag (or cTag) provided does not match the current etag on the item, a `412 Precondition Failed` error response is returned.</span></span> |

## <a name="parameters"></a><span data-ttu-id="32fe3-139">Параметры</span><span class="sxs-lookup"><span data-stu-id="32fe3-139">Parameters</span></span>

| <span data-ttu-id="32fe3-140">Параметр</span><span class="sxs-lookup"><span data-stu-id="32fe3-140">Parameter</span></span>            | <span data-ttu-id="32fe3-141">Тип</span><span class="sxs-lookup"><span data-stu-id="32fe3-141">Type</span></span>                          | <span data-ttu-id="32fe3-142">Описание</span><span class="sxs-lookup"><span data-stu-id="32fe3-142">Description</span></span>
|:---------------------|:------------------------------|:---------------------------------
| <span data-ttu-id="32fe3-143">item</span><span class="sxs-lookup"><span data-stu-id="32fe3-143">item</span></span>                 | <span data-ttu-id="32fe3-144">driveItemUploadableProperties</span><span class="sxs-lookup"><span data-stu-id="32fe3-144">driveItemUploadableProperties</span></span> | <span data-ttu-id="32fe3-145">Данные о выгружаемого файла</span><span class="sxs-lookup"><span data-stu-id="32fe3-145">Data about the file being uploaded</span></span>
| <span data-ttu-id="32fe3-146">deferCommit</span><span class="sxs-lookup"><span data-stu-id="32fe3-146">deferCommit</span></span>          | <span data-ttu-id="32fe3-147">Логический</span><span class="sxs-lookup"><span data-stu-id="32fe3-147">Boolean</span></span>                       | <span data-ttu-id="32fe3-148">Если параметр имеет значение true, окончательный Создание файла в месте назначения будут требуют явного запроса.</span><span class="sxs-lookup"><span data-stu-id="32fe3-148">If set to true, final creation of the file in the destination will require an explicit request.</span></span> <span data-ttu-id="32fe3-149">Только на OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="32fe3-149">Only on OneDrive for Business.</span></span>

## <a name="item-properties"></a><span data-ttu-id="32fe3-150">Свойства элемента</span><span class="sxs-lookup"><span data-stu-id="32fe3-150">Item properties</span></span>

| <span data-ttu-id="32fe3-151">Свойство</span><span class="sxs-lookup"><span data-stu-id="32fe3-151">Property</span></span>             | <span data-ttu-id="32fe3-152">Тип</span><span class="sxs-lookup"><span data-stu-id="32fe3-152">Type</span></span>               | <span data-ttu-id="32fe3-153">Описание</span><span class="sxs-lookup"><span data-stu-id="32fe3-153">Description</span></span>
|:---------------------|:-------------------|:---------------------------------
| <span data-ttu-id="32fe3-154">описание</span><span class="sxs-lookup"><span data-stu-id="32fe3-154">description</span></span>          | <span data-ttu-id="32fe3-155">Строка</span><span class="sxs-lookup"><span data-stu-id="32fe3-155">String</span></span>             | <span data-ttu-id="32fe3-156">Предоставляет видимыми описание элемента.</span><span class="sxs-lookup"><span data-stu-id="32fe3-156">Provides a user-visible description of the item.</span></span> <span data-ttu-id="32fe3-157">Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="32fe3-157">Read-write.</span></span> <span data-ttu-id="32fe3-158">Только на личные OneDrive.</span><span class="sxs-lookup"><span data-stu-id="32fe3-158">Only on OneDrive Personal.</span></span>
| <span data-ttu-id="32fe3-159">name</span><span class="sxs-lookup"><span data-stu-id="32fe3-159">name</span></span>                 | <span data-ttu-id="32fe3-160">Строка</span><span class="sxs-lookup"><span data-stu-id="32fe3-160">String</span></span>             | <span data-ttu-id="32fe3-p108">Имя элемента (имя и расширение файла). Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="32fe3-p108">The name of the item (filename and extension). Read-write.</span></span>

### <a name="request"></a><span data-ttu-id="32fe3-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="32fe3-163">Request</span></span>

<span data-ttu-id="32fe3-164">В отклике на этот запрос будут представлены подробные сведения о новом экземпляре [uploadSession](../resources/uploadsession.md) (в том числе URL-адрес для отправки фрагментов файла).</span><span class="sxs-lookup"><span data-stu-id="32fe3-164">The response to this request will provide the details of the newly created [uploadSession](../resources/uploadsession.md), which includes the URL used for uploading the parts of the file.</span></span> 

<!-- { "blockType": "request", "name": "upload-fragment-create-session", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drive/root:/{item-path}:/createUploadSession
Content-Type: application/json

{
  "item": {
    "@odata.type": "microsoft.graph.driveItemUploadableProperties",
    "@microsoft.graph.conflictBehavior": "rename",
    "name": "largefile.dat"
  }
}
```

### <a name="response"></a><span data-ttu-id="32fe3-165">Ответ</span><span class="sxs-lookup"><span data-stu-id="32fe3-165">Response</span></span>

<span data-ttu-id="32fe3-166">В случае успешного выполнения запроса ответ будет содержать сведения о том, куда отправлять остальные запросы (в виде ресурса [UploadSession](../resources/uploadsession.md)).</span><span class="sxs-lookup"><span data-stu-id="32fe3-166">The response to this request, if successful, will provide the details for where the remainder of the requests should be sent as an [UploadSession](../resources/uploadsession.md) resource.</span></span>

<span data-ttu-id="32fe3-167">Этот ресурс предоставляет сведения о том, куда следует отправлять диапазон байтов файла и когда истекает срок действия сеанса отправки.</span><span class="sxs-lookup"><span data-stu-id="32fe3-167">This resource provides details about where the byte range of the file should be uploaded and when the upload session expires.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession",
       "optionalProperties": [ "nextExpectedRanges" ]  } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "uploadUrl": "https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337",
  "expirationDateTime": "2015-01-29T09:21:55.523Z"
}
```

## <a name="upload-bytes-to-the-upload-session"></a><span data-ttu-id="32fe3-168">Отправка байтов в сеанс отправки</span><span class="sxs-lookup"><span data-stu-id="32fe3-168">Upload bytes to the upload session</span></span>

<span data-ttu-id="32fe3-169">Чтобы отправить файл или его часть, приложение выполняет запрос PUT на адрес **uploadUrl**, указанный в отклике для **createUploadSession**.</span><span class="sxs-lookup"><span data-stu-id="32fe3-169">To upload the file, or a portion of the file, your app makes a PUT request to the **uploadUrl** value received in the **createUploadSession** response.</span></span>
<span data-ttu-id="32fe3-170">Вы можете отправить файл целиком или разделить его на несколько диапазонов байтов. При этом каждый запрос должен содержать фрагмент размером не более 60 МБ.</span><span class="sxs-lookup"><span data-stu-id="32fe3-170">You can upload the entire file, or split the file into multiple byte ranges, as long as the maximum bytes in any given request is less than 60 MiB.</span></span>

<span data-ttu-id="32fe3-171">Фрагменты файл должен загружаться последовательно в порядке.</span><span class="sxs-lookup"><span data-stu-id="32fe3-171">The fragments of the file must be uploaded sequentially in order.</span></span>
<span data-ttu-id="32fe3-172">В противном случае возникнет ошибка.</span><span class="sxs-lookup"><span data-stu-id="32fe3-172">Uploading fragments out of order will result in an error.</span></span>

<span data-ttu-id="32fe3-173">**Примечание.** Если приложение делит файл на несколько диапазонов байтов, размер каждого из них **ДОЛЖЕН** быть кратным 320 КБ (327 680 байтов).</span><span class="sxs-lookup"><span data-stu-id="32fe3-173">**Note:** If your app splits a file into multiple byte ranges, the size of each byte range **MUST** be a multiple of 320 KiB (327,680 bytes).</span></span> <span data-ttu-id="32fe3-174">Если размер фрагментов не делится на 320 КБ без остатка, при отправке некоторых файлов возникнут ошибки.</span><span class="sxs-lookup"><span data-stu-id="32fe3-174">Using a fragment size that does not divide evenly by 320 KiB will result in errors committing some files.</span></span>

### <a name="example"></a><span data-ttu-id="32fe3-175">Пример</span><span class="sxs-lookup"><span data-stu-id="32fe3-175">Example</span></span>

<span data-ttu-id="32fe3-176">В этом примере приложение отправляет первые 26 из 128 байтов файла.</span><span class="sxs-lookup"><span data-stu-id="32fe3-176">In this example, the app is uploading the first 26 bytes of a 128 byte file.</span></span>

* <span data-ttu-id="32fe3-177">Заголовок **Content-Length** задает размер текущего запроса.</span><span class="sxs-lookup"><span data-stu-id="32fe3-177">The **Content-Length** header specifies the size of the current request.</span></span>
* <span data-ttu-id="32fe3-178">Заголовок **Content-Range** указывает диапазон (в байтах) для всего файла, представленного в запросе.</span><span class="sxs-lookup"><span data-stu-id="32fe3-178">The **Content-Range** header indicates the range of bytes in the overall file that this request represents.</span></span>
* <span data-ttu-id="32fe3-179">Прежде чем отправлять первый фрагмент файла, необходимо знать общий размер этого файла.</span><span class="sxs-lookup"><span data-stu-id="32fe3-179">The total length of the file is known before you can upload the first fragment of the file.</span></span>

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-piece", "scopes": "files.readwrite" } -->

```http
PUT https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337
Content-Length: 26
Content-Range: bytes 0-25/128

<bytes 0-25 of the file>
```

<span data-ttu-id="32fe3-180">**Важно!** Приложение должно указывать в заголовках **Content-Range** всех запросов один и тот же общий размер файла.</span><span class="sxs-lookup"><span data-stu-id="32fe3-180">**Important:** Your app must ensure the total file size specified in the **Content-Range** header is the same for all requests.</span></span>
<span data-ttu-id="32fe3-181">Если объявить для диапазона байтов другой размер файла, запрос не будет выполнен.</span><span class="sxs-lookup"><span data-stu-id="32fe3-181">If a byte range declares a different file size, the request will fail.</span></span>

### <a name="response"></a><span data-ttu-id="32fe3-182">Ответ</span><span class="sxs-lookup"><span data-stu-id="32fe3-182">Response</span></span>

<span data-ttu-id="32fe3-183">После выполнения запроса сервер отправит в ответ код `202 Accepted`, если требуется отправить дополнительные диапазоны байтов.</span><span class="sxs-lookup"><span data-stu-id="32fe3-183">When the request is complete, the server will respond with `202 Accepted` if there are more byte ranges that need to be uploaded.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->

```http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["26-"]
}
```

<span data-ttu-id="32fe3-184">С помощью значения **nextExpectedRanges** приложение может определить, где должен начинаться следующий диапазон байтов.</span><span class="sxs-lookup"><span data-stu-id="32fe3-184">Your app can use the **nextExpectedRanges** value to determine where to start the next byte range.</span></span>
<span data-ttu-id="32fe3-185">Вы можете увидеть несколько диапазонов, указывающих части файла, еще не полученные сервером.</span><span class="sxs-lookup"><span data-stu-id="32fe3-185">You may see multiple ranges specified, indicating parts of the file that the server has not yet received.</span></span> <span data-ttu-id="32fe3-186">Это удобно, когда требуется возобновить прерванную передачу, а клиенту неизвестно состояние службы.</span><span class="sxs-lookup"><span data-stu-id="32fe3-186">This is useful if you need to resume a transfer that was interrupted and your client is unsure of the state on the service.</span></span>

<span data-ttu-id="32fe3-187">Размер диапазонов байтов всегда следует определять в соответствии с приведенными ниже рекомендациями.</span><span class="sxs-lookup"><span data-stu-id="32fe3-187">You should always determine the size of your byte ranges according to the best practices below.</span></span> <span data-ttu-id="32fe3-188">Не рассчитывайте на то, что свойство **nextExpectedRanges** вернет диапазоны надлежащего размера для отправляемого диапазона байтов.</span><span class="sxs-lookup"><span data-stu-id="32fe3-188">Do not assume that **nextExpectedRanges** will return reanges of proper size for a byte range to upload.</span></span>
<span data-ttu-id="32fe3-189">Свойство **nextExpectedRanges** указывает диапазоны файла, которые не были получены, а не схему отправки файла приложением.</span><span class="sxs-lookup"><span data-stu-id="32fe3-189">The **nextExpectedRanges** property indicates ranges of the file that have not been received and not a pattern for how your app should upload the file.</span></span>

<!-- { "blockType": "ignored", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->

```http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": [
  "12345-55232",
  "77829-99375"
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="32fe3-190">Примечания</span><span class="sxs-lookup"><span data-stu-id="32fe3-190">Remarks</span></span>

* <span data-ttu-id="32fe3-191">В свойстве `nextExpectedRanges` не всегда указываются все отсутствующие диапазоны.</span><span class="sxs-lookup"><span data-stu-id="32fe3-191">The `nextExpectedRanges` property won't always list all of the missing ranges.</span></span>
* <span data-ttu-id="32fe3-p115">При успешной записи фрагментов оно возвращает следующий диапазон (например, "523-").</span><span class="sxs-lookup"><span data-stu-id="32fe3-p115">On successful fragment writes, it will return the next range to start from (eg. "523-").</span></span>
* <span data-ttu-id="32fe3-p116">При сбоях в тех случаях, когда клиент отправляет файл, уже полученный сервером, сервер возвращает отклик `HTTP 416 Requested Range Not Satisfiable`. Вы можете [запросить состояние отправки](#resuming-an-in-progress-upload), чтобы получить более подробный список недостающих диапазонов.</span><span class="sxs-lookup"><span data-stu-id="32fe3-p116">On failures when the client sent a fragment the server had already received, the server will respond with `HTTP 416 Requested Range Not Satisfiable`. You can [request upload status](#resuming-an-in-progress-upload) to get a more detailed list of missing ranges.</span></span>
* <span data-ttu-id="32fe3-p117">Как отклик на добавление заголовка авторизации при совершении вызова `PUT` может появиться сообщение об ошибке `HTTP 401 Unauthorized`. Заголовок авторизации и токен носителя необходимо отправлять только при выполнении `POST` на начальном этапе. Не следует включать их, когда совершается вызов `PUT`.</span><span class="sxs-lookup"><span data-stu-id="32fe3-p117">Including the Authorization header when issuing the `PUT` call may result in a `HTTP 401 Unauthorized` response. The Authorization header and bearer token should only be sent when issuing the `POST` during the first step. It should be not be included when issueing the `PUT`.</span></span>

## <a name="completing-a-file"></a><span data-ttu-id="32fe3-199">Завершение отправки файла</span><span class="sxs-lookup"><span data-stu-id="32fe3-199">Completing a file</span></span>

<span data-ttu-id="32fe3-200">Если `deferCommit` — значение false или удалить, а затем загрузка выполняется автоматически при диапазона окончательный байтов файла находится в состоянии загрузки URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="32fe3-200">If `deferCommit` is false or unset, then the upload is automatically completed when the final byte range of the file is PUT to the upload URL.</span></span>
<span data-ttu-id="32fe3-201">Если `deferCommit` имеет значение true, а затем после диапазона окончательный байтов файла находится в состоянии загрузки URL-адрес, передача должна быть явно выполнена окончательный запрос POST для передачи URL-адрес с нулевой длины содержимого.</span><span class="sxs-lookup"><span data-stu-id="32fe3-201">If `deferCommit` is true, then after the final byte range of the file is PUT to the upload URL, the upload should be explicitly completed by a final POST request to the upload url with zero-length content.</span></span>

<span data-ttu-id="32fe3-202">После завершения загрузки сервер будет отвечать на последнем запроса с `HTTP 201 Created` или `HTTP 200 OK`.</span><span class="sxs-lookup"><span data-stu-id="32fe3-202">When the upload is completed, the server will respond to the final request with an `HTTP 201 Created` or `HTTP 200 OK`.</span></span>
<span data-ttu-id="32fe3-203">Тело отклика также включает набор свойств по умолчанию для ресурса **driveItem**, представляющего полностью отправленный файл.</span><span class="sxs-lookup"><span data-stu-id="32fe3-203">The response body will also include the default property set for the **driveItem** representing the completed file.</span></span>

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-final", "scopes": "files.readwrite" } -->

```
PUT https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337
Content-Length: 21
Content-Range: bytes 101-127/128

<final bytes of the file>
```

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "912310013A123",
  "name": "largefile.vhd",
  "size": 128,
  "file": { }
}
```


<!-- { "blockType": "request", "opaqueUrl": true, "name": "commit-upload", "scopes": "files.readwrite" } -->

```
POST https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337
Content-Length: 0
```

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "912310013A123",
  "name": "largefile.vhd",
  "size": 128,
  "file": { }
}
```

## <a name="handling-upload-conflicts"></a><span data-ttu-id="32fe3-204">Обработка конфликтов при отправке</span><span class="sxs-lookup"><span data-stu-id="32fe3-204">Handling upload conflicts</span></span>

<span data-ttu-id="32fe3-205">В случае возникновения конфликта после отправки файла (например, если в ходе сеанса отправки был создан элемент с таким же именем) при отправке последнего диапазона байтов возвращается ошибка.</span><span class="sxs-lookup"><span data-stu-id="32fe3-205">If a conflict occurs after the file is uploaded (for example, an item with the same name was created during the upload session), an error is returned when the last byte range is uploaded.</span></span>

```http
HTTP/1.1 409 Conflict
Content-Type: application/json

{
  "error":
  {
    "code": "upload_name_conflict",
    "message": "Another file exists with the same name as the uploaded session. You can redirect the upload session to use a new filename by calling PUT with the new metadata and @microsoft.graph.sourceUrl attribute.",
  }
}
```

## <a name="cancel-the-upload-session"></a><span data-ttu-id="32fe3-206">Отмена сеанса отправки</span><span class="sxs-lookup"><span data-stu-id="32fe3-206">Cancel the upload session</span></span>

<span data-ttu-id="32fe3-p120">Чтобы отменить сеанс отправки, отправьте запрос DELETE на URL-адрес отправки. При этом очищается временный файл, содержащий ранее отправленные данные. Это следует делать в тех случаях, когда отправка прерывается (например, если пользователь отменил передачу).</span><span class="sxs-lookup"><span data-stu-id="32fe3-p120">To cancel an upload session send a DELETE request to the upload URL. This cleans up the temporary file holding the data previously uploaded. This should be used in scenarios where the upload is aborted, for example, if the user cancels the transfer.</span></span>

<span data-ttu-id="32fe3-210">Временные файлы и соответствующий сеанс отправки автоматически очищаются по прошествии времени, указанного свойством **expirationDateTime**.</span><span class="sxs-lookup"><span data-stu-id="32fe3-210">Temporary files and their accompanying upload session are automatically cleaned up after the **expirationDateTime** has passed.</span></span>
<span data-ttu-id="32fe3-211">Временные файлы могут быть удалены не сразу по истечении срока действия.</span><span class="sxs-lookup"><span data-stu-id="32fe3-211">Temporary files may not be deleted immedately after the expiration time has elapsed.</span></span>

### <a name="request"></a><span data-ttu-id="32fe3-212">Запрос</span><span class="sxs-lookup"><span data-stu-id="32fe3-212">Request</span></span>

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-cancel", "scopes": "files.readwrite" } -->

```http
DELETE https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337
```

### <a name="response"></a><span data-ttu-id="32fe3-213">Ответ</span><span class="sxs-lookup"><span data-stu-id="32fe3-213">Response</span></span>

<span data-ttu-id="32fe3-214">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="32fe3-214">The following example shows the response.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

## <a name="resuming-an-in-progress-upload"></a><span data-ttu-id="32fe3-215">Возобновление выполняемой отправки</span><span class="sxs-lookup"><span data-stu-id="32fe3-215">Resuming an in-progress upload</span></span>

<span data-ttu-id="32fe3-p122">При отключении или сбое отправки до полного выполнения запроса все байты в этом запросе игнорируются. Это может произойти при разрыве соединения между приложением и службой. В этом случае приложение может возобновить передачу файла с ранее отправленного фрагмента.</span><span class="sxs-lookup"><span data-stu-id="32fe3-p122">If an upload request is disconnected or fails before the request is completed, all bytes in that request are ignored. This can occur if the connection between your app and the service is dropped. If this occurs, your app can still resume the file transfer from the previously completed fragment.</span></span>

<span data-ttu-id="32fe3-219">Чтобы узнать, какие диапазоны байтов были получены ранее, приложение может запросить состояние сеанса отправки.</span><span class="sxs-lookup"><span data-stu-id="32fe3-219">To find out which byte ranges have been received previously, your app can request the status of an upload session.</span></span>

### <a name="example"></a><span data-ttu-id="32fe3-220">Пример</span><span class="sxs-lookup"><span data-stu-id="32fe3-220">Example</span></span>

<span data-ttu-id="32fe3-221">Получить состояние отправки можно, отправив запрос GET на адрес `uploadUrl`.</span><span class="sxs-lookup"><span data-stu-id="32fe3-221">Query the status of the upload by sending a GET request to the `uploadUrl`.</span></span>

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-resume", "scopes": "files.readwrite" } -->

```
GET https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF86633784148bb98a1zjcUhf7b0mpUadahs
```

<span data-ttu-id="32fe3-222">В ответ сервер отправит список отсутствующих байтовых диапазонов, которые требуется отправить, и время окончания срока действия для сеанса отправки.</span><span class="sxs-lookup"><span data-stu-id="32fe3-222">The server will respond with a list of missing byte ranges that need to be uploaded and the expiration time for the upload session.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["12345-"]
}
```

### <a name="upload-remaining-data"></a><span data-ttu-id="32fe3-223">Отправка оставшихся данных</span><span class="sxs-lookup"><span data-stu-id="32fe3-223">Upload remaining data</span></span>

<span data-ttu-id="32fe3-224">Теперь, когда приложению известно, с какого момента начинать отправку, возобновите операцию, выполнив действия из раздела [Отправка байтов в сеанс отправки](#upload-bytes-to-the-upload-session).</span><span class="sxs-lookup"><span data-stu-id="32fe3-224">Now that your app knows where to start the upload from, resume the upload by following the steps in [upload bytes to the upload session](#upload-bytes-to-the-upload-session).</span></span>

## <a name="handle-upload-errors"></a><span data-ttu-id="32fe3-225">Обработка ошибок отправки</span><span class="sxs-lookup"><span data-stu-id="32fe3-225">Handle upload errors</span></span>

<span data-ttu-id="32fe3-226">После отправки последнего диапазона байтов файла может возникнуть ошибка.</span><span class="sxs-lookup"><span data-stu-id="32fe3-226">When the last byte range of a file is uploaded, it is possible for an error to occur.</span></span> <span data-ttu-id="32fe3-227">Она может быть вызвана конфликтом имен или превышением ограничения квоты.</span><span class="sxs-lookup"><span data-stu-id="32fe3-227">This can be due to a name conflict or quota limitation being exceeded.</span></span>
<span data-ttu-id="32fe3-228">Сеанс отправки будет сохранен до истечения срока его действия. Это позволяет приложению возобновить отправку, явно зафиксировав сеанс отправки.</span><span class="sxs-lookup"><span data-stu-id="32fe3-228">The upload session will be preserved until the expiration time, which allows your app to recover the upload by explicitly committing the upload session.</span></span>

<span data-ttu-id="32fe3-229">Для этого приложение должно отправить запрос PUT с новым ресурсом **driveItem**, который будет использоваться при фиксации сеанса отправки.</span><span class="sxs-lookup"><span data-stu-id="32fe3-229">To explicitly commit the upload session, your app must make a PUT request with a new **driveItem** resource that will be used when committing the upload session.</span></span>
<span data-ttu-id="32fe3-230">Этот новый запрос должен устранить причину первоначальной ошибки отправки.</span><span class="sxs-lookup"><span data-stu-id="32fe3-230">This new request should correct the source of error that generated the original upload error.</span></span>

<span data-ttu-id="32fe3-231">Чтобы указать, что приложение применяет существующий сеанс отправки, запрос PUT должен включать свойство `@microsoft.graph.sourceUrl` со значением URL-адреса сеанса отправки.</span><span class="sxs-lookup"><span data-stu-id="32fe3-231">To indicate that your app is committing an existing upload session, the PUT request must include the `@microsoft.graph.sourceUrl` property with the value of your upload session URL.</span></span>

<!-- { "blockType": "ignored", "name": "explicit-upload-commit", "scopes": "files.readwrite", "tags": "service.graph" } -->

```http
PUT /me/drive/root:/{path_to_parent}
Content-Type: application/json
If-Match: {etag or ctag}

{
  "name": "largefile.vhd",
  "@microsoft.graph.conflictBehavior": "rename",
  "@microsoft.graph.sourceUrl": "{upload session URL}"
}
```

<span data-ttu-id="32fe3-232">**Примечание.** В этом вызове можно использовать заголовки `@microsoft.graph.conflictBehavior` и `if-match` надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="32fe3-232">**Note:** You can use the `@microsoft.graph.conflictBehavior` and `if-match` headers as expected in this call.</span></span>

### <a name="response"></a><span data-ttu-id="32fe3-233">Ответ</span><span class="sxs-lookup"><span data-stu-id="32fe3-233">Response</span></span>

<span data-ttu-id="32fe3-234">Если файл можно зафиксировать с помощью новых метаданных, возвращается ответ `HTTP 201 Created` или `HTTP 200 OK` с метаданными ресурса Item для отправленного файла.</span><span class="sxs-lookup"><span data-stu-id="32fe3-234">If the file can be committed using the new metadata, an `HTTP 201 Created` or `HTTP 200 OK` response will be returned with the Item metadata for the uploaded file.</span></span>

<!-- { "blockType": "ignored", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "912310013A123",
  "name": "largefile.vhd",
  "size": 128,
  "file": { }
}
```

## <a name="best-practices"></a><span data-ttu-id="32fe3-235">Рекомендации</span><span class="sxs-lookup"><span data-stu-id="32fe3-235">Best practices</span></span>

* <span data-ttu-id="32fe3-236">Возобновляйте или повторно запускайте операции отправки, не выполненные из-за разрывов соединения или каких-либо ошибок с кодом 5xx, в том числе:</span><span class="sxs-lookup"><span data-stu-id="32fe3-236">Resume or retry uploads that fail due to connection interruptions or any 5xx errors, including:</span></span>
  * `500 Internal Server Error`
  * `502 Bad Gateway`
  * `503 Service Unavailable`
  * `504 Gateway Timeout`
* <span data-ttu-id="32fe3-237">Используйте стратегию экспоненциального откладывания, если при возобновлении или повторной отправке возвращаются ошибки сервера с кодом 5xx.</span><span class="sxs-lookup"><span data-stu-id="32fe3-237">Use an exponential back off strategy if any 5xx server errors are returned when resuming or retrying upload requests.</span></span>
* <span data-ttu-id="32fe3-238">При возникновении других ошибок не следует использовать эту стратегию. Вместо этого ограничьте количество повторных попыток.</span><span class="sxs-lookup"><span data-stu-id="32fe3-238">For other errors, you should not use an exponential back off strategy but limit the number of retry attempts made.</span></span>
* <span data-ttu-id="32fe3-239">Для устранения ошибок `404 Not Found` при возобновляемой отправке начинайте всю отправку заново.</span><span class="sxs-lookup"><span data-stu-id="32fe3-239">Handle `404 Not Found` errors when doing resumable uploads by starting the entire upload over.</span></span> <span data-ttu-id="32fe3-240">Это означает, что сеанс отправки больше не существует.</span><span class="sxs-lookup"><span data-stu-id="32fe3-240">This indicates the upload session no longer exists.</span></span>
* <span data-ttu-id="32fe3-241">Используйте возобновляемую отправку для файлов размером более 10 МБ (10 485 760 байтов).</span><span class="sxs-lookup"><span data-stu-id="32fe3-241">Use resumable file transfers for files larger than 10 MiB (10,485,760 bytes).</span></span>
* <span data-ttu-id="32fe3-242">Размер 10 МБ для диапазона байтов оптимален в случае стабильных высокоскоростных подключений.</span><span class="sxs-lookup"><span data-stu-id="32fe3-242">A byte range size of 10 MiB for stable high speed connections is optimal.</span></span> <span data-ttu-id="32fe3-243">Если используется более медленное или менее надежное подключение, то вы можете получить оптимальные результаты, используя фрагменты меньшего размера.</span><span class="sxs-lookup"><span data-stu-id="32fe3-243">For slower or less reliable connections you may get better results from a smaller fragment size.</span></span> <span data-ttu-id="32fe3-244">Рекомендуем использовать фрагменты размером 5–10 МБ.</span><span class="sxs-lookup"><span data-stu-id="32fe3-244">The recommended fragment size is between 5-10 MiB.</span></span>
* <span data-ttu-id="32fe3-245">Используйте размер фрагментов, кратный 320 КБ (327 680 байтов).</span><span class="sxs-lookup"><span data-stu-id="32fe3-245">Use a byte range size that is a multiple of 320 KiB (327,680 bytes).</span></span> <span data-ttu-id="32fe3-246">В противном случае после отправки последнего диапазона байтов большого файла может произойти сбой.</span><span class="sxs-lookup"><span data-stu-id="32fe3-246">Failing to use a fragment size that is a multiple of 320 KiB can result in large file transfers failing after the last byte range is uploaded.</span></span>

## <a name="error-responses"></a><span data-ttu-id="32fe3-247">Ответы с ошибками</span><span class="sxs-lookup"><span data-stu-id="32fe3-247">Error responses</span></span>

<span data-ttu-id="32fe3-248">Дополнительные сведения о том как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="32fe3-248">See the [Error Responses][error-response] topic for details about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Upload large files using an upload session.",
  "keywords": "upload,large file,fragment,BITS",
  "section": "documentation"
} -->
