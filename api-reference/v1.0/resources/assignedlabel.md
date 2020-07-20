---
title: Тип ресурса Ассигнедлабел
description: Представляет метку конфиденциальности, назначенную группе Microsoft 365.
localization_priority: Normal
author: krbain
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 2e527dbf8cc1dd42474bee467f5e1f9a0beca261
ms.sourcegitcommit: 566d09c17f9d641b6fac9b9159405a3cc41e037b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/20/2020
ms.locfileid: "45184014"
---
# <a name="assignedlabel-resource-type"></a>Тип ресурса Ассигнедлабел

Пространство имен: microsoft.graph

Представляет метку конфиденциальности, назначенную группе Microsoft 365. Метки конфиденциальности позволяют администраторам применять определенные параметры группы к группе, назначая классификацию группе (например, конфиденциальную, строго конфиденциальную или общую). Метки конфиденциальности публикуются администраторами в центре безопасности Microsoft 365 & соответствия требованиям в рамках возможностей защиты информации Майкрософт. Дополнительные сведения о метках конфиденциальности приведены в разделе [Обзор меток конфиденциальности](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels?view=o365-worldwide).

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