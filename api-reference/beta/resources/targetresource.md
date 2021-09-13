---
title: тип комплекса ресурсов targetResource — API Graph Microsoft
description: Определяет тип API Graph API для объекта targetResource, который поддерживает деятельность организации аудита (клиента) журналов аудита.
author: cloudhandler
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: identity-and-access-reports
ms.openlocfilehash: 566db033d6d62ac584ee2057f172d5330f12b8a3
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59053870"
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


