---
title: тип ресурса directorySetting
description: Параметры каталога можно создать на основе доступных directorySettingTemplates и изменить их по умолчанию.
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 50c73e9c68cd3d2fa3f4aed6c7eba84141443d1a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440453"
---
# <a name="directorysetting-resource-type"></a>тип ресурса directorySetting

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Параметры каталога могут быть созданы на основе доступных [directorySettingTemplates](directorysettingtemplate.md)и изменены по заранее. Эти параметры могут управлять поведением сущности или функций как на уровне клиента, так и на определенном уровне объекта. Если один и тот же параметр определяется как на уровне клиента, так и на уровне определенного объекта, определенный параметр уровня сущности может отказаться от параметра для всех клиентов.  Например, параметр для клиента может разрешить приглашать гостей существующими членами групп, но определенный параметр группы может отказаться и не разрешит приглашать гостей членами группы. В настоящее время параметры, определенные системой, регулируют только поведение групп Office.

> **Примечание.** Бета-версия типа ресурса directorySetting применяется только к группам. Версия /v1.0 переименована в groupSetting.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Создание параметра](../api/directorysetting-post-settings.md) | [directorySetting](directorysetting.md) |Создание объекта настройки на основе directorySettingTemplate. Запрос POST должен предоставить параметрValues для всех параметров, определенных в шаблоне.|
|[Получение параметра](../api/directorysetting-get.md) | [directorySetting](directorysetting.md) |Считывание свойств определенного объекта setting.|
|[Перечисление параметров](../api/directorysetting-list.md) | Коллекция [directorySetting](directorysetting.md) |Перечисление свойств всех объектов setting.|
|[Обновление параметра](../api/directorysetting-update.md) | [directorySetting](directorysetting.md)  |Обновление объекта setting. В обновлении можно изменить только параметрValues.|
|[Удаление параметра](../api/directorysetting-delete.md) | Нет |Удаление объекта параметра. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|displayName|string|Отображение имени этой группы параметров, которое происходит из связанного шаблона. Только для чтения.|
|id|string| Уникальный идентификатор для этих параметров. Только для чтения.|
|templateId|string| Уникальный идентификатор для шаблона, используемого для создания этой группы параметров. Только для чтения.|
|values|[settingValue](settingvalue.md) collection| Коллекция пар значений имен. Необходимо содержать и задать все параметры, определенные в шаблоне.|

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


