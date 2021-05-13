---
title: Создание accessReviewHistoryDefinition
description: Создайте новый объект accessReviewHistoryDefinition.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 3c0a1309ae67a2f4aa3f066deb5fe8adeec84119
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474124"
---
# <a name="create-accessreviewhistorydefinition"></a>Создание accessReviewHistoryDefinition

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте новый [объект accessReviewHistoryDefinition.](../resources/accessreviewhistorydefinition.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|AccessReview.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|AccessReview.ReadWrite.All|

В роли каталога должен также быть подписан пользователь, который позволяет им читать обзор доступа для получения любых данных.  Дополнительные сведения см. в дополнительных сведениях о требованиях к роли и разрешению для [отзывов о доступе.](../resources/accessreviewsv2-root.md)

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/accessReviews/historyDefinitions
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

В теле запроса поставляют представление JSON объекта [accessReviewHistoryDefinition.](../resources/accessreviewhistorydefinition.md)

В следующей таблице показаны необходимые свойства, используемые для создания [accessReviewHistoryDefinition.](../resources/accessreviewhistorydefinition.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName | String  | Имя для сбора данных истории проверки доступа. Обязательно. |
|reviewHistoryPeriodStartDateTime  | DateTimeOffset  | Timestamp, отзывы, начиная с этой даты или после нее, будут включены в извлеченные данные истории. Обязательно.  |
|reviewHistoryPeriodEndDateTime  | DateTimeOffset  | Timestamp, отзывы, начиная с этой даты или до этой даты, будут включены в извлеченные данные истории. Обязательный.  |
|scopes|коллекция microsoft.graph.accessReviewQueryScope| Используется для фильтрации отзывов, включенных в извлеченные данные истории. Извлекает отзывы, область которых совпадает с этой предоставленной областью. Обязательно.  |

### <a name="supported-scope-queries-for-accessreviewhistorydefinition"></a>Поддерживаемые запросы области для accessReviewHistoryDefinition

Ниже приводится запросы, поддерживаемые [в accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) на основе [accessreviewqueryscope.](../resources/accessreviewqueryscope.md) Эти области диктуют, какой тип данных истории отзывов входит в загружаемый CSV-файл, который создается при создания определения.

|Сценарий| Запрос |
|--|--|
| Включайте каждый результат проверки для отдельных групп (исключает определения, охватываемые для всех Microsoft 365 `accessReviewScheduleDefinition` групп с гостевых пользователей) | /identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups')" |
| Включайте каждый результат проверки в определенную группу (исключает определения, охватываемые для всех Microsoft 365 `accessReviewScheduleDefinition` групп с гостевых пользователей) | /identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups/{group id}') |
| Включайте каждый результат проверки для `accessReviewScheduleDefinition` всех Microsoft 365 групп с гостевых пользователей | /identityGovernance/accessReviews/definitions?$filter=contains(scope/query, './members') |
| `accessReviewScheduleDefinition`Включи каждый результат проверки в пакет доступа | /identityGovernance/accessReviews/definitions?$filter=contains (scope/query, 'accessPackageAssignments') |
| `accessReviewScheduleDefinition`Включай каждый результат проверки для директоров служб, назначенных привилегированной роли | /identityGovernance/accessReviews/definitions?$filter=contains(scope/query, 'roleAssignmentScheduleInstances') |
| `accessReviewScheduleDefinition`Включи каждый результат проверки для reivews определенной группы | /identityGovernance/accessReviews/definitions?$filter=scope/query eq '/groups/a1382a9b-8320-4e9c-8f73-dfead37d7723/members' |

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) в тексте ответа.

## <a name="examples"></a>Примеры

В следующем примере показано, как создать определение истории доступа для доступа к отзывам по пакетам и группам доступа, которое будет работать между датой начала 01/01/2021 и датой окончания 04/05/2021.

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accessreviewhistorydefinition_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/historyDefinitions
Content-Type: application/json

{
  "displayName": "Last quarter's group reviews April 2021",
  "decisions": [
    "approve",
    "deny",
    "dontKnow",
    "notReviewed",
    "notNotified"
  ],
  "reviewHistoryPeriodStartDateTime": "2021-01-01T00:00:00Z",
  "reviewHistoryPeriodEndDateTime": "2021-04-05T00:00:00Z",
  "scopes": [
    {
      "@odata.type": "#microsoft.graph.accessReviewQueryScope",
      "queryType": "MicrosoftGraph",     
      "query": "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, 'accessPackageAssignments')",
      "queryRoot": null
    },  
    {
      "@odata.type": "#microsoft.graph.accessReviewQueryScope",
      "queryType": "MicrosoftGraph",     
      "query": "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups')",
      "queryRoot": null
    }
  ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accessreviewhistorydefinition-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accessreviewhistorydefinition-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accessreviewhistorydefinition-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accessreviewhistorydefinition-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewHistoryDefinition"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.accessReviewHistoryDefinition",
  "id": "b2cb022f-b7e1-40f3-9854-c65a40861c38",
  "displayName": "Last quarter's group reviews April 2021",
  "reviewHistoryPeriodStartDateTime": "2021-01-01T00:00:00Z",
  "reviewHistoryPeriodEndDateTime": "2021-04-05T00:00:00Z",
  "decisions": [
    "approve",
    "deny",
    "dontKnow",
    "notReviewed",
    "notNotified"
  ],
  "status": "requested",
  "createdDateTime": "2021-04-14T00:22:48.9392594Z",
  "fulfilledDateTime": null,
  "downloadUri": null,
  "createdBy": {
      "id": "957f1027-c0ee-460d-9269-b8444459e0fe",
      "displayName": "MOD Administrator",
      "userPrincipalName": "admin@contoso.com"
  },
  "scopes": [
    {
      "@odata.type": "#microsoft.graph.accessReviewQueryScope",
      "queryType": "MicrosoftGraph",     
      "query": "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, 'accessPackageAssignments')",
      "queryRoot": null
    },  
    {
      "@odata.type": "#microsoft.graph.accessReviewQueryScope",
      "queryType": "MicrosoftGraph",     
      "query": "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups')",
      "queryRoot": null
    }
  ]
}
```
