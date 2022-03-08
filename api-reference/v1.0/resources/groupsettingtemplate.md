---
title: тип ресурса groupSettingTemplate
description: Шаблоны параметров группы представляют параметры, определяемые системой, доступные для клиента.
ms.localizationpriority: medium
author: Jordanndahl
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 6da14127e3253b9f23b75997cb0e73cc5b05deb4
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63333892"
---
# <a name="groupsettingtemplate-resource-type"></a>тип ресурса groupSettingTemplate

Пространство имен: microsoft.graph

Шаблоны параметров группы представляют параметры, определяемые системой, доступные для клиента. [Параметры группы](groupsetting.md) могут быть созданы на основе доступных **группSettingTemplates**, а значения изменены по заранее. Шаблоны параметров группы не могут быть созданы, обновлены или удалены. Эти параметры могут представлять параметры для клиента или представлять определенные параметры группы. В настоящее время только шаблоны, доступные для групп, применяются к Microsoft 365 группам и включают параметры, например, могут ли пользователи создавать группы или приглашать гостей из-за пределов организации в члены группы.

Дополнительные сведения о доступных Microsoft 365 группах см. в [параметрах Template](/azure/active-directory/enterprise-users/groups-settings-cmdlets).

> [!TIP]
> Версия `/beta` этого ресурса называется [directorySettingTemplate](/graph/api/resources/directorysettingtemplate?view=graph-rest-beta&preserve-view=true).

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
|[Get groupSettingTemplate](../api/groupsettingtemplate-get.md) | [groupSettingTemplate](groupsettingtemplate.md) | Ознакомьтесь с определенными свойствами одного из системных объектов groupSettingTemplate. |
|[List groupSettingTemplate](../api/groupsettingtemplate-list.md) | [Коллекция groupSettingTemplate](groupsettingtemplate.md) |Список всех системных объектов groupSettingTemplate.|

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|description|String| Описание шаблона. |
|displayName|Строка| Отображение имени шаблона. Названный шаблон `Group.Unified` можно использовать для настройки параметров Microsoft 365 групп, `Group.Unified.Guest` а названный шаблон можно использовать для настройки параметров, определенных для группы.|
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

