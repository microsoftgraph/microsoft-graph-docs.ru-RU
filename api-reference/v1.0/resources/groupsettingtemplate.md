---
title: Тип ресурса groupSettingTemplate
description: Шаблоны параметров групп представляют системные параметры, доступные для клиента. Параметры группы могут быть созданы на основе доступных **граупсеттингтемплатес**, а значения по умолчанию изменяются. Шаблоны параметров групп не могут быть созданы, обновлены или удалены. Эти параметры могут представлять параметры на уровне клиента или конкретные параметры группы. В настоящее время доступны только шаблоны Office 365, а также параметры, например, могут ли пользователи создавать группы или приглашать гостей извне организации для становиться членами группы.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3d0624be1511b542da08e76ed5f9c51e60fe58a1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029283"
---
# <a name="groupsettingtemplate-resource-type"></a>Тип ресурса groupSettingTemplate

Шаблоны параметров групп представляют системные параметры, доступные для клиента. [Параметры группы](groupsetting.md) могут быть созданы на основе доступных **граупсеттингтемплатес**, а значения по умолчанию изменяются. Шаблоны параметров групп не могут быть созданы, обновлены или удалены. Эти параметры могут представлять параметры на уровне клиента или конкретные параметры группы. В настоящее время доступны только шаблоны Office 365, а также параметры, например, могут ли пользователи создавать группы или приглашать гостей извне организации для становиться членами группы.

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
|[Получение groupSettingTemplate](../api/groupsettingtemplate-get.md) | [groupSettingTemplate](groupsettingtemplate.md) | Чтение определенных свойств одного из системных объектов groupSettingTemplate, определенных системой. |
|[Список groupSettingTemplate](../api/groupsettingtemplate-list.md) | [Коллекция groupSettingTemplate](groupsettingtemplate.md) |Перечисление всех объектов groupSettingTemplate, определенных системой.|

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|description|String| Описание шаблона. |
|displayName|Строка| Отображаемое имя шаблона. |
|id|String| Уникальный идентификатор шаблона. Только для чтения.|
|values|Коллекция [сеттингтемплатевалуе](settingtemplatevalue.md)| Коллекция Settingtemplatevalue, в которой перечислены набор доступных параметров, значения по умолчанию и типы, которые составляют этот шаблон. |

## <a name="relationships"></a>Отношения

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
