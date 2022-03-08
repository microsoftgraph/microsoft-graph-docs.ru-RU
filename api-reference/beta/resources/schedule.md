---
title: тип ресурса
description: Коллекция schedulingGroups, shifts, timeOffReasons и timesOff в команде.
author: aaku
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 0aff494a1a5fdc4c710272e279089ff35fbd51fa
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335194"
---
# <a name="schedule-resource-type"></a>тип ресурса

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Коллекция объектов [schedulingGroup](schedulinggroup.md) , [объектов переноса](shift.md) , [объектов TimeOffReason](timeoffreason.md) и [объектов timeOff в](timeoff.md) [команде](../resources/team.md). 

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Создание или замена расписания](../api/team-put-schedule.md) | [schedule](schedule.md) | Создание или замена расписания.|
|[Получить расписание](../api/schedule-get.md) | [schedule](schedule.md) | Получите расписание.|
|[Предоставление общего доступа](../api/schedule-share.md) | Нет | Поделитесь диапазоном времени расписания с участниками расписания.|

## <a name="properties"></a>Свойства
|Имя                   |Тип           |Описание                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| id                    |string  |ID расписания.|
| enabled               |Boolean    | Указывает, включено ли расписание для группы. Обязательный элемент.|
| timeZone              |string  | Указывает часовой пояс группы расписания с помощью формата базы данных tz. Обязательный элемент.|
| provisionStatus       |operationStatus    | Состояние подготовка расписания. Возможные значения , `notStarted`, `running``completed``failed`. |
| provisionStatusCode   |Строка  | Дополнительные сведения о том, почему подготовка расписания не удалась. |
| timeClockEnabled                  |Boolean  | Указывает, включены ли часы времени для расписания.             |
| openShiftsEnabled                 |Boolean  | Указывает, включены ли открытые смены для расписания.             | 
| swapShiftsRequestsEnabled                 |Boolean| Указывает, включены ли запросы на смены для расписания.             |
| offerShiftRequestsEnabled                 |Boolean  | Указывает, включены ли запросы на перенос предложения для расписания.             | 
| timeOffRequestsEnabled                    |Boolean | Указывает, включены ли запросы на время для расписания.             | 



## <a name="relationships"></a>Связи
|Имя                   |Тип           |Описание                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| сдвиги   | Коллекция [shift](shift.md)  | Изменения в расписании. |
| timesOff   |[коллекция timeOff](timeoff.md)  | Случаи отключения времени в расписании. |
| timeOffReasons   |[коллекция timeOffReason](timeoffreason.md)  | Набор причин для отключки в расписании. |
| schedulingGroups   |Коллекция [schedulingGroup](schedulinggroup.md)  | Логическая группировка пользователей в расписании (обычно по роли). |
| openshifts   |[коллекция openShift](openshift.md) | Набор открытых смен в группе планирования в расписании. |
| workforceintegrations   |коллекция [workforceIntegration](workforceintegration.md)  | Пример интеграции рабочей силы в одну команду с исходящие потоки данных в синхронных уведомлениях об изменениях (для поддерживаемых сущностям). |
| swapshiftchangerequests   |[коллекция swapShiftsChangeRequest](swapshiftschangerequest.md)  | Запросы на замену для сдвигов в расписании. |
| openshiftchangerequests   |[коллекция openShiftChangeRequest](openshiftchangerequest.md)  | Запросы на открытую смену в расписании. |
| timeoffrequest   |[коллекция timeOffRequest](timeoffrequest.md)  | Время отключения запросов в расписании. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

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


