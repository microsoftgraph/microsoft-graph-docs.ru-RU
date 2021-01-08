---
title: 'printDocument: createUploadSession'
description: Создайте сеанс отправки для итеративной отправки диапазонов двоичных файлов printDocument.
localization_priority: Normal
author: nilakhan
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 0dbb2a9101fbf5033d1c91f1254c6ea0ba00f6e4
ms.sourcegitcommit: a0a5690ad9c109149e0b8c8baba164648ff5c226
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/08/2021
ms.locfileid: "49784851"
---
# <a name="printdocument-createuploadsession"></a>printDocument: createUploadSession

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте сеанс отправки, который позволяет приложению итеративно загружать диапазоны двоичного файла, связанного с документом печати.

В рамках ответа это действие возвращает URL-адрес отправки, который можно использовать в последующих `PUT` последовательном запросах. Для указания точного диапазона отгрузки можно использовать заготчики запросов для каждой `PUT` операции. Это позволяет возобновить передачу на случай, если сетевое подключение будет отброшено во время отправки. 

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из следующих разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).
Помимо следующих разрешений, у пользователя или клиента приложения должна быть активная подписка [](printer-get.md) универсальной печати и разрешение, которое предоставляет доступ "Получить принтер" или "Получить [printerShare"](printershare-get.md) в зависимости от того, используется ли принтер или printerShare.

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | PrintJob.Create, PrintJob.ReadWrite, PrintJob.ReadWrite.All |
| Делегированное (личная учетная запись Майкрософт) | Не поддерживается. |
| Приложение                            | PrintJob.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

Чтобы создать сеанс отправки с помощью **принтера:** 

<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/documents/{id}/createUploadSession
```

Чтобы создать сеанс отправки с помощью **printerShare:** 

<!-- { "blockType": "ignored" } -->
```http
POST /print/shares/{id}/jobs/{id}/documents/{id}/createUploadSession
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание   |
|:--------------|:--------------|
| Авторизация | Bearer {токен}. Обязательный. |
| Content-Type | application/json. Обязательный.|


## <a name="request-body"></a>Текст запроса

В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр    | Тип        | Описание |
|:-------------|:------------|:------------|
|properties|[printDocumentUploadProperties](../resources/printDocumentUploadProperties.md)|Представляет свойства двоичного файла, который необходимо отправить.|

Значение свойства **contentType** в теле запроса должно поддерживаться принтером или printerShare. Вы можете получить поддерживаемые типы контента, получив [printerCapabilities](../resources/printercapabilities.md) принтера или printerShare. 

Для **преобразования OXPS** в ФОРМАТ PDF необходимо передать в качестве contentType для `application/oxps` принтера или принтераShare, который поддерживает `application/pdf` . Универсальная печать преобразует **OXPS в ФОРМАТ PDF** при **следующих** условиях: 
1.  В `application/pdf` **printerCapabilities** поддерживается совместное использования принтера или принтера. 
2.  The printer/printer share does NOT support `application/oxps` in **printerCapabilities**. 
3.  Значение свойства **contentType** в теле запроса: `application/oxps` .

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика и новый объект `200 OK` [uploadSession](../resources/uploadsession.md) в тексте отклика.

>**Примечание.** Свойство **uploadUrl,** возвращаемого в рамках объекта ответа **uploadSession,** является непрозрачным URL-адресом для последующих запросов на отправку диапазонов байтов `PUT` файла. Он содержит соответствующий маркер auth для последующих запросов, срок действия `PUT` которых **истекает по истечении срока действия.** Не изменяя этот URL-адрес.

## <a name="examples"></a>Примеры

В следующем примере показано, как создать сеанс отправки, который можно использовать при последующих операциях отправки файлов в указанный printDocument.

### <a name="request"></a>Запрос

<!-- {
  "blockType": "request",
}-->
```http
POST https://graph.microsoft.com/beta/print/shares/1c879027-5120-4aaf-954a-ebfd509a3bcc/jobs/46207/documents/9001bcd9-e36a-4f51-bfc6-140c3ad7f9f7/createUploadSession
Content-type: application/json

{
  "properties": {
    "documentName": "TestFile.pdf",
    "contentType": "application/pdf", 
    "size": 4533322
  }
}
```

### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.uploadSession"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.uploadSession",
    "uploadUrl": "https://print.print.microsoft.com/uploadSessions/5400be13-5a4e-4c20-be70-90c85bfe5d6e?tempauthtoken={token}",
    "expirationDateTime": "2020-10-25T02:19:38.1694207Z",
    "nextExpectedRanges": [
        "0-4533321"
    ]
}
```
