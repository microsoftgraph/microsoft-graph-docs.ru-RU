---
title: Тип ресурса cloudAppSecurityState
description: Содержит информацию о состояниях об облачных приложений (destinationServiceName, destinationServiceIp).
localization_priority: Normal
ms.openlocfilehash: ff76adf1d3879c3dac3f19ae122d82c9523d5193
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876806"
---
# <a name="cloudappsecuritystate-resource-type"></a>Тип ресурса cloudAppSecurityState

Содержит информацию о состояниях об облачных приложений (destinationServiceName, destinationServiceIp).

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|destinationServiceIp|Строка|Конечный IP-адрес подключения для облачных приложений и служб.|
|destinationServiceName|Строка|Имя облачных приложений и служб (например «Salesforce», «Общего банка данных», и т.д.).|
|riskScore|Строка|Оценка риска поставщика создается/вычисляемые из облачных приложений и служб. Рекомендуемое значение диапазона 0-1, который соответствует в процентах.|

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
