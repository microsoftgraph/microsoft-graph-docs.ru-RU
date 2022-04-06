---
title: Моделирование спискаАтомации
description: Получите список автоматизации моделирования атак для клиента.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 13bdd574c1b783992b27144ded3ab3a31f2da5a7
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2022
ms.locfileid: "63758339"
---
# <a name="list-simulationautomations"></a>Моделирование спискаАтомации
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите список автоматизации моделирования атак для клиента.

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
GET /security/attackSimulation/simulationAutomations
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает параметры `$count`запросов , `$filter`, `$orderby`, , `$skip`и `$select` `$top`[OData](/graph/query-parameters), чтобы помочь настроить ответ. Параметры и параметры `$filter` `$orderby` запроса можно использовать в **свойствах displayName** и **status** .

Если набор результатов охватывает несколько страниц, `@odata.nextLink` тело ответа содержит набор ответов, который можно использовать для страницы с помощью набора результатов.

Ниже приводится пример их использования:

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /security/attackSimulation/simulationAutomations?$count=true
GET /security/attackSimulation/simulationAutomations?$filter={property} eq '{property-value}'
GET /security/attackSimulation/simulationAutomations?$filter={property} eq '{property-value}'&$top=5
GET /security/attackSimulation/simulationAutomations?$orderby={property}
GET /security/attackSimulation/simulationAutomations?$skip={skipCount}
GET /security/attackSimulation/simulationAutomations?$top=1
GET /security/attackSimulation/simulationAutomations?$select={property}
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код `200 OK` ответа и коллекцию объектов [simulationAutomation](../resources/simulationautomation.md) в тексте ответа.

## <a name="examples"></a>Примеры

Ниже приведен пример запроса.

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "list_simulationautomation"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/attackSimulation/simulationAutomations
```


### <a name="response"></a>Отклик

Ниже приведен пример ответа.

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.simulationAutomation)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.simulationAutomation",
      "id": "fbad62b0-b32d-b6ac-9f48-d84bbea08f96",
      "displayName": "Reed Flores",
      "description": "Sample Simulation Automation Description",
      "status": "running",
      "createdDateTime": "2022-01-01T01:01:01.01Z",
      "createdBy": {
        "id": "99af58b9-ef1a-412b-a581-cb42fe8c8e21",
        "displayName": "Reed Flores",
        "email": "reed@contoso.com"
      },
      "lastModifiedDateTime": "2022-01-01T01:01:01.01Z",
      "lastModifiedBy": {
        "id": "99af58b9-ef1a-412b-a581-cb42fe8c8e21",
        "displayName": "Reed Flores",
        "email": "reed@contoso.com"
      },
      "lastRunDateTime": "2022-01-01T01:01:01.01Z",
      "nextRunDateTime": "2022-01-01T01:01:01.01Z"
    }
  ]
}
```

