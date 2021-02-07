---
title: Тип ресурса targetResource
description: Представляет целевые типы ресурсов, связанные с действиями аудита.
localization_priority: Normal
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 66470d9e29bad5c662bfa6aa3227091b2ec739bc
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130152"
---
# <a name="targetresource-resource-type"></a>Тип ресурса targetResource

Пространство имен: microsoft.graph

Представляет целевые типы ресурсов, связанные с действиями аудита. 

## <a name="properties"></a>Свойства

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String|Указывает уникальный ИД ресурса.|
|displayName|String|Указывает видимое имя, определенное для ресурса. Обычно указывается, когда создается ресурс.|
|type|String|Описывает тип ресурса.  Примеры значений: `Application` , `Group` , и `ServicePrincipal` `User` .|
|userPrincipalName|String|Если **за** установлен тип, это включает имя пользователя, инициа которого было инициировано действие; для `User` других `null` типов.|
|groupType|String|Если **за** установлен `Group` тип, это указывает на тип группы.|
|modifiedProperties|[Коллекция modifiedProperty](modifiedproperty.md)|Указывает имя, старое значение и новое значение каждого из измененных атрибутов. Значения свойств зависят от типа **операции.**|

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

