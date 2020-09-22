---
title: Тип ресурса Ассигнедлабел
description: Представляет метку конфиденциальности, назначенную группе Microsoft 365. Метки конфиденциальности позволяют администраторам применять определенные параметры группы к группе, назначая классификацию группе (например, конфиденциальную, строго конфиденциальную или общую).
localization_priority: Normal
author: krbain
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 8ef079363d4951f269ea509534cecd2e6ae2a0f9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050108"
---
# <a name="assignedlabel-resource-type"></a>Тип ресурса Ассигнедлабел

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет метку конфиденциальности, назначенную группе Microsoft 365. Метки конфиденциальности позволяют администраторам применять определенные параметры группы к группе, назначая классификацию группе (например, конфиденциальную, строго конфиденциальную или общую). Метки конфиденциальности публикуются администраторами в центре безопасности Microsoft 365 & соответствия требованиям в рамках возможностей защиты информации Майкрософт. Дополнительные сведения о метках конфиденциальности приведены в разделе [Обзор меток конфиденциальности](/Office365/SecurityCompliance/sensitivity-labels).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|лабелид|Строка|Уникальный идентификатор метки.|
|displayName|Строка|Отображаемое имя метки. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignedLabel"
}-->

```json
{
  "labelId": "String",
  "displayName": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "assignedLabel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


