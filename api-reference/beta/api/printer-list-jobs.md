---
title: Список printJobs для принтера
description: Извлечение списка заданий печати, связанных с принтером.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 8bda64c21c2f94a40115b24bc9297451efed417a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960912"
---
# <a name="list-printjobs-for-a-printer"></a>Список printJobs для принтера

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Извлечение списка заданий печати, связанных с [принтером.](../resources/printer.md)

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

Чтобы использовать службу универсальной печати, клиент пользователя или приложения должен иметь активную подписку на универсальную печать, разрешение на получение доступа к принтеру и одно из разрешений, перечисленных в следующей таблице. [](printer-get.md) Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)

Чтобы прочитать задания печати у другого пользователя, пользователь должен быть администратором печати и иметь разрешение PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All или PrintJob.ReadWrite.All.

|Тип разрешения | Разрешения (в порядке повышения привилегий) |
|:---------------|:--------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)| PrintJob.ReadBasic, PrintJob.Read, PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Application| PrintJob.ReadBasic.All, PrintJob.Read.All, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/jobs
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает некоторые параметры запросов OData для настройки отклика. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

* Свойство **documents** по умолчанию опущено из ответа. Чтобы также вернуть список [печатных документов](../resources/printdocument.md) для каждого задания печати, используйте `$expand=documents` .
* Этот метод поддерживает фильтрацию заданий печати пользователем, который их создал. Используйте `$filter=createdBy/userPrincipalName eq '{upn}'` , **где {upn}** — это [основное имя](/azure/active-directory/hybrid/plan-connect-userprincipalname#what-is-userprincipalname) пользователя связанного пользователя.

### <a name="exceptions"></a>Exceptions
Некоторые операторы не поддерживаются: `$count` , `$search` `$filter` .

## <a name="request-headers"></a>Заголовки запросов
| Имя      |Описание|
|:----------|:----------|
| Авторизация | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.
## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код ответа и `200 OK` коллекцию [объектов printJob](../resources/printjob.md) в тексте отклика.
## <a name="example"></a>Пример
### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_jobs_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}/jobs
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-jobs-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-jobs-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-jobs-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-jobs-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

### <a name="response"></a>Отклик
Ниже приведен пример отклика.
>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJob",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 461

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers('c05f3726-0d4b-4aa1-8fe9-2eb981bb26fb')/jobs",
  "value": [
    {
      "id": "5182",
      "createdDateTime": "2020-02-04T00:00:00.0000000Z",
      "createdBy": {},
      "status": {
        "processingState": "completed",
        "processingStateDescription": "The print job has completed successfully and no further processing will take place."
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List jobs",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
