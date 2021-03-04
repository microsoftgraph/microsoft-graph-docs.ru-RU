---
title: тип ресурса directorySettingTemplate
description: Шаблоны параметров каталогов представляют параметры, определяемые системой, доступные для клиента.
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 71984d472aab9f78197134fae0668fd0a90d7716
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440411"
---
# <a name="directorysettingtemplate-resource-type"></a>тип ресурса directorySettingTemplate

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Шаблоны параметров каталогов представляют параметры, определяемые системой, доступные для клиента. [Параметры каталога](directorysetting.md) могут быть созданы на основе доступных directorySettingTemplates, а значения изменены по заранее. Шаблоны параметров каталога не могут быть созданы, обновлены или удалены. Эти параметры могут представлять параметры для клиента или представлять определенные параметры сущности.  В настоящее время только доступные шаблоны применяются к группам Office и включают параметры, например, могут ли пользователи создавать группы или приглашать гостей из-за пределов организации, чтобы стать членами группы.

> **Примечание.**/бета-версия типа ресурса directorySettingTemplate применяется только к группам. Версия /v1.0 переименована в groupSettingTemplate.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Get directorySettingTemplate](../api/directorysettingtemplate-get.md) | [directorySettingTemplate](directorysettingtemplate.md) |Ознакомьтесь с определенными свойствами одного из системных объектов directorySettingTemplate.|
|[Каталог listSettingTemplate](../api/directorysettingtemplate-list.md) | [Коллекция directorySettingTemplate](directorysettingtemplate.md) |Список всех системных объектов directorySettingTemplate.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|description|string|Описание шаблона. Только для чтения.|
|displayName|string|Отображение имени шаблона. Только для чтения. |
|id|string| Уникальный идентификатор шаблона. Только для чтения.|
|values|[settingTemplateValue](settingtemplatevalue.md) collection| Коллекция параметровTemplateValues, которые перечисляют набор доступных параметров, по умолчанию и типов, которые составляют этот шаблон.  Только для чтения. |

## <a name="relationships"></a>Связи
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
  "suppressions": []
}
-->


