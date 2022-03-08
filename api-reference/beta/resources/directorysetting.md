---
title: тип ресурса directorySetting
description: Параметры каталога можно создать на основе доступных directorySettingTemplates и изменить их по умолчанию.
ms.localizationpriority: medium
author: dkershaw10
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: eb442e80e92b746e864507536b0e0b0992e8cd9a
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335278"
---
# <a name="directorysetting-resource-type"></a>тип ресурса directorySetting

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Параметры каталога определяют конфигурации, которые можно использовать для настройки ограничений, определенных для клиента и объектов, и допустимого поведения. Например, можно заблокировать списки слов для имен отображения групп или определить, разрешено ли гостю быть владельцами групп.

По умолчанию все сущности наследуют предустановленные по умолчанию. Чтобы изменить параметры по умолчанию, необходимо создать новый объект параметров с помощью [directorySettingTemplates](directorysettingtemplate.md). Если один и тот же параметр определяется как для клиента, так и для определенной группы, параметр на уровне сущности переопределяет параметр на уровне клиента. Например, параметр для клиента может разрешить приглашать гостей существующими членами групп, но отдельные параметры группы могут переопределять и не разрешая приглашать гостей членами группы.

> [!TIP]
> Версия `/v1.0` этого ресурса называется [groupSetting](/graph/api/resources/groupsetting?view=graph-rest-1.0&preserve-view=true).

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Создание параметра](../api/group-post-settings.md) | [directorySetting](directorysetting.md) |Создание объекта настройки на основе directorySettingTemplate.|
|[Получение параметра](../api/directorysetting-get.md) | [directorySetting](directorysetting.md) |Считывание свойств определенного объекта setting.|
|[Перечисление параметров](../api/group-list-settings.md) | Коллекция [directorySetting](directorysetting.md) |Перечисление свойств всех объектов setting.|
|[Обновление параметра](../api/directorysetting-update.md) | [directorySetting](directorysetting.md)  |Обновление объекта setting. В обновлении можно изменить только параметрValues.|
|[Удаление параметра](../api/directorysetting-delete.md) | Нет |Удаление объекта setting. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|displayName|string|Отображение имени этой группы параметров, которое происходит из связанного шаблона. Только для чтения.|
|id|string| Уникальный идентификатор для этих параметров. Только для чтения.|
|templateId|string| Уникальный идентификатор для шаблона, используемого для создания этой группы параметров. Только для чтения.|
|values|[settingValue](settingvalue.md) collection| Коллекция пар имен и значений, соответствующих свойствам name и defaultValue в объекте [referenced directorySettingTemplates](directorysettingtemplate.md) .|

## <a name="relationships"></a>Связи
Нет


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directorySetting"
}-->

```json
{
  "displayName": "string",
  "id": "string (identifier)",
  "templateId": "string",
  "values": [{"@odata.type": "microsoft.graph.settingValue"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directorySetting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


