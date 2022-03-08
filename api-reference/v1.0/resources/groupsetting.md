---
title: тип ресурса groupSetting
description: Параметры группы определяют конфигурации, которые можно использовать для настройки ограничений, определенных для клиента и объектов, и разрешенного поведения. Например, можно заблокировать списки слов для имен отображения групп или определить, разрешено ли гостю быть владельцами групп.
author: Jordanndahl
ms.localizationpriority: medium
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 17e535c8584d6e9364257220eadc1aebba9c540b
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337434"
---
# <a name="groupsetting-resource-type"></a>тип ресурса groupSetting

Пространство имен: microsoft.graph

Параметры группы определяют конфигурации, которые можно использовать для настройки ограничений, определенных для клиента и объектов, и разрешенного поведения. Например, можно заблокировать списки слов для имен отображения групп или определить, разрешено ли гостю быть владельцами групп.

По умолчанию все группы наследуют предустановленные по умолчанию. Чтобы изменить параметры по умолчанию, необходимо создать новый объект параметров с помощью [groupSettingTemplates](groupsettingtemplate.md). Если один и тот же параметр определяется как для клиента, так и для определенной группы, параметр группового уровня переопределяет параметр на уровне клиента. Например, параметр для клиента может разрешить приглашать гостей существующими членами групп, но отдельные параметры группы могут переопределять и не разрешая приглашать гостей членами группы.

Параметры группы применяются только к Microsoft 365 группам.

> [!TIP]
> Версия `/beta` этого ресурса называется [directorySetting](/graph/api/resources/directorysetting?view=graph-rest-beta&preserve-view=true).

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
|[Создание параметра](../api/group-post-settings.md) | [groupSetting](groupsetting.md) |Создание объекта настройки на основе **groupSettingTemplate**.|
|[Получение параметра](../api/groupsetting-get.md) | [groupSetting](groupsetting.md) | Считывание свойств определенного объекта setting. |
|[Перечисление параметров](../api/group-list-settings.md) | Коллекция объектов [groupSetting](groupsetting.md) | Перечисление свойств всех объектов setting. |
|[Обновление параметра](../api/groupsetting-update.md) | [groupSetting](groupsetting.md) | Обновление объекта groupsetting. |
|[Удаление параметра](../api/groupsetting-delete.md) | Нет | Удаление объекта setting. |

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|displayName|Строка| Отображение имени этой группы параметров, которое происходит из связанного шаблона. |
|id|String| Уникальный идентификатор для этих параметров. Только для чтения. |
|templateId|Строка| Уникальный идентификатор для объекта [groupSettingTemplates](groupsettingtemplate.md) на уровне клиента, который был настроен для этого объекта параметров группового уровня. Только для чтения. |
|values|[settingValue](settingvalue.md) collection| Коллекция пар имен и значений, соответствующих свойствам **name** и **defaultValue** в объекте [referenced groupSettingTemplates](groupsettingtemplate.md) . |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.groupSetting"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)",
  "templateId": "String",
  "values": [{"@odata.type": "microsoft.graph.settingValue"}]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupSetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

