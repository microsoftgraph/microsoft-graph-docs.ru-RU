---
title: тип ресурса
description: Коллекция schedulingGroups, shifts, timeOffReasons и timesOff в команде.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: b7ad28acfc03726d9645afce686b327d6d5414b9755f6f01791e21b544a5d8e4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54189347"
---
# <a name="schedule-resource-type"></a>тип ресурса

Пространство имен: microsoft.graph

Коллекция объектов [schedulingGroup,](schedulinggroup.md) [объектов переноса,](shift.md) [объектов TimeOffReason](timeoffreason.md) и [объектов timeOff в](timeoff.md) [команде.](../resources/team.md) 

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Создание или замена расписания](../api/team-put-schedule.md) | [schedule](schedule.md) | Создание или замена расписания.|
|[Получить расписание](../api/schedule-get.md) | [schedule](schedule.md) | Получите расписание.|
|[Предоставление общего доступа](../api/schedule-share.md) | Нет | Поделитесь диапазоном времени расписания с участниками расписания.|

## <a name="properties"></a>Свойства
|Имя                   |Тип           |Описание                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| id                    |строка  |ID расписания.|
| enabled               |Boolean    | Указывает, включено ли расписание для группы. Обязательный элемент.|
| timeZone              |string  | Указывает часовой пояс группы расписания с помощью формата базы данных tz. Обязательный элемент.|
| provisionStatus       |operationStatus    | Состояние подготовка расписания. Возможные значения `notStarted` , `running` , `completed` `failed` . |
| provisionStatusCode   |Строка  | Дополнительные сведения о том, почему подготовка расписания не удалась. |
| timeClockEnabled                  |Логический  | Указывает, включены ли часы времени для расписания.             |
| openShiftsEnabled                 |Логическое  | Указывает, включены ли открытые смены для расписания.             | 
| swapShiftsRequestsEnabled                 |Логическое| Указывает, включены ли запросы на смены для расписания.             |
| offerShiftRequestsEnabled                 |Логическое  | Указывает, включены ли запросы на перенос предложения для расписания.             | 
| timeOffRequestsEnabled                    |Логическое | Указывает, включены ли запросы на время для расписания.             | 



## <a name="relationships"></a>Связи
|Имя                   |Тип           |Описание                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| сдвиги   | Коллекция [shift](shift.md)  | Изменения в расписании. |
| timesOff   |[коллекция timeOff](timeoff.md)  | Случаи отключения времени в расписании. |
| timeOffReasons   |[коллекция timeOffReason](timeoffreason.md)  | Набор причин для отключки в расписании. |
| schedulingGroups   |Коллекция объектов [schedulingGroup](schedulinggroup.md)  | Логическая группировка пользователей в расписании (обычно по роли). |
| openshifts   |[коллекция openShift](openshift.md) | Набор открытых смен в группе планирования в расписании. |
| workforceintegrations   |[коллекция workforceIntegration](workforceintegration.md)  | Пример интеграции рабочей силы в одну команду с исходящие потоки данных в синхронных уведомлениях об изменениях (для поддерживаемых сущностям). |
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

