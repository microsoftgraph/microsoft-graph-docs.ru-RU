---
title: Создание historyDefinitions
description: Создайте объект accessReviewHistoryDefinition.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: ab8e755f918d35d59e06795f4c16a96de180a101
ms.sourcegitcommit: ca3edeed9408ee94bb12d7acf506d7317bf01d25
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2022
ms.locfileid: "64842325"
---
# <a name="create-historydefinitions"></a>Создание historyDefinitions

Пространство имен: microsoft.graph

Создайте объект [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) .

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись)|AccessReview.ReadWrite.All|
|Делегированное (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|AccessReview.ReadWrite.All|

Пользователь, выполнив вход, также должен иметь роль каталога, которая позволяет ему считывать проверку доступа для получения любых данных.  Дополнительные сведения см. в разделе о требованиях к роли и разрешениям для [проверок доступа](../resources/accessreviewsv2-overview.md).

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

В тексте запроса добавьте представление объекта [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) в формате JSON.

В следующей таблице показаны обязательные свойства, используемые для [создания объекта accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName | String  | Имя для сбора данных журнала проверки доступа. Обязательный. |
|reviewHistoryPeriodStartDateTime  | DateTimeOffset  | Метка времени. Проверки, начиная с этой даты или после нее, будут включены в извлеченные данные журнала. Требуется только в том случае, **если параметр scheduleSettings** не определен.  |
|reviewHistoryPeriodEndDateTime  | DateTimeOffset  | Метка времени. Проверки, начиная с этой даты или до этой даты, будут включены в извлеченные данные журнала. Требуется только в том случае, **если параметр scheduleSettings** не определен.  |
|scopes|[Коллекция accessReviewQueryScope](../resources/accessreviewqueryscope.md)| Используется для фильтрации проверок, включенных в извлеченные данные журнала. Извлекает проверки, область которых соответствует указанной области. Обязательный. <br> Дополнительные сведения см [. в разделе "Поддерживаемые запросы области для accessReviewHistoryDefinition"](#supported-scope-queries-for-accessreviewhistorydefinition). |
| scheduleSettings  |[accessReviewHistoryScheduleSettings](../resources/accessReviewHistoryScheduleSettings.md)| Параметры для серии определений журнала повторяющихся проверок доступа. Требуется только в том случае, если **параметр reviewHistoryPeriodStartDateTime** или **reviewHistoryPeriodEndDateTime** не определен. Пока не поддерживается.|

### <a name="supported-scope-queries-for-accessreviewhistorydefinition"></a>Поддерживаемые запросы области для accessReviewHistoryDefinition

Свойство **scopes** [объекта accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) основано на **ресурсе accessReviewQueryScope**, который позволяет настраивать различные ресурсы в свойстве **запроса.** Затем эти ресурсы представляют область определения журнала и определяют тип данных журнала проверки, включенных в скачиваемый CSV-файл, который создается при создании [объектов accessReviewHistoryInstance в](../resources/accessreviewhistoryinstance.md) определении журнала.

Используйте следующий формат для свойства **запроса** :

```http
/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '{object}')
```

Значение является одним `{object}` из ресурсов, которые можно настроить в **accessReviewScheduleDefinition**. Например, ниже приводится каждый результат проверки accessReviewScheduleDefinition для отдельных групп (и исключаются определения, область действия для всех Microsoft 365 групп с гостевыми пользователями).

```http
/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups')
```

Дополнительные сведения о поддерживаемых значениях см. в $filter [параметра запроса в accessReviewScheduleDefinition](accessreviewset-list-definitions.md#use-the-filter-query-parameter).

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод возвращает код `201 Created` отклика и объект [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) в теле отклика.

## <a name="examples"></a>Примеры

В следующем примере показано, как создать определение журнала проверки доступа с областью действия проверки доступа для пакетов и групп доступа, выполняемых с 01.01.2021 до 05.04.2021.

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
