---
title: Тип ресурса directorySettingTemplate
description: Шаблоны параметр Directory представляют системные параметры, доступные для клиента. Параметры каталога могут создаваться на основе доступных directorySettingTemplates и значения, измененные из предварительно значения по умолчанию. Шаблоны параметр каталога не создан, обновлении или удалении. Эти параметры можно представить параметры на уровне клиента или может представлять параметров определенной сущности.  На данный момент доступны только шаблоны применяются к группам Office и включают параметры, такие как пользователи могут создавать группы или пригласить Гости из за пределами организации стать членам группы.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 366817df422686a8db658f1cab1d5805c24c4f91
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516660"
---
# <a name="directorysettingtemplate-resource-type"></a>Тип ресурса directorySettingTemplate

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Шаблоны параметр Directory представляют системные параметры, доступные для клиента. [Параметры каталога](directorysetting.md) могут создаваться на основе доступных directorySettingTemplates и значения, измененные из предварительно значения по умолчанию. Шаблоны параметр каталога не создан, обновлении или удалении. Эти параметры можно представить параметры на уровне клиента или может представлять параметров определенной сущности.  На данный момент доступны только шаблоны применяются к группам Office и включают параметры, такие как пользователи могут создавать группы или пригласить Гости из за пределами организации стать членам группы.

> **Примечание**: версия /beta типа ресурса directorySettingTemplate применяется только к группам. Версия /v1.0 переименовано в groupSettingTemplate.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение directorySettingTemplate](../api/directorysettingtemplate-get.md) | [directorySettingTemplate](directorysettingtemplate.md) |Чтение определенных свойств объекта directorySettingTemplate определения системы.|
|[Список directorySettingTemplate](../api/directorysettingtemplate-list.md) | [Коллекция directorySettingTemplate](directorysettingtemplate.md) |Список всех системных объектов directorySettingTemplate.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|description|строка|Описание шаблона. Только для чтения.|
|displayName|string|Отображаемое имя шаблона. Только для чтения. |
|id|string| Уникальный идентификатор шаблона. Только для чтения.|
|values|Коллекция объектов [settingTemplateValue](settingtemplatevalue.md)| Коллекция объектов settingTemplateValue, перечисляющих набор доступных параметров, значений по умолчанию и типов, которые составляют шаблон.  Только для чтения. |

## <a name="relationships"></a>Отношения
Нет


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directorySettingTemplate"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
  "values": [{"@odata.type": "microsoft.graph.settingTemplateValue"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directorySettingTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/directorysettingtemplate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
