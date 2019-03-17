---
title: Тип ресурса "Расписание"
description: Коллекция Счедулингграупс, Shift, Тимеоффреасонс и Тимесофф в команде.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: de3662fcf3c5a8e50493e365f6a10a8641a451df
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657513"
---
# <a name="schedule-resource-type"></a>Тип ресурса "Расписание"

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Коллекция объектов [счедулингграуп](schedulinggroup.md) , объектов [сдвига](shift.md) , объектов [тимеоффреасон](timeoffreason.md) и объектов [тимеофф](timeoff.md) в [команде](../resources/team.md). 

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Создание или замена расписания](../api/team-put-schedule.md) | [Диспетчер](schedule.md) | Создание или замена `schedule`.|
|[Получение расписания](../api/schedule-get.md) | [Диспетчер](schedule.md) | Получение `schedule`.|
|[share](../api/schedule-share.md) | Нет | Предоставьте общий `schedule` доступ к диапазону времени с участниками расписания.|

## <a name="properties"></a>Свойства
|Имя                   |Тип           |Описание                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| id                    |`string`  |Идентификатор объекта `schedule`.|
| enabled               |`bool`    | Указывает, включено ли расписание для группы. Обязательный.|
| timeZone              |`string`  | Указывает часовой пояс, в течение которого Группа расписаний использует формат базы данных. Обязательный.|
| Провисионстатус       |`enum`    | Состояние подготовки расписания. |
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
  "suppressions": [
    "Error: /api-reference/beta/resources/schedule.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
