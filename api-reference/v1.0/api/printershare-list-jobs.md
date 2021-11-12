---
title: Список printJobs для принтераShare
description: Извлечение списка заданий печати, связанных с совместной печатью.
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 5d19fbfc79ee464d6149ed645c3e48448e163654
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2021
ms.locfileid: "60941619"
---
# <a name="list-printjobs-for-a-printershare"></a>Список printJobs для принтераShare
Пространство имен: microsoft.graph

Извлечение списка заданий печати, связанных с [принтеромShare.](../resources/printershare.md)

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

Чтобы использовать службу универсальной печати, клиент пользователя или приложения должен иметь активную подписку на универсальную печать, разрешение, предоставляемую доступ [к принтеру Get PrinterShare,](printershare-get.md) и одно из разрешений, перечисленных в следующей таблице.

Чтобы прочитать задания печати у другого пользователя, пользователь должен быть администратором печати и иметь разрешение PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All или PrintJob.ReadWrite.All.

|Тип разрешения | Разрешения (в порядке повышения привилегий) |
|:---------------|:--------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)| PrintJob.ReadBasic, PrintJob.Read, PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений| PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/shares/{printerShareId}/jobs
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает некоторые параметры запросов OData для настройки отклика. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

* Свойство **documents** по умолчанию опущено из ответа. Чтобы также вернуть список [печатных документов](../resources/printdocument.md) для каждого задания печати, используйте `$expand=documents` .
* Этот метод поддерживает фильтрацию заданий печати пользователем, который их создал. Используйте `$filter=createdBy/userPrincipalName eq '{upn}'` , **где {upn}** — это [основное имя](/azure/active-directory/hybrid/plan-connect-userprincipalname#what-is-userprincipalname) пользователя связанного пользователя.

### <a name="exceptions"></a>Исключения
Некоторые операторы не поддерживаются: `$count` , `$search` .

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [printJob](../resources/printjob.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_printjob_2"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/shares/{printerShareId}/jobs
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-printjob-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-printjob-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-printjob-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-printjob-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик
**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.printJob)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/shares('f37141d9-0afb-484f-96d3-0ef0a679e6c1')/jobs",
  "value": [
    {
      "id": "103",
      "createdDateTime": "2020-02-04T00:00:00.0000000Z",
      "createdBy": {        
      },
      "status": {
        "state": "completed",
        "description": "The print job has completed successfully and no further processing will take place.",
        "details": [          
        ],
        "isAcquiredByPrinter": true
      },
      "configuration": {        
      },
      "redirectedTo": null,
      "redirectedFrom": null,
      "isFetchable": false
    }
  ]
}
```

