---
title: Создание subjectRightsRequest
description: Создайте объект subjectRightsRequest.
author: skadam-msft
ms.localizationpriority: medium
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 9c4530948142d639295993d24f4c44392e647af4
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461494"
---
# <a name="create-subjectrightsrequest"></a>Создание subjectRightsRequest
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте объект [subjectRightsRequest](../resources/subjectrightsrequest.md) .

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись)|SubjectRightsRequest.ReadWrite.All|
|Делегированное (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается|

## <a name="http-request"></a>HTTP-запрос

[!INCLUDE [subject-rights-request-privacy-deprecate](../../includes/subject-rights-request-privacy-deprecate.md)]

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /security/subjectRightsRequests
POST /privacy/subjectRightsRequests

```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [subjectRightsRequest](../resources/subjectrightsrequest.md) в формате JSON.

В следующей таблице показаны свойства, необходимые при создании [subjectRightsRequest](../resources/subjectrightsrequest.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
| contentQuery         | Строка | KQL на основе запроса содержимого, который должен использоваться для поиска. Это свойство определяется только для интерфейсов API `\security` , к ним можно получить доступ с помощью пути запроса, а не пути `\privacy` запроса.|
|dataSubject|[microsoft.graph.dataSubject](../resources/datasubject.md)|Содержит свойства субъекта данных для запроса.|
|dataSubjectType|dataSubjectType|Тип субъекта данных. Возможные значения: `customer`, `currentEmployee`, `formerEmployee`, `prospectiveEmployee`, `student`, `teacher`, `faculty`, `other`, `unknownFutureValue`.|
|description|Строка|Описание запроса.|
|displayName|String|Имя запроса.|
| externalId           | String| Внешний идентификатор запроса, который неизменяем после создания и используется для отслеживания запроса внешней системы. Это свойство определяется только для интерфейсов API `\security` , к ним можно получить доступ с помощью пути запроса, а не пути `\privacy` запроса.|
| includeAllVersions   | Boolean | Включите все версии документов. По умолчанию будут возвращены текущие копии документов. Если SharePoint сайтов включено управление версиями, включая все версии, будут включены исторические копии документов. Это свойство определяется только для интерфейсов API `\security` , к ним можно получить доступ с помощью пути запроса, а не пути `\privacy` запроса.|
| includeAuthoredContent| Boolean | Включите контент, созданный субъектом данных. Это свойство определяется только для интерфейсов API `\security` , к ним можно получить доступ с помощью пути запроса, а не пути `\privacy` запроса.|
|internalDueDateTime|DateTimeOffset|Внутренняя дата выполнения, используемая для отслеживания завершения запроса.|
| mailboxLocations     | [subjectRightsRequestMailboxLocation](../resources/subjectrightsrequestmailboxlocation.md)|Расположения почтовых ящиков, в которых должен выполняться поиск. Это свойство определяется только для интерфейсов API `\security` , к ним можно получить доступ с помощью пути запроса, а не пути `\privacy` запроса.|
| pauseAfterEstimate   | Boolean| Приостановка запроса после завершения оценки. По умолчанию оценка данных будет выполняться, а затем приостанавливаться, что позволяет просмотреть результаты, а затем выбрать параметр для получения данных в пользовательском интерфейсе. Это свойство можно задать, `false` если требуется выполнить оценку, а затем автоматически начать с извлечения содержимого. Это свойство определяется только для интерфейсов API `\security` , к ним можно получить доступ с помощью пути запроса, а не пути `\privacy` запроса.|
|Правила|Коллекция String|Одно или несколько нормативных требований для запроса.|
| siteLocations| [subjectRightsRequestSiteLocation](../resources/subjectrightsrequestsitelocation.md)| В SharePoint и OneDrive сайтов, в которых должен выполняться поиск. Это свойство определяется только для интерфейсов API `\security` , к ним можно получить доступ с помощью пути запроса, а не пути `\privacy` запроса.|
|type|subjectRightsRequestType|Тип запроса. Возможные значения: `export`, `access`, `tagForAction`, `unknownFutureValue`. Тип `delete` в настоящее время не поддерживается.|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код `201 Created` отклика и объект [subjectRightsRequest](../resources/subjectRightsRequest.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_subjectRightsRequest_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/privacy/subjectRightsRequests
Content-Type: application/json

{
    "type": "export",
    "contentQuery": "((\"Diego Siciliani\" OR \"Diego.Siciliani@contoso.com\") OR (participants:\"Diego.Siciliani@contoso.com\"))",
    "dataSubjectType": "customer",
    "externalId": "F53BF2DA-607D-412A-B568-FAA0F023AC0B",
    "displayName": "Export report for customer Id: 12345",
    "description": "This is a export request",
    "includeAllVersions": false,
    "includeAuthoredContent": true,
    "internalDueDateTime": "2022-07-20T22:42:28Z",
    "dataSubject": {
        "firstName": "Diego",
        "lastName": "Siciliani",
        "email": "Diego.Siciliani@contoso.com",
        "residency": "USA"
    },
    "mailboxLocations": null,
    "pauseAfterEstimate": true,
    "regulations": [
        "CCPA"
    ],
    "siteLocations": {
        "@odata.type": "microsoft.graph.subjectRightsRequestAllSiteLocation"
    }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-subjectrightsrequest-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-subjectrightsrequest-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-subjectrightsrequest-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-subjectrightsrequest-from--go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subjectRightsRequest"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "type": "export",
    "dataSubjectType": "customer",
    "regulations": [
        "CCPA"
    ],
    "displayName": "Export report for customer Id: 12345",
    "description": "This is a export request",
    "status": "active",
    "internalDueDateTime": "2022-07-20T22:42:28Z",
    "lastModifiedDateTime": "2022-05-10T22:42:28Z",
    "id": "CA084038-C5D2-493D-8DAB-23FC12393C76",
    "createdDateTime": "2022-05-10T22:42:28Z",
    "stages": [
        {
            "stage": "contentRetrieval",
            "status": "notStarted",
            "error": null
        },
        {
            "stage": "contentReview",
            "status": "notStarted",
            "error": null
        },
        {
            "stage": "generateReport",
            "status": "notStarted",
            "error": null
        },
        {
            "stage": "caseResolved",
            "status": "notStarted",
            "error": null
        }
    ],
    "createdBy": {
        "user": {
            "id": "1B761ED2-AA7E-4D82-9CF5-C09D737B6167",
            "displayName": "srradmin@contoso.com"
        }
    },
    "lastModifiedBy": {
        "user": {
            "id": "1B761ED2-AA7E-4D82-9CF5-C09D737B6167",
            "displayName": "srradmin@contoso.com"
        }
    },
    "dataSubject": {
        "firstName": "Diego",
        "lastName": "Siciliani",
        "email": "Diego.Siciliani@contoso.com",
        "residency": "USA"
    },
    "team": {
        "id": "5484809c-fb5b-415a-afc6-da7ff601034e",
        "webUrl": "https://teams.contoso.com/teams/teamid"
    },
    "includeAllVersions": false,
    "pauseAfterEstimate": false,
    "includeAuthoredContent": false,
    "externalId": "F53BF2DA-607D-412A-B568-FAA0F023AC0B",
    "contentQuery": "((\"Diego Siciliani\" OR \"Diego.Siciliani@contoso.com\") OR (participants:\"Diego.Siciliani@contoso.com\"))",
    "mailboxLocations": null,
    "siteLocations": {
        "@odata.type": "microsoft.graph.subjectRightsRequestAllSiteLocation"
    }
}
```

