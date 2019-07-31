---
title: Тип ресурса "Расписание"
description: Коллекция Счедулингграупс, Shift, Тимеоффреасонс и Тимесофф в команде.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: a404c620b20cfcb69076ecc3bac25f907a12216c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965329"
---
# <a name="schedule-resource-type"></a>Тип ресурса "Расписание"

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Коллекция объектов [счедулингграуп](schedulinggroup.md) , объектов [сдвига](shift.md) , объектов [тимеоффреасон](timeoffreason.md) и объектов [тимеофф](timeoff.md) в [команде](../resources/team.md). 

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Создание или замена расписания](../api/team-put-schedule.md) | [schedule](schedule.md) | Создание или замена `schedule`.|
|[Получение расписания](../api/schedule-get.md) | [schedule](schedule.md) | Получение `schedule`.|
|[share](../api/schedule-share.md) | Нет | Предоставьте общий `schedule` доступ к диапазону времени с участниками расписания.|

## <a name="properties"></a>Свойства
|Имя                   |Тип           |Описание                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| id                    |`string`  |Идентификатор объекта `schedule`.|
| enabled               |`bool`    | Указывает, включено ли расписание для группы. Обязательно.|
| timeZone              |`string`  | Указывает часовой пояс, в течение которого Группа расписаний использует формат базы данных. Обязательно.|
| Провисионстатус       |`operationStatus`    | Состояние подготовки расписания. `notStarted`Возможные значения: `running`,, `completed`,. `failed` |
| Провисионстатускоде   |`string`  | Дополнительные сведения о том, почему не удалось подготовить расписание. |


## <a name="relationships"></a>Связи
|Имя                   |Тип           |Описание                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| Сдвигает   |`collection(shift)`  | Смены в расписании. |
| Тимесофф   |`collection(timeOff)`  | Экземпляры повременных вызовов в расписании. |
| Тимеоффреасонс   |`collection(timeOffReason)`  | Набор причин незапланированного времени. |
| Счедулингграупс   |`collection(schedulingGroup)`  | Логическая группа пользователей в расписании (обычно по роли). |


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.schedule"
}-->

```json
{
  "id": "833fc4df-c88b-4398-992f-d8afcfe41df2",
  "enabled": true,
  "timeZone": "America/Chicago",
  "provisionStatus": "Completed",
  "provisionStatusCode": null
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "schedule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
