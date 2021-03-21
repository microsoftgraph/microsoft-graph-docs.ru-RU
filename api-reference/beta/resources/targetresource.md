---
title: тип сложного типа ресурсов targetResource — API Microsoft Graph
description: Определяет сложный тип API microsoft Graph, который поддерживает деятельность организации (клиента) по отчету о журнале аудита.
author: cloudhandler
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-access-reports
ms.openlocfilehash: 12030bdb5c51e41e821218e3db67c4878a90c53d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954960"
---
# <a name="targetresource-resource-type"></a>тип ресурса targetResource

Пространство имен: microsoft.graph

Представляет целевые типы ресурсов, связанные с деятельностью аудита. 


## <a name="properties"></a>Свойства

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|Строка|Указывает уникальный ID ресурса.|
|displayName|Строка|Указывает видимое имя, определенное для ресурса. Обычно указывается, когда создается ресурс.|
|type|Строка|Описывает тип ресурса.  Примеры значений включают `Application` `Group` , и `ServicePrincipal` `User` .|
|userPrincipalName|String|При **наборе** типа включается имя пользователя, которое `User` инициировало действие; для других `null` типов.|
|groupType|groupType|При **наборе** типа указывается тип `Group` группы.  Возможные значения: `unifiedGroups` `azureAD` , и `unknownFutureValue`|
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


