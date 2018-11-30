---
title: Тип ресурса cloudAppSecurityState
description: Содержит информацию о состояниях об облачных приложений (destinationServiceName, destinationServiceIp).
ms.openlocfilehash: 915044c3084e3d9a9435d602ecc7ec809d2168f2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079236"
---
# <a name="cloudappsecuritystate-resource-type"></a>Тип ресурса cloudAppSecurityState

Содержит информацию о состояниях об облачных приложений (destinationServiceName, destinationServiceIp).

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Description |
|:-------------|:------------|:------------|
|destinationServiceIp|String|Конечный IP-адрес подключения для облачных приложений и служб.|
|destinationServiceName|String|Имя облачных приложений и служб (например «Salesforce», «Общего банка данных», и т.д.).|
|riskScore|String|Оценка риска поставщика создается/вычисляемые из облачных приложений и служб. Рекомендуемое значение диапазона 0-1, который соответствует в процентах.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.cloudAppSecurityState"
}-->

```json
{
  "destinationServiceIp": "String",
  "destinationServiceName": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "cloudAppSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->