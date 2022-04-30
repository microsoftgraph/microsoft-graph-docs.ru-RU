---
title: Отправка документов с помощью API универсальной печати Microsoft Graph
description: Представляем универсальную печать — современное решение печати, которое можно использовать в организациях для управления инфраструктурой печати через облачные службы Майкрософт.
author: nilakhan
ms.localizationpriority: high
ms.custom: scenarios:getting-started
ms.openlocfilehash: 36dd113e02e15822f9a64b04da390d5a87cae867
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2022
ms.locfileid: "65133106"
---
# <a name="upload-documents-using-the-microsoft-graph-universal-print-api"></a>Отправка документов с помощью API универсальной печати Microsoft Graph

Чтобы напечатать документ с помощью API универсальной печати в Microsoft Graph, [создайте задание печати](/graph/api/printershare-post-jobs), отправьте документ и [запустите задание печати](/graph/api/printjob-start). В этой статье описано, как отправить документ, начиная с [создания сеанса отправки](/graph/api/printdocument-createuploadsession).

Чтобы отправить файл или его часть, приложение выполняет запрос PUT на адрес **uploadUrl**, указанный в отклике для **createUploadSession**. Вы можете отправить файл целиком или разделить его на фрагменты. При этом каждый запрос должен содержать фрагмент размером не более 10 МБ.

Сегменты файла можно отправлять в любом порядке, в том числе параллельно (до четырех параллельных запросов). После отправки всех двоичных сегментов документа двоичный файл связывается с **printDocument**.

## <a name="http-request"></a>HTTP-запрос

Отправьте запрос PUT на адрес **uploadUrl**, указанный в ответе для **createUploadSession**.

### <a name="request-headers"></a>Заголовки запросов
| Имя          | Описание   |
|:--------------|:--------------|
| Content-Range | Диапазон байтов: {startByteIndex}-{endByteIndex}‬/{documentSizeInBytes}. Обязательно.|
| Content-Length | {contentLength}‬ обязательно.|

### <a name="request-body"></a>Текст запроса
Текст запроса — это большой двоичный объект, содержащий байты документа, указанные как **инклюзивный** диапазон байтов, в заголовке `Content-Range`. 

### <a name="example"></a>Пример

```http
PUT https://print.print.microsoft.com/uploadSessions/5400be13-5a4e-4c20-be70-90c85bfe5d6e?tempauthtoken={token}
Content-Range: bytes=0-72796/4533322
Content-Length: 72797

<bytes 0-72796 of the file>

```

Здесь 0 и 72796 — это индексы начала и окончания сегмента файла, а 4533322 — размер документа.
## <a name="http-response"></a>HTTP-ответ

После выполнения запроса сервер отправит в ответ код `202 Accepted`, если требуется отправить дополнительные диапазоны байтов.

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->

```http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
  "expirationDateTime": "2020-10-25T02:19:38.1694207Z",
  "nextExpectedRanges": ["72797-4533321"]
}
```

С помощью значения **nextExpectedRanges** приложение может определить, где должен начинаться следующий диапазон байтов. Вы можете увидеть несколько диапазонов, указывающих части файла, еще не полученные сервером. Свойство **nextExpectedRanges** указывает диапазоны файла, которые не были получены, а не схему отправки файла приложением.

<!-- { "blockType": "ignored", "@odata.type": "microsoft.graph.uploadSession", "truncated": true } -->

```http
HTTP/1.1 202 Accepted
Content-Type: application/json

{
  "expirationDateTime": "2020-10-25T02:19:38.1694207Z",
  "nextExpectedRanges": [
  "72797-72897",
  "78929-4533322"
  ]
}
```

### <a name="remarks"></a>Примечания

* При сбоях в тех случаях, когда клиент отправляет файл, уже полученный сервером, сервер возвращает отклик `HTTP 416 Requested Range Not Satisfiable`. Вы можете [запросить состояние отправки](#get-the-upload-session), чтобы получить более подробный список недостающих диапазонов.
* Включение заголовка `Authorizatio`n при вызове `PUT` может привести к ответу `HTTP 401 Unauthorized`. Заголовок авторизации и маркер носителя необходимо отправлять только при создании сеанса отправки. Их не следует включать при отправке данных для сеанса отправки.

## <a name="completing-a-file"></a>Завершение отправки файла

После получения последнего диапазона байтов файла сервер отправляет ответ `HTTP 201 Created`. Текст ответа также будет включать набор свойств для связанного **printDocument**.

### <a name="request"></a>Запрос
<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-final", "scopes": "printjob.readwrite" } -->
```http
PUT https://print.print.microsoft.com/uploadSessions/5400be13-5a4e-4c20-be70-90c85bfe5d6e?tempauthtoken={token}
Content-Length: 10
Content-Range: bytes 4533312-4533321/4533322

<final bytes of the file>
```

### <a name="response"></a>Отклик
<!-- { "blockType": "response", "@odata.type": "microsoft.graph.printDocument", "truncated": true } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
   "id": "9001bcd9-e36a-4f51-bfc6-140c3ad7f9f7",
   "documentName": "TestFile.pdf",
   "contentType": "application/pdf", 
   "size": 4533322
}
```

>**Примечание.** Сеанс отправки удаляется после завершения отправки документов.

## <a name="get-the-upload-session"></a>Получение сеанса отправки

Чтобы получить сеанс отправки, отправьте запрос GET на URL-адрес отправки. 

### <a name="request"></a>Запрос
<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-resume", "scopes": "files.readwrite" } -->

```http
GET https://print.print.microsoft.com/uploadSessions/5400be13-5a4e-4c20-be70-90c85bfe5d6e?tempauthtoken={token}
```

### <a name="response"></a>Отклик

<!-- { "blockType": "response" } -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "expirationDateTime": "2020-10-25T02:19:38.1694207Z",
  "nextExpectedRanges": [
  "72797-72897",
  "78929-4533322"
  ]
}
```
## <a name="code-examples-create-upload-session-and-upload-documents"></a>Примеры кода: создание сеанса отправки и отправка документов
 
# <a name="c"></a>[C#](#tab/csharp)

```csharp

            GraphServiceClient graphClient = new GraphServiceClient( authProvider );

            var properties = new PrintDocumentUploadProperties
            {
                DocumentName = "TestFile.pdf",
                ContentType = "application/pdf",
                Size = 4533322
            };

            var uploadSession = await graphClient.Print.Printers["{printer-id}"].Jobs["{printJob-id}"].Documents["{printDocument-id}"]
                .CreateUploadSession(properties)
                .Request()
                .PostAsync()

            // if using Graph SDK, maxSliceSize should in multiples of 320 KiB
            int maxSliceSize = 320 * 1024;
            var fileUploadTask =
                new LargeFileUploadTask<PrintDocument>(uploadSession, fileStream, maxSliceSize);

            // Create a callback that is invoked after each slice is uploaded
            IProgress<long> progress = new Progress<long>(prog =>
            {
                Console.WriteLine($"Uploaded {prog} bytes of {fileStream.Length} bytes");
            });

            // Upload the file

            var uploadResult = await fileUploadTask.UploadAsync(progress);
```

# <a name="javascript"></a>[JavaScript](#tab/javascript)

```javascript

    const options = {
      authProvider,
    };
    const client = Client.init(options);
   
    const fileName = "test.txt";
    const file = fs.readFileSync(`./${fileName}`);
    const stats = fs.statSync(`./${fileName}`);
    const requestUrl ="https://graph.microsoft.com/v1.0/print/shares/{id}/jobs/{id}/documents/{id}/createuploadsession"
    const payload = {
        "properties": {
            "documentName": fileName,
            "contentType": "application/pdf",
            "size": stats.size
        }
    }
    const uploadSession = await LargeFileUploadTask.createUploadSession(client, requestUrl, payload);

    // Create FileUpload object. 
    /* Note:
     * As alternatives to using a javascript `File` object to create a `FileUpload`, 
     * you can use a `ReadStream` object to create a `StreamUpload`.
     * const readStream = fs.createReadStream(`./test/sample_files/${fileName}`);
     * const fileObject = new StreamUpload(readStream, fileName, totalsize);
     * OR
     * you can also create a custom implementation of the `FileObject` interface.
     * FileUpload and StreamUpload classes are available in 3.0.0 version of the Microsoft Graph JS client library.
     */
    const fileObject = new FileUpload(file, file.name, file.size);
     
    // Create LargeFileUploadTask object and start the upload() task
    const task = new LargeFileUploadTask(client, fileObject, uploadSession);
    const uploadResponse = await task.upload();
```
---

## <a name="cancel-the-upload-session"></a>Отмена сеанса отправки

Чтобы отменить сеанс отправки, отправьте запрос DELETE на URL-адрес отправки. Это следует делать в тех случаях, когда отправка прерывается (например, если пользователь отменил передачу).

Временные файлы и соответствующий сеанс отправки автоматически очищаются по прошествии времени, указанного свойством **expirationDateTime**.

### <a name="request"></a>Запрос

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-cancel", "scopes": "printjob.readwrite" } -->

```http
DELETE https://print.print.microsoft.com/uploadSessions/5400be13-5a4e-4c20-be70-90c85bfe5d6e?tempauthtoken={token}
```

### <a name="response"></a>Отклик

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```
