---
title: тип ресурса groupSettingTemplate
description: Шаблоны параметров группы представляют параметры, определяемые системой, доступные для клиента.
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: a7868538c13b1e386e7aa10dcdf3fed9c03b198f
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680873"
---
# <a name="groupsettingtemplate-resource-type"></a>тип ресурса groupSettingTemplate

Пространство имен: microsoft.graph

Шаблоны параметров группы представляют параметры, определяемые системой, доступные для клиента. [Параметры группы](groupsetting.md) могут быть созданы на основе доступных **группSettingTemplates** и значений, измененных по заранее. Шаблоны параметров группы не могут быть созданы, обновлены или удалены. Эти параметры могут представлять параметры для клиента или представлять определенные параметры группы. В настоящее время только доступные шаблоны применяются к Microsoft 365 группам и включают параметры, например, могут ли пользователи создавать группы или приглашать гостей из-за пределов организации в члены группы.

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
|[Get groupSettingTemplate](../api/groupsettingtemplate-get.md) | [groupSettingTemplate](groupsettingtemplate.md) | Ознакомьтесь с определенными свойствами одного из системных объектов groupSettingTemplate. |
|[List groupSettingTemplate](../api/groupsettingtemplate-list.md) | [Коллекция groupSettingTemplate](groupsettingtemplate.md) |Список всех системных объектов groupSettingTemplate.|

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|description|String| Описание шаблона. |
|displayName|String| Отображение имени шаблона. |
|id|String| Уникальный идентификатор шаблона. Только для чтения.|
|values|[settingTemplateValue](settingtemplatevalue.md) collection| Коллекция параметровTemplateValues, которые перечисляют набор доступных параметров, по умолчанию и типов, которые составляют этот шаблон. |

## <a name="relationships"></a>Связи

Отсутствуют.


## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.groupSettingTemplate"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "values": [{"@odata.type": "microsoft.graph.settingTemplateValue"}]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupSettingTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

