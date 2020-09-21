---
title: Тип ресурса Счедулеинформатион
description: Представляет доступность пользователя, списка рассылки или ресурса за указанный период времени.
localization_priority: Normal
author: harini84
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 6c9196cccf4c1c0ae8bb5122f56f6576528f0345
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48077648"
---
# <a name="scheduleinformation-resource-type"></a>Тип ресурса Счедулеинформатион

Пространство имен: microsoft.graph

Представляет доступность пользователя, списка рассылки или ресурса (помещения или оборудования) за указанный период времени.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|аваилабилитивиев |Строка |Представляет объединенное представление доступности всех элементов в `scheduleItems` . Представление состоит из временных слотов. Доступность во время каждого временного слота указывается следующим образом: `0` = Free, `1` = под вопросом, `2` = занят, `3` = нет на месте, `4` Рабочий процесс.|
|error |[фрибусеррор](freebusyerror.md) |Сведения об ошибке при попытке получить сведения о доступности пользователя, списка рассылки или ресурса. |
|счедулеид |Строка |SMTP-адрес пользователя, списка рассылки или ресурса, определяющего экземпляр **счедулеинформатион**. |
|счедулеитемс |Коллекция [счедулеитем](scheduleitem.md) |Содержит элементы, описывающие доступность пользователя или ресурса. |
|workingHours |[workingHours](workinghours.md) |Дни недели и часы работы пользователя в определенном часовом поясе. Они задаются как часть [mailboxSettings](mailboxsettings.md)пользователя.|


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scheduleInformation"
}-->

```json
{
  "availabilityView": "String",
  "error": {"@odata.type": "microsoft.graph.freeBusyError"},
  "scheduleId": "String",
  "scheduleItems": [{"@odata.type": "microsoft.graph.scheduleItem"}],
  "workingHours": {"@odata.type": "microsoft.graph.workingHours"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "scheduleInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->

