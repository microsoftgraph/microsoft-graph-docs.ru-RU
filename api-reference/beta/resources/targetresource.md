---
title: сложный тип ресурса targetResource — API Microsoft Graph
description: Определяет сложный тип ресурса сущности targetResource API Microsoft Graph, который поддерживает действия Организации отчетности журнала аудита (клиента).
author: lleonard-msft
localization_priority: Normal
ms.prod: azure-ad
ms.openlocfilehash: a03ca03e0b7105c8f07347f6ed52aa322a6fd090
ms.sourcegitcommit: e8b488f8068845522b869bf97475da7b078bee3d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/01/2019
ms.locfileid: "30342291"
---
# <a name="targetresource-resource-type"></a>Тип ресурса targetResource

Представляет целевые типы ресурсов, связанные с действиями аудита. 


## <a name="properties"></a>Свойства

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String|Указывает уникальный идентификатор ресурса.|
|displayName|String|Указывает отображаемое имя, заданное для ресурса. Обычно указывается при создании ресурса.|
|type|String|Описывает тип ресурса.  Примеры значений: `Application`, `Group` `ServicePrincipal`, и `User`.|
|userPrincipalName|String|Если **** для `User`параметра Type задано значение, включается имя пользователя, инициировавшего действие; `null` для других типов.|
|groupType|String|Если **** для `Group`параметра Type задано значение, это указывает тип группы.|
|modifiedProperties|Коллекция [модифиедпроперти](modifiedproperty.md)|Указывает имя, старое значение и новое значение каждого атрибута, который изменился. Значения свойств зависят от **типа**операции.|

## <a name="json-representation"></a>Описание в формате JSON

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
