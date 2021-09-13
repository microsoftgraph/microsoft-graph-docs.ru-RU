---
title: тип ресурса targetResource
description: Представляет целевые типы ресурсов, связанные с деятельностью аудита.
ms.localizationpriority: medium
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 3c922888888971a6dc46ddddc88fbef4e77873a2
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59032106"
---
# <a name="targetresource-resource-type"></a>тип ресурса targetResource

Пространство имен: microsoft.graph

Представляет целевые типы ресурсов, связанные с деятельностью аудита. 

## <a name="properties"></a>Свойства

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|Строка|Указывает уникальный ID ресурса.|
|displayName|String|Указывает видимое имя, определенное для ресурса. Обычно указывается, когда создается ресурс.|
|type|Строка|Описывает тип ресурса.  Примеры значений включают `Application` `Group` , и `ServicePrincipal` `User` .|
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

