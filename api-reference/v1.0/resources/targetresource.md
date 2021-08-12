---
title: тип ресурса targetResource
description: Представляет целевые типы ресурсов, связанные с деятельностью аудита.
localization_priority: Normal
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 4a98ccc2bf577289e867345a256c737275a295ca0a7954d23138f1cb68d669bc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54222632"
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

