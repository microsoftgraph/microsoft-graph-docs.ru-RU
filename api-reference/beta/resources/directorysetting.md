---
title: Тип ресурса directorySetting
description: Параметры каталога можно основанного на доступные directorySettingTemplates и изменено с предварительно значения по умолчанию. Эти параметры можно управлять сущности или функцию поведения, как на уровне клиента, так и на уровне определенной сущности. Если же параметр определен на уровне всей клиента и определенных сущностей, параметр уровня определенной сущности может отказаться от клиента по умолчанию.  Например клиента по умолчанию может разрешить Гости планируемой с существующих членов группы, но параметр конкретную группу может отказаться и запретить гостевым планируемой членами группы. В настоящее время системных параметров являются только влияет на поведение группы Office.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b489bf1130bd91d28b3a2b41a78c38b881e90d27
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521371"
---
# <a name="directorysetting-resource-type"></a>Тип ресурса directorySetting

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Параметры каталога можно основанного на доступные [directorySettingTemplates](directorysettingtemplate.md)и изменено с предварительно значения по умолчанию. Эти параметры можно управлять сущности или функцию поведения, как на уровне клиента, так и на уровне определенной сущности. Если же параметр определен на уровне всей клиента и определенных сущностей, параметр уровня определенной сущности может отказаться от клиента по умолчанию.  Например клиента по умолчанию может разрешить Гости планируемой с существующих членов группы, но параметр конкретную группу может отказаться и запретить гостевым планируемой членами группы. В настоящее время системных параметров являются только влияет на поведение группы Office.

> **Примечание**: версия /beta типа ресурса directorySetting применяется только к группам. Версия /v1.0 переименовано в groupSetting.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Создание параметра](../api/directorysetting-post-settings.md) | [directorySetting](directorysetting.md) |Создание объекта setting на основе directorySettingTemplate. POST-запрос должен предоставлять объекты settingValue для всех параметров, определенных в шаблоне.|
|[Получение параметра](../api/directorysetting-get.md) | [directorySetting](directorysetting.md) |Считывание свойств определенного объекта setting.|
|[Перечисление параметров](../api/directorysetting-list.md) | Коллекция [directorySetting](directorysetting.md) |Перечисление свойств всех объектов setting.|
|[Обновление параметра](../api/directorysetting-update.md) | [directorySetting](directorysetting.md)  |Обновление объекта setting. Можно изменить только settingValues в обновление.|
|[Удаление параметра](../api/directorysetting-delete.md) | Нет |Удаление объекта параметра. |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|displayName|строка|Отображаемое имя этой группы параметров, которое получено с использованием связанного шаблона. Только для чтения.|
|id|string| Уникальный идентификатор этих параметров. Только для чтения.|
|templateId|string| Уникальный идентификатор шаблона, который использовался для создания этой группы параметров. Только для чтения.|
|values|Коллекция объектов [settingValue](settingvalue.md)| Коллекция пар "имя-значение". Должно содержать и задавать все параметры, определенные в шаблоне.|

## <a name="relationships"></a>Отношения
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
  "suppressions": [
    "Error: /api-reference/beta/resources/directorysetting.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
