---
title: Выполняется список
description: Получите список запусков автоматизации моделирования атак для клиента.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 36f0a7375b1aafbaa5eed5ec44b8c47790c2bf0b
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2022
ms.locfileid: "63758333"
---
# <a name="list-runs"></a>Выполняется список
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите список запусков автоматизации моделирования атак для клиента.

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
GET /security/attackSimulation/simulationAutomations/{simulationAutomationId}/runs
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает параметры `$count`запросов , и `$select` `$skiptoken``$top`[OData](/graph/query-parameters), чтобы помочь настроить ответ.

Если набор результатов охватывает несколько страниц, `@odata.nextLink` тело ответа содержит набор ответов, который можно использовать для страницы с помощью набора результатов.

Ниже приводится пример их использования:

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /security/attackSimulation/simulationautomations/{simulationAutomationId}/runs?$count=true
GET /security/attackSimulation/simulationautomations/{simulationAutomationId}/runs?$skipToken={skipToken}
GET /security/attackSimulation/simulationautomations/{simulationAutomationId}/runs?$top=1
GET /security/attackSimulation/simulationautomations/{simulationAutomationId}/runs?$select={property}
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код `200 OK` ответа и коллекцию объектов [simulationAutomationRun](../resources/simulationautomationrun.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "list_simulationautomationrun"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/attackSimulation/simulationAutomations/fbad62b0-b32d-b6ac-9f48-d84bbea08f96/runs
```


### <a name="response"></a>Отклик

Ниже приведен пример ответа.

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.simulationAutomationRun",
  "isCollection": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.simulationAutomationRun",
      "id": "ac4936a5-3865-a0ec-7254-67a22f6121e2",
      "status": "succeeded",
      "startDateTime": "2021-01-01T02:01:01.01Z",
      "endDateTime": "2021-01-01T02:01:01.01Z",
      "simulationId": "bc4936a5-3865-a0ec-7254-67a22f6121e2"
    }
  ]
}
```

