---
title: 'вложение: createUploadSession'
description: Создайте сеанс отправки для последовательной отправки диапазонов файла, чтобы прикрепить файл к указанному сообщению.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 116b73b53689c01e346568b6b5d67e56fb31b283
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2019
ms.locfileid: "37621619"
---
# <a name="attachment-createuploadsession"></a>вложение: createUploadSession

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте сеанс отправки, который позволяет приложению итеративно отправлять диапазоны файлов, чтобы прикрепить файл к указанному [сообщению](../resources/message.md).

Используйте этот способ, чтобы вкладывать в **сообщение**файлы размером от 3 МБ до 150MB. Чтобы прикрепить файлы размером в 4 МБ, просто [выполните команду POST в свойстве навигации вложений](message-post-attachments.md). 

В качестве части ответа это действие возвращает URL-адрес отправки, который можно использовать в последующих последовательных `PUT` запросах. Заголовки запросов для каждой `PUT` операции позволяют указать точный диапазон байтов для отправки. Это позволяет возобновить передачу в случае, если сетевое подключение будет разорвано во время отправки. 

Ниже приведены действия по присоединению файла с помощью сеанса отправки.

1. Создание сеанса отправки
2. В пределах этого сеанса передачи, итеративно отправлять диапазоны байтов (до 4 МБ каждый раз), пока не будут отправлены все байты файла, а файл будет присоединен к указанному сообщению.
3. Сохранение идентификатора вложения для последующего доступа
4. Необязательно: Удаление сеанса отправки 

В этом примере показано, как [прикрепить большие файлы к сообщениям Outlook](/graph/outlook-large-attachments) .


## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Mail.ReadWrite |
| Делегированные (личная учетная запись Майкрософт) | Mail.ReadWrite |
| Для приложений                            | Mail.ReadWrite |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/attachments/createUploadSession
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание   |
|:--------------|:--------------|
| Авторизация | Bearer {token} |


## <a name="request-body"></a>Тело запроса

В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр    | Тип        | Описание |
|:-------------|:------------|:------------|
|аттачментитем|[аттачментитем](../resources/attachmentitem.md)|Представляет атрибуты элемента, который требуется отправить и вложить. Как минимум, укажите тип вложения (`file`), имя и размер файла.|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод `201, Created` возвращает код отклика и новый объект [uploadSession](../resources/uploadsession.md) в тексте отклика.

>**Примечание.** 
>
>Свойство **адрес uploadurl** , возвращаемое как часть объекта Response **uploadSession** , является непрозрачным URL- `PUT` адресом для последующих запросов на отправку диапазонов байтов файла. Он содержит соответствующий маркер проверки подлинности `PUT` для последующих запросов, срок действия которых истечет через **expirationDateTime**. Не настраивайте этот URL-адрес.
>
>Свойство **nextExpectedRanges** указывает местоположение байта следующего файла, из которого необходимо выполнить загрузку, например `"NextExpectedRanges":["2097152"]`. Необходимо отправлять байты в файле по порядку.

<!-- The **nextExpectedRanges** property specifies one or more ranges of bytes that the server is still missing for the file. These ranges are zero-indexed and of the format `{start}-{end}`, unless if the server misses the remainder of the bytes from the start of that range, in which case the format is simply `{start}`.  -->


## <a name="examples"></a>Примеры

Ниже приведен пример вызова этого API.

### <a name="request"></a>Запрос

Ниже приведен пример запроса.
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

### <a name="response"></a>Отклик

Ниже приведен пример отклика.

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