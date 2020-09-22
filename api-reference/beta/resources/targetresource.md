---
title: сложный тип ресурса targetResource — API Microsoft Graph
description: Определяет сложный тип ресурса сущности targetResource API Microsoft Graph, который поддерживает действия Организации отчетности журнала аудита (клиента).
author: cloudhandler
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bec25af7e0f39a4adf15577c21d4141e1a3c431a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985652"
---
# <a name="targetresource-resource-type"></a>Тип ресурса targetResource

Пространство имен: microsoft.graph

Представляет целевые типы ресурсов, связанные с действиями аудита. 


## <a name="properties"></a>Свойства

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String|Указывает уникальный идентификатор ресурса.|
|displayName|String|Указывает отображаемое имя, заданное для ресурса. Обычно указывается при создании ресурса.|
|type|String|Описывает тип ресурса.  Примеры значений: `Application` , `Group` , `ServicePrincipal` и `User` .|
|userPrincipalName|String|Если для параметра **Type** задано значение `User` , это имя пользователя, инициировавшего действие, `null` для других типов.|
|groupType|String|Если для параметра **Type** задано значение `Group` , это указывает тип группы.|
|modifiedProperties|Коллекция [модифиедпроперти](modifiedproperty.md)|Указывает имя, старое значение и новое значение каждого атрибута, который изменился. Значения свойств зависят от **типа**операции.|

## <a name="json-representation"></a>Представление JSON

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


