---
title: Отправка документов с помощью API универсальной печати Microsoft Graph
description: Универсальная печать — это современное решение печати, которое можно использовать в организациях для управления инфраструктурой печати через облачные службы Майкрософт.
author: nilakhan
localization_priority: Priority
ms.prod: universal-print
ms.custom: scenarios:getting-started
ms.openlocfilehash: 448c0525a318cac64bb5d381b986c238f563025d
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515703"
---
# <a name="upload-documents-using-the-microsoft-graph-universal-print-api"></a>Отправка документов с помощью API универсальной печати Microsoft Graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../api-reference/includes/cloudprinting-pricing-disclaimer.md)]

Чтобы напечатать документ с помощью API универсальной печати в Microsoft Graph, [создайте задание печати](/graph/api/printershare-post-jobs), отправьте документ и [запустите задание печати](/graph/api/printjob-start). В этой статье описано, как отправить документ, начиная с [создания сеанса отправки](/graph/api/printdocument-createuploadsession).

Чтобы отправить файл или его часть, приложение отправляет запрос PUT на адрес **uploadUrl**, указанный в ответе для **createUploadSession**.
Вы можете отправить файл целиком или разделить его на несколько диапазонов байтов. При этом каждый запрос должен содержать фрагмент размером менее 10 МБ.

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
### <a name="http-response"></a>HTTP-ответ

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
* В ответ на добавление заголовка авторизации при совершении вызова `PUT` может появиться сообщение об ошибке `HTTP 401 Unauthorized`. Заголовок авторизации и маркер носителя необходимо отправлять только при создании сеанса отправки. Их не следует включать при отправке данных для сеанса отправки.

## <a name="completing-a-file"></a>Завершение отправки файла

После получения последнего диапазона байтов файла сервер отправляет ответ `HTTP 201 Created`. Текст ответа также будет включать набор свойств для связанного **printDocument**.

<!-- { "blockType": "request", "opaqueUrl": true, "name": "upload-fragment-final", "scopes": "printjob.readwrite" } -->

```http
PUT https://print.print.microsoft.com/uploadSessions/5400be13-5a4e-4c20-be70-90c85bfe5d6e?tempauthtoken={token}
Content-Length: 10
Content-Range: bytes 4533312-4533321/4533322

<final bytes of the file>
```

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
