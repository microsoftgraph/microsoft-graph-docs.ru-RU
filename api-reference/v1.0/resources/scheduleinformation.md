---
title: Тип ресурса Счедулеинформатион
description: Представляет доступность пользователя, списка рассылки или ресурса за указанный период времени.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 2767f4d289b4ffb0b4be6001a3a28ee0727c33dc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533813"
---
# <a name="scheduleinformation-resource-type"></a>Тип ресурса Счедулеинформатион

Пространство имен: microsoft.graph

Представляет доступность пользователя, списка рассылки или ресурса (помещения или оборудования) за указанный период времени.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|аваилабилитивиев |Строка |Представляет объединенное представление доступности всех элементов в `scheduleItems`. Представление состоит из временных слотов. Доступность во время каждого временного слота указывается следующим `0`образом: = `1`Free, = `2`под вопросом, `3`= занят, = нет `4`на месте, Рабочий процесс.|
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
