---
title: 'attachment: createUploadSession'
description: Создайте сеанс отправки для итеративной отправки диапазонов файла, чтобы встроить файл в указанное сообщение.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 4e36ba5570fdf02814c8ff28483e9ac60278806f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131420"
---
# <a name="attachment-createuploadsession"></a>attachment: createUploadSession

Пространство имен: microsoft.graph

Создайте сеанс отправки, который позволяет приложению итеративно загружать диапазоны файла, чтобы встроить файл в указанный элемент Outlook. Элемент может быть [сообщением или](../resources/message.md) [событием.](../resources/event.md)

Используйте этот подход для вложения файла, если размер файла составляет от 3 до 150 МБ. Чтобы встроить файл размером менее 3 МБ, сделайте операцию со свойством навигации вложений элемента Outlook. Узнайте, как это сделать для сообщения или `POST` [события.](event-post-attachments.md)  [](message-post-attachments.md) 

В рамках ответа это действие возвращает URL-адрес отправки, который можно использовать в последующих `PUT` последовательном запросе. В загонах запросов для каждой операции можно указать точный диапазон отгрузки. `PUT` Это позволяет возобновить передачу на случай, если сетевое подключение будет отброшено во время отправки. 

Ниже следующую постройки вложите файл в элемент Outlook с помощью сеанса отправки.

1. Создание сеанса отправки.
2. В этом сеансе отправки итеративным образом загружаются диапазоны в диапазоне до 4 МБ каждый раз, пока не будут загружены все файлы и файл вложен в указанный элемент.
3. Сохраните ИД вложения для дальнейшего доступа.
4. Необязательно: удалите сеанс отправки.

См. [пример прикрепления](/graph/outlook-large-attachments) больших файлов к сообщениям или событиям Outlook.

> [!TIP]
> Exchange Online позволяет администраторам настраивать ограничение на размер сообщений для почтовых ящиков Microsoft 365, включая вложения в сообщения. По умолчанию это ограничение составляет 35 МБ. Узнайте, как настроить [максимальный](https://www.microsoft.com/microsoft-365/blog/2015/04/15/office-365-now-supports-larger-email-messages-up-to-150-mb) размер сообщения для поддержки вложений, которые больше предельного значения по умолчанию для клиента. 

> [!IMPORTANT] 
> Следует помнить об [известной](/graph/known-issues#attaching-large-files-to-messages) проблеме при вложении большого файла в сообщение или событие в общем или делегированного почтовом ящике.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Calendars.ReadWrite, Mail.ReadWrite |
| Делегированные (личная учетная запись Майкрософт) | Calendars.ReadWrite, Mail.ReadWrite |
| Для приложений                            | Calendars.ReadWrite, Mail.ReadWrite |

## <a name="http-request"></a>HTTP-запрос

Создание сеанса отправки для вложения файла в **событие:** 

<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/attachments/createUploadSession
```

Создание сеанса отправки для вложения файла в **сообщение:** 

<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/attachments/createUploadSession
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание   |
|:--------------|:--------------|
| Authorization | Bearer {token} |


## <a name="request-body"></a>Текст запроса

В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр    | Тип        | Описание |
|:-------------|:------------|:------------|
|AttachmentItem|[attachmentItem](../resources/attachmentitem.md)|Представляет атрибуты элемента, который необходимо отправить и встроить. Укажите как минимум тип вложения ( ), имя и `file` размер файла.|

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика и новый объект `201 Created` [uploadSession](../resources/uploadsession.md) в тексте отклика.

>**Примечание.** 
>
>Свойство **uploadUrl,** возвращенное как часть объекта ответа **uploadSession,** является непрозрачным URL-адресом для последующих запросов на отправку диапазонов байтов `PUT` файла. Он содержит соответствующий маркер auth для последующих запросов, срок действия `PUT` которых **истекает по истечении срока действия.** Не настраивать этот URL-адрес.
>
>Свойство **nextExpectedRanges** указывает следующее расположение файла для отправки, `"NextExpectedRanges":["2097152"]` например. Байты файла необходимо отправлять по порядку.

<!-- The **nextExpectedRanges** property specifies one or more ranges of bytes that the server is still missing for the file. These ranges are zero-indexed and of the format `{start}-{end}`, unless if the server misses the remainder of the bytes from the start of that range, in which case the format is simply `{start}`.  -->


## <a name="examples"></a>Примеры

В следующем примере показано, как создать сеанс отправки, который можно использовать при последующих операциях отправки файлов в указанное сообщение.

### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "attachment_createuploadsession",
  "sampleKeys": ["AAMkADI5MAAIT3drCAAA="]
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/AAMkADI5MAAIT3drCAAA=/attachments/createUploadSession
Content-type: application/json

{
  "AttachmentItem": {
    "attachmentType": "file",
    "name": "flower", 
    "size": 3483322
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/attachment-createuploadsession-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/attachment-createuploadsession-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/attachment-createuploadsession-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/attachment-createuploadsession-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

> **Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "name": "attachment_createuploadsession",
  "truncated": true,
  "@odata.type": "microsoft.graph.uploadSession"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.uploadSession",
    "uploadUrl": "https://outlook.office.com/api/v1.0/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/AttachmentSessions('AAMkADI5MAAIT3k0uAAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIUlN6bllHMmNI",
    "expirationDateTime": "2019-09-25T01:09:30.7671707Z",
    "nextExpectedRanges": [
        "0-"
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attachment: createUploadSession",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

