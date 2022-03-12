---
title: Создание historyDefinitions
description: Создайте новый объект accessReviewHistoryDefinition.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 7533b52e58f7229043bf9e6132ca02d36d7acc29
ms.sourcegitcommit: 1ae0079021dfcbcc910dcdc74440d367ec4af7d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2022
ms.locfileid: "63460135"
---
# <a name="create-historydefinitions"></a>Создание historyDefinitions

Пространство имен: microsoft.graph

Создайте новый [объект accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) .

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|AccessReview.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|AccessReview.ReadWrite.All|

В роли каталога должен также быть подписан пользователь, который позволяет им читать обзор доступа для получения любых данных.  Дополнительные сведения см. в дополнительных сведениях о требованиях к роли и разрешениям для [отзывов о доступе](../resources/accessreviewsv2-overview.md).

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
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

В теле запроса поставляют представление JSON объекта [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) .

В следующей таблице показаны необходимые свойства, используемые для создания [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName | String  | Имя для сбора данных истории проверки доступа. Обязательный. |
|reviewHistoryPeriodStartDateTime  | DateTimeOffset  | Timestamp. Отзывы, начиная с этой даты или после нее, будут включены в извлеченные данные истории. Только если **расписаниеSettings** не определено.  |
|reviewHistoryPeriodEndDateTime  | DateTimeOffset  | Timestamp. Обзоры, начиная с этой даты или до этой даты, будут включены в извлеченные данные истории. Только если **расписаниеSettings** не определено.  |
|scopes|[accessReviewQueryScope](../resources/accessreviewqueryscope.md) collection| Используется для фильтрации отзывов, включенных в извлеченные данные истории. Извлекает отзывы, область которых совпадает с этой предоставленной областью. Обязательный. <br> Дополнительные возможности см [. в разделах Поддерживаемые запросы области для accessReviewHistoryDefinition](#supported-scope-queries-for-accessreviewhistorydefinition). |
| scheduleSettings  |[accessReviewHistoryScheduleSettings](../resources/accessReviewHistoryScheduleSettings.md)| Параметры для серии определений истории повторного просмотра доступа. Только если не определены **reviewHistoryPeriodStartDateTime** или **reviewHistoryPeriodEndDateTime** .|

### <a name="supported-scope-queries-for-accessreviewhistorydefinition"></a>Поддерживаемые запросы области для accessReviewHistoryDefinition

Свойство **областей** [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) основано на **ресурсе accessReviewQueryScope**, который позволяет настраивать различные ресурсы в свойстве **запроса.** Эти ресурсы затем представляют область определения истории и диктуют тип данных истории отзывов, включенных в загружаемый CSV-файл, который создается при создания [accessReviewHistoryInstances](../resources/accessreviewhistoryinstance.md) определения истории.

Используйте следующий формат для свойства **запроса** :

```http
/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '{object}')
```

Значение — `{object}` это один из ресурсов, которые можно настроить в **accessReviewScheduleDefinition**. Например, ниже приводится каждый результат проверки accessReviewScheduleDefinition для отдельных групп (и исключает определения, охватимые для всех Microsoft 365 групп с гостевых пользователей).

```http
/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups')
```

Дополнительные поддерживаемые значения см. в $filter [параметре запроса accessReviewScheduleDefinition](accessreviewset-list-definitions.md#use-the-filter-query-parameter).

## <a name="response"></a>Отклик

В случае успешной `201 Created` работы этот метод возвращает код отклика и [объект accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) в тексте ответа.

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
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/historyDefinitions
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
  "scheduleSettings": {
      "reportRange": "P1M",
      "recurrence": {
          "pattern": {
              "type": "monthly",
              "interval": 1
          },
          "range": {
              "type": "noEnd",
              "startDate": "2018-08-03T21:02:30.667Z",
              "count": 0
          }
        }
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
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accessreviewhistorydefinition-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accessreviewhistorydefinition-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accessreviewhistorydefinition-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-accessreviewhistorydefinition-from--go-snippets.md)]
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
    "scheduleSettings": {
        "reportRange": "P1M",
        "recurrence": {
            "pattern": {
                "type": "monthly",
                "interval": 1
            },
            "range": {
                "type": "noEnd",
                "startDate": "2018-08-03T21:02:30.667Z",
                "count": 0
            }
        }
    },
    "decisions": [
        "approve",
        "deny",
        "dontKnow",
        "notReviewed",
        "notNotified"
    ],
    "status": "requested",
    "createdDateTime": "2021-04-14T00:22:48.9392594Z",
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
