---
title: 'printDocument: createUploadSession'
description: Создайте сеанс отправки для последовательной отправки диапазонов двоичного файла printDocument.
localization_priority: Normal
author: nilakhan
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 47043b64806cfa9ef3a66026a60b84ae11112168
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48705142"
---
# <a name="printdocument-createuploadsession"></a>printDocument: createUploadSession

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте сеанс отправки, позволяющий приложению итеративно отправлять диапазоны двоичного файла, связанного с печатным документом.

В качестве части ответа это действие возвращает URL-адрес отправки, который можно использовать в последующих последовательных `PUT` запросах. Заголовков запросов для каждой `PUT` операции можно использовать для указания точного диапазона байтов, которые необходимо отправить. Это позволяет возобновить передачу в случае, если сетевое подключение будет разорвано во время отправки. 

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из следующих разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).
В дополнение к следующим разрешениям пользователь или клиент приложения должен иметь активную универсальную подписку на печать и иметь разрешение на получение доступа к [принтеру](printer-get.md) или [Получение](printershare-get.md) доступа к принтершаре в зависимости от того, используется ли принтер или принтершаре.

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | PrintJob. ReadWrite, PrintJob. ReadWrite. ALL |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | PrintJob.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

Чтобы создать сеанс отправки с помощью **принтера**, выполните следующие действия: 

<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/jobs/{id}/documents/{id}/createUploadSession
```

Чтобы создать сеанс отправки с помощью **принтершаре**, выполните указанные ниже действия. 

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
|properties|[принтдокументуплоадпропертиес](../resources/printDocumentUploadProperties.md)|Представляет свойства двоичного файла, который необходимо отправить.|

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и новый объект [uploadSession](../resources/uploadsession.md) в тексте отклика.

>**Note**: свойство **адрес uploadurl** , возвращаемое как часть объекта Response **uploadSession** , является непрозрачным URL-адресом для последующих `PUT` запросов на отправку диапазонов байтов файла. Он содержит соответствующий маркер проверки подлинности для последующих `PUT` запросов, срок действия которых истечет через **expirationDateTime**. Не изменяйте этот URL-адрес.

## <a name="examples"></a>Примеры

В приведенном ниже примере показано, как создать сеанс отправки, который можно использовать в последующих операциях отправки файлов для указанного элемента printDocument.

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
