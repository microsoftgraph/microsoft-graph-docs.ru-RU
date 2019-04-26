---
title: Тип ресурса groupSettingTemplate
description: Шаблоны параметров групп представляют системные параметры, доступные для клиента. Параметры группы могут быть созданы на основе доступных **граупсеттингтемплатес**, а значения по умолчанию изменяются. Шаблоны параметров групп не могут быть созданы, обновлены или удалены. Эти параметры могут представлять параметры на уровне клиента или конкретные параметры группы. В настоящее время доступны только шаблоны Office 365, а также параметры, например, могут ли пользователи создавать группы или приглашать гостей извне организации для становиться членами группы.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2b9b95303b72bc111f045010e71459f541e9a9b8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570794"
---
# <a name="groupsettingtemplate-resource-type"></a>Тип ресурса groupSettingTemplate

Шаблоны параметров групп представляют системные параметры, доступные для клиента. [Параметры группы](groupsetting.md) могут быть созданы на основе доступных **граупсеттингтемплатес**, а значения по умолчанию изменяются. Шаблоны параметров групп не могут быть созданы, обновлены или удалены. Эти параметры могут представлять параметры на уровне клиента или конкретные параметры группы. В настоящее время доступны только шаблоны Office 365, а также параметры, например, могут ли пользователи создавать группы или приглашать гостей извне организации для становиться членами группы.

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
|[Получение groupSettingTemplate](../api/groupsettingtemplate-get.md) | [groupSettingTemplate](groupsettingtemplate.md) | Чтение определенных свойств одного из системных объектов groupSettingTemplate, определенных системой. |
|[Список groupSettingTemplate](../api/groupsettingtemplate-list.md) | [Коллекция groupSettingTemplate](groupsettingtemplate.md) |ПереЧисление всех объектов groupSettingTemplate, определенных системой.|

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|description|String| Описание шаблона. |
|displayName|String| Отображаемое имя шаблона. |
|id|Строка| Уникальный идентификатор шаблона. Только для чтения.|
|values|Коллекция [сеттингтемплатевалуе](settingtemplatevalue.md)| Коллекция Settingtemplatevalue, в которой перечислены набор доступных параметров, значения по умолчанию и типы, которые составляют этот шаблон. |

## <a name="relationships"></a>Связи

Отсутствуют.


## <a name="json-representation"></a>Представление JSON

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
