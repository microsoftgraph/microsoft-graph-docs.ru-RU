---
title: сложный тип ресурса targetResource — API Microsoft Graph
description: Определяет сложный тип ресурса сущности targetResource API Microsoft Graph, который поддерживает действия Организации отчетности журнала аудита (клиента).
author: davidmu1
localization_priority: Normal
ms.prod: azure-ad
ms.openlocfilehash: 0a52a8586d8bce211729b8dffe2a43129b94b30d
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657653"
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
