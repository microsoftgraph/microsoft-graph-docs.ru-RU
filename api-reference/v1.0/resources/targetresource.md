---
title: Тип ресурса targetResource
description: Представляет целевые типы ресурсов, связанные с действиями аудита.
localization_priority: Normal
author: dhanyahk
ms.prod: azure-ad
ms.openlocfilehash: 33a381d6088245be235f37549184183443fe3237
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629217"
---
# <a name="targetresource-resource-type"></a>Тип ресурса targetResource

Представляет целевые типы ресурсов, связанные с действиями аудита. 

## <a name="properties"></a>Свойства

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String|Указывает уникальный идентификатор ресурса.|
|displayName|Строка|Указывает отображаемое имя, заданное для ресурса. Обычно указывается при создании ресурса.|
|type|String|Описывает тип ресурса.  Примеры значений: `Application`, `Group` `ServicePrincipal`, и `User`.|
|userPrincipalName|String|Если **** для `User`параметра Type задано значение, включается имя пользователя, инициировавшего действие; `null` для других типов.|
|groupType|String|Если **** для `Group`параметра Type задано значение, это указывает тип группы.|
|modifiedProperties|Коллекция [модифиедпроперти](modifiedproperty.md)|Указывает имя, старое значение и новое значение каждого атрибута, который изменился. Значения свойств зависят от **типа**операции.|

## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResource"
}-->

```json
{
  "id": "String",
  "displayName": "String",
  "type": "String",
  "userPrincipalName": "String",
  "groupType": "String",
  "modifiedProperties": [{"@odata.type": "microsoft.graph.modifiedProperty"}]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
