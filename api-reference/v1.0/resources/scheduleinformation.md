---
title: тип ресурса scheduleInformation
description: Представляет доступность пользователя, списка рассылки или ресурса за определенный период времени.
localization_priority: Normal
author: harini84
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 67b7396cfebc19baa3771c2ec8d153950928288506cfc699851b891e15409a0f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54231483"
---
# <a name="scheduleinformation-resource-type"></a>тип ресурса scheduleInformation

Пространство имен: microsoft.graph

Представляет доступность пользователя, списка рассылки или ресурса (комнаты или оборудования) в течение определенного периода времени.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|availabilityView |String |Представляет собой объединенную точку зрения на доступность всех элементов `scheduleItems` в . Представление состоит из интервалов времени. Доступность в течение каждого интервала времени указывается с: `0` = бесплатно, = предварительный, = занят, = вне `1` `2` `3` офиса, `4` = работа в другом месте.|
|error |[freeBusyError](freebusyerror.md) |Сведения об ошибках при попытке получить доступность пользователя, списка рассылки или ресурса. |
|scheduleId |String |SMTP-адрес пользователя, списка рассылки или ресурса, определяющий экземпляр **scheduleInformation.** |
|scheduleItems |[коллекция scheduleItem](scheduleitem.md) |Содержит элементы, описывая доступность пользователя или ресурса. |
|workingHours |[workingHours](workinghours.md) |Дни недели и часы работы пользователя в определенном часовом поясе. Они устанавливаются в составе почтовых [ящиков пользователяSettings](mailboxsettings.md).|


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

