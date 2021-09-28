---
title: Моделирование списка
description: Список имитаций атак клиента.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 6fc53a52fbd543fbdc9eeb6263d8c2fda1260f16
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979724"
---
# <a name="list-simulations"></a>Моделирование списка
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Список имитаций атак клиента.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | SecurityEvents.Read.All                     |
| Делегированное (личная учетная запись Майкрософт) | Не поддерживается.                              |
| Приложение                            | SecurityEvents.Read.All                     |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /security/attackSimulation/simulations
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает следующие параметры запроса OData, чтобы помочь настроить ответ: `$count` , , , , `$filter` `$orderby` `$skiptoken` `$top` .

Поддержка следующих свойств `$filter` `$orderby` и: **attackTechnique**, **attackType**, **completionDateTime**, **displayName**, **isAutomated,** **launchDateTime**, **режим**, **состояние**.

Используйте `@odata.nextLink` для pagination.

Ниже приводится пример их использования:

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /security/attackSimulation/simulations?$count=true
GET /security/attackSimulation/simulations?$filter={property} eq '{property-value}'
GET /security/attackSimulation/simulations?$filter={property} eq '{property-value}'&$top=5
GET /security/attackSimulation/simulations?$orderby={property}
GET /security/attackSimulation/simulations?$top=1
```

Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` моделирования в тексте [](../resources/simulation.md) отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "list_simulation"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/attackSimulation/simulations
```


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.simulation)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "f1b13829-3829-f1b1-2938-b1f12938b1f1",
      "displayName": "Sample Simulation",
      "description": "Sample Simulation Description",
      "attackType": "social",
      "attackTechnique": "credentialHarvesting",
      "status": "scheduled",
      "createdDateTime": "2021-01-01T01:01:01.01Z",
      "createdBy": {
        "id": "99af58b9-ef1a-412b-a581-cb42fe8c8e21",
        "displayName": "Sample User",
        "email": "sampleuser@contoso.com"
      },
      "lastModifiedDateTime": "2021-01-01T01:01:01.01Z",
      "lastModifiedBy": {
        "id": "99af58b9-ef1a-412b-a581-cb42fe8c8e21",
        "displayName": "Sample User",
        "email": "sampleuser@contoso.com"
      },
      "launchDateTime": "2021-01-01T02:01:01.01Z",
      "completionDateTime": "2021-01-07T01:01:01.01Z",
      "includeAllAccountTargets": false,
      "enableRegionTimezoneDelivery": false,
      "mode": "real",
      "isAutomated": false,
      "cleanupArtifacts": false,
      "payloadSource": "global",
      "payloadDeliveryPlatform": "email",
      "trainingAssignmentPreference": "manual",
      "trainingContentPreference": "microsoft",
      "trainingDueDateTime": "2021-01-31T01:01:01.01Z"
    }
  ]
}
```

