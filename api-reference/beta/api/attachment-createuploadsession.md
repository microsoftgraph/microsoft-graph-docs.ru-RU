---
title: 'вложение: createUploadSession'
description: Создайте сеанс отправки для последовательной отправки диапазонов файла, чтобы прикрепить файл к указанному сообщению.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a068413b1849da27f3723bb9d006ab487b07a3a0
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2020
ms.locfileid: "42589917"
---
# <a name="attachment-createuploadsession"></a>вложение: createUploadSession

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте сеанс отправки, который позволяет приложению итеративно отправлять диапазоны файлов, чтобы прикрепить файл к элементу Outlook. Элемент может быть [сообщением](../resources/message.md) или [событием](../resources/event.md).

Используйте этот способ, чтобы вложить файл, если размер файла находится в пределах от 3 МБ до 150 МБ. Чтобы присоединить файл размером менее 3 МБ, выполните `POST` операцию для свойства навигации **вложений** элемента Outlook; сведения о том, как сделать это [для сообщения](message-post-attachments.md) или [события](event-post-attachments.md). 

В качестве части ответа это действие возвращает URL-адрес отправки, который можно использовать в последующих последовательных `PUT` запросах. Заголовки запросов для каждой `PUT` операции позволяют указать точный диапазон байтов для отправки. Это позволяет возобновить передачу в случае, если сетевое подключение будет разорвано во время отправки. 

Ниже приведены действия по присоединению файла к элементу Outlook с помощью сеанса отправки:

1. Создание сеанса отправки.
2. В пределах этого сеанса передачи, итеративно отправлять диапазоны байтов (до 4 МБ каждый раз), пока не будут отправлены все байты файла, а файл будет присоединен к указанному элементу.
3. Сохраните идентификатор вложения для последующего доступа.
4. Необязательно: удалите сеанс отправки.

В этом примере показано, [как прикрепить крупные файлы к сообщениям или событиям Outlook](/graph/outlook-large-attachments) .

> [!TIP]
> Exchange Online позволяет администраторам настраивать ограничения на размер сообщений для почтовых ящиков Office 365, включая вложения в сообщения. По умолчанию это максимальный размер сообщения 35 МБ. Узнайте [, как настроить максимальный размер сообщения](https://www.microsoft.com/microsoft-365/blog/2015/04/15/office-365-now-supports-larger-email-messages-up-to-150-mb) для поддержки вложений, превышающих ограничение по умолчанию для клиента. 

> [!IMPORTANT] 
> Если вы присоединяете большой файл к сообщению или событию в общем или делегированном почтовом ящике, учитывайте [известную ошибку](/graph/known-issues#attaching-large-files-to-messages) .


## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Mail.ReadWrite |
| Делегированные (личная учетная запись Майкрософт) | Mail.ReadWrite |
| Для приложений                            | Mail.ReadWrite |

## <a name="http-request"></a>HTTP-запрос

Создание сеанса отправки для присоединения файла к **событию**: 

<!-- { "blockType": "ignored" } -->
```http
POST /me/events/{id}/attachments/createUploadSession
```

Создание сеанса отправки для вложения файла в **сообщение**: 

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
|аттачментитем|[аттачментитем](../resources/attachmentitem.md)|Представляет атрибуты элемента, который требуется отправить и вложить. Как минимум, укажите тип вложения (`file`), имя и размер файла.|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [uploadSession](../resources/uploadsession.md) в тексте отклика.

>**Примечание.** 
>
>Свойство **адрес uploadurl** , возвращаемое как часть объекта Response **uploadSession** , является непрозрачным URL- `PUT` адресом для последующих запросов на отправку диапазонов байтов файла. Он содержит соответствующий маркер проверки подлинности `PUT` для последующих запросов, срок действия которых истечет через **expirationDateTime**. Не настраивайте этот URL-адрес.
>
>Свойство **nextExpectedRanges** указывает местоположение байта следующего файла, из которого необходимо выполнить загрузку, например `"NextExpectedRanges":["2097152"]`. Байты файла необходимо отправлять по порядку.

<!-- The **nextExpectedRanges** property specifies one or more ranges of bytes that the server is still missing for the file. These ranges are zero-indexed and of the format `{start}-{end}`, unless if the server misses the remainder of the bytes from the start of that range, in which case the format is simply `{start}`.  -->


## <a name="examples"></a>Примеры

В приведенном ниже примере показано, как создать сеанс отправки, который можно использовать в последующих операциях отправки файлов для указанного сообщения.

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "attachment_createuploadsession",
  "sampleKeys": ["AAMkADI5MAAIT3drCAAA="]
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADI5MAAIT3drCAAA=/attachments/createUploadSession
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.uploadSession",
    "uploadUrl": "https://outlook.office.com/api/beta/Users('a8e8e219-4931-95c1-b73d-62626fd79c32@72aa88bf-76f0-494f-91ab-2d7cd730db47')/Messages('AAMkADI5MAAIT3drCAAA=')/AttachmentSessions('AAMkADI5MAAIT3k0uAAA=')?authtoken=eyJhbGciOiJSUzI1NiIsImtpZCI6IktmYUNIUlN6bllHMmNI",
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
