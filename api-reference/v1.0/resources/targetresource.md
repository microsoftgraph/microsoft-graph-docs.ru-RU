---
title: тип ресурса targetResource
description: Представляет целевые типы ресурсов, связанные с деятельностью аудита.
localization_priority: Normal
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 148591f603a45d0e8752e4af87beaabd39152fae
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961890"
---
# <a name="targetresource-resource-type"></a>тип ресурса targetResource

Пространство имен: microsoft.graph

Представляет целевые типы ресурсов, связанные с деятельностью аудита. 

## <a name="properties"></a>Свойства

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String|Указывает уникальный ID ресурса.|
|displayName|String|Указывает видимое имя, определенное для ресурса. Обычно указывается, когда создается ресурс.|
|type|String|Описывает тип ресурса.  Примеры значений включают `Application` `Group` , и `ServicePrincipal` `User` .|
|userPrincipalName|String|При **наборе** типа включается имя пользователя, которое `User` инициировало действие; для других `null` типов.|
|groupType|groupType|При **наборе** типа указывается тип `Group` группы. Возможные значения: `unifiedGroups` `azureAD` , и `unknownFutureValue`|
|modifiedProperties|[измененная коллекцияProperty](modifiedproperty.md)|Указывает имя, старое значение и новое значение каждого измененного атрибута. Значения свойств зависят от **типа операции.**|

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

