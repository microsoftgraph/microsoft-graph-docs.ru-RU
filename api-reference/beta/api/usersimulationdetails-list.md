---
title: Список пользователей моделирования
description: Список пользователей клиента в кампании моделирования атак с их действиями в Интернете.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: ecb3bcc46b57cbd6b5afd3f0f698fba3da5ef436
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996672"
---
# <a name="list-simulationusers"></a>Списки simulationUsers
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Список пользователей клиента и его действий в интернете в кампании моделирования атак.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | SecurityEvents.Read.All                     |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                              |
| Для приложений                            | SecurityEvents.Read.All                     |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /security/attackSimulation/simulations/{id}/report/simulationUsers
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает следующие параметры запроса OData, чтобы помочь настроить ответ: `$count` `$skiptoken` , , `$top` .

Используйте `@odata.nextLink` для pagination.

Ниже приводится пример их использования:

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /security/attackSimulation/simulations/{id}/report/simulationUsers?$top=1
GET /security/attackSimulation/simulations/{id}/report/simulationUsers?$count=true
```

Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и коллекцию `200 OK` [объектов userSimulationDetails](../resources/usersimulationdetails.md) в теле ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_usersimulationdetails"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/attackSimulation/simulations/{id}/report/simulationUsers
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-usersimulationdetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-usersimulationdetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-usersimulationdetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-usersimulationdetails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.userSimulationDetails)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "isCompromised": true,
      "compromisedDateTime": "2021-01-01T01:02:01.01Z",
      "simulationEvents": [
        {
          "eventName": "SuccessfullyDeliveredEmail",
          "eventDateTime": "2021-01-01T01:01:01.01Z",
          "ipAddress": "100.200.100.200",
          "osPlatformDeviceDetails": "Sample OS",
          "browser": "Sample Browser"
        },
        {
          "eventName": "EmailLinkClicked",
          "eventDateTime": "2021-01-01T01:02:01.01Z",
          "ipAddress": "100.200.100.200",
          "osPlatformDeviceDetails": "Sample OS",
          "browser": "Sample Browser"
        }
      ],
      "trainingEvents": [
        {
          "displayName": "Sample Training",
          "latestTrainingStatus": "assigned",
          "trainingAssignedProperties": {
            "contentDateTime": "2021-01-01T01:03:01.01Z",
            "ipAddress": "100.200.100.200",
            "osPlatformDeviceDetails": "Sample OS",
            "browser": "Sample Browser",
            "potentialScoreImpact": 5.0
          },
          "trainingUpdatedProperties": {
            "contentDateTime": "2021-01-01T01:04:01.01Z",
            "ipAddress": "100.200.100.201",
            "osPlatformDeviceDetails": "Sample OS-2",
            "browser": "Sample Browser",
            "potentialScoreImpact": 5.0
          },
          "trainingCompletedProperties": {
            "contentDateTime": "2021-01-01T01:05:01.01Z",
            "ipAddress": "100.200.100.202",
            "osPlatformDeviceDetails": "Sample OS",
            "browser": "Sample Browser-2",
            "potentialScoreImpact": 5.0
          }
        }
      ],
      "assignedTrainingsCount": 1,
      "completedTrainingsCount": 0,
      "inProgressTrainingsCount": 0,
      "reportedPhishDateTime": "2021-01-01T01:01:01.01Z",
      "simulationUser": {
        "userId": "99af58b9-ef1a-412b-a581-cb42fe8c8e21",
        "displayName": "Sample User",
        "email": "sampleuser@contoso.com"
      }
    }
  ]
}
```

