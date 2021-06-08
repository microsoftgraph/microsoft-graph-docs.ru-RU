---
title: Тип ресурса timecard
description: Запись в расписании.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 25818e091ac2d4f6590fd7ea2c395752d0238bd0
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786412"
---
# <a name="timecard-resource-type"></a>Тип ресурса timecard

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет запись химкарта в расписании.

## <a name="methods"></a>Методы

| Метод       | Тип возвращаемых данных  |Описание|
|:---------------|:--------|:----------|
|[Список](../api/timecard-list.md) | [коллекция timeCard](timecard.md) | Получите список объектов **timecard** в этом расписании.|
|[Создание](../api/timecard-post.md) | [timeCard](timecard.md) | Создайте новый **объект timecard.**|
|[получение](../api/timecard-get.md); | [timeCard](timecard.md) | Получите **объект timecard** по ID.|
|[Replace](../api/timecard-replace.md) | Нет | Замените **объект timecard.**|
|[Delete](../api/timecard-delete.md) | Нет | Удаление объекта **timecard** из расписания.|
|[clockIn](../api/timecard-clockin.md) | [timeCard](timecard.md) | Часы, чтобы запустить **хронограф.**|
|[clockOut](../api/timecard-clockout.md) | Нет | Часы, чтобы положить конец **открытой карточке времени**.|
|[startBreak](../api/timecard-startbreak.md) | Нет | Запустите **timeCardBreak** в определенной **карточке времени.**|
|[endBreak](../api/timecard-endbreak.md) | Нет | Завершение открытого **времениCardBreak** в определенной **карточке времени.**|
|[confirmTimeCard](../api/timecard-confirm.md) | Нет | Подтверждение **записи химкарта.**|

## <a name="properties"></a>Свойства
|Свойство               |Тип           |Описание                                                                |
|-----------------------|---------------|---------------------------------------------------------------------------|
| id                    |`string`  |ID **timeCard**.|
| userId                    |`string` |Пользовательский ID, к которому **принадлежит timeCard.** |
| state                 |`timeCardState`  | Текущее состояние **timeCard во** время жизненного цикла. Возможные значения: `clockedIn` `onBreak` , , `clockedOut` `unknownFutureValue` .|
| clockInEvent       |[timeCardEvent](../resources/timecardevent.md)    | Событие с часовой стрелкой **timeCard**. |
| clockOutEvent                 |[timeCardEvent](../resources/timecardevent.md)  |Событие clock-out **timeCard**. |
| notes                 | [itemBody](itembody.md)  |Заметки о **timeCard**. |
| перерывы    |[коллекция timeCardBreak](timecardbreak.md)  |Список перерывов, связанных с **timeCard**.|
| originalEntry| [timeCardEntry](../resources/timecardentry.md) | Исходное **времяCardEntry** **timeCard** перед изменением пользователя. |
| confirmedBy |`confirmedBy`    | Указать, подтверждена ли эта запись **timeCard.** Возможные значения: `none`, `user`, `manager`, `unknownFutureValue`.|
|createdDateTime|`Edm.dateTimeOffset`| Время создания **timeCard.** |
|createdBy|`IdentitySet`| Удостоверение лица, создавшего объект. |
|lastModifiedDateTime|`dateTimeOffset`| Время последнего изменения **timeCard.**|
|lastModifiedBy| `IdentitySet`| Удостоверение человека, который в последний раз изменил объект.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeCard",
   "baseType":"microsoft.graph.changeTrackedEntity"
}-->

```json
{
  "userId": "string (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {"@odata.type":"microsoft.graph.identitySet"},
  "clockInEvent" : {"@odata.type":"microsoft.graph.timeCardEvent"},
  "clockOutEvent" : {"@odata.type":"microsoft.graph.timeCardEvent"},
  "notes" : {"@odata.type":"microsoft.graph.itemBody"},
  "breaks" : [{"@odata.type":"microsoft.graph.timeCardEvent"}],
  "originalEntry" : {"@odata.type":"microsoft.graph.timeCardEntry"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeCard resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
