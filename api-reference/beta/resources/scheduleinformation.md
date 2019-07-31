---
title: Тип ресурса Счедулеинформатион
description: 'Представляет доступность пользователя, списка рассылки или ресурса за указанный период времени. '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-teams
author: ''
ms.openlocfilehash: 3d6ede4e1085a8be3f78b714f690b79b836abbcb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965322"
---
# <a name="scheduleinformation-resource-type"></a>Тип ресурса Счедулеинформатион

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Представляет доступность пользователя, списка рассылки или ресурса (помещения или оборудования) за указанный период времени.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|Аваилабилитивиев |String |Представляет объединенное представление доступности всех элементов в `scheduleItems`. Представление состоит из временных слотов. Доступность во время каждого временного слота указывается следующим `0`образом: = `1`Free, = `2`под вопросом, `3`= занят, = нет `4`на месте, Рабочий процесс.|
|error |[Фрибусеррор](freebusyerror.md) |Сведения об ошибке при попытке получить сведения о доступности пользователя, списка рассылки или ресурса. |
|Счедулеид |String |SMTP-адрес пользователя, списка рассылки или ресурса, определяющего экземпляр **счедулеинформатион**. |
|Счедулеитемс |Коллекция [счедулеитем](scheduleitem.md) |Содержит элементы, описывающие доступность пользователя или ресурса. |
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
  "tocPath": "",
  "suppressions": []
}
-->
