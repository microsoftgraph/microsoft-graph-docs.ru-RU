---
title: тип ресурса teamsUserActivityUserDetail
description: Представляет сведения о действиях пользователей Microsoft Teams пользователем.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 4afa7f17acac13eaa1c517953517fcfbe344aaa7
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766436"
---
# <a name="teamsuseractivityuserdetail-resource-type"></a>тип ресурса teamsUserActivityUserDetail

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о действиях пользователей Microsoft Teams пользователем.

## <a name="properties"></a>Свойства

| Свойство                                 | Тип              | Описание                                                  |
| :--------------------------------------- | :---------------- | ------------------------------------------------------------ |
| reportRefreshDate                        | Дата              | Последняя дата контента.                              |
| userPrincipalName                        | String            | Имя участника-пользователя. Это имя для входа через Интернет по стандарту RFC 822. В соответствии с соглашением оно должно указывать на имя пользователя для электронной почты. Общий формат: псевдоним@домен. При этом домен должен входить в коллекцию проверенных доменов клиента. Это свойство обязательно указывать при создании пользователя. |
| isLicensed                               | Логический           | Назначена ли пользователю лицензия Teams.          |
| lastActivityDate                         | Дата              | Последняя дата участия пользователя в действии Microsoft Teams. |
| isDeleted                                | Логический           | Был ли этот пользователь удален или удален.          |
| deletedDate                              | Дата              | Дата, когда произошла операция удаления. Значение по умолчанию — "null", если пользователь не удален. |
| assignedProducts                         | Коллекция String | Продукты, которые назначены пользователю.                             |
| teamChatMessageCount                     | Int64             | Количество уникальных сообщений, которые пользователь разместил в командном чате. |
| privateChatMessageCount                  | Int64             | Количество уникальных сообщений, которые пользователь разместил в частном чате. |
| callCount                                | Int64             | Число вызовов 1:1, в которые принимал участие пользователь.       |
| meetingCount                             | Int64             | Количество онлайн-собраний, в которые принимал участие пользователь. |
| meetingsOrganizedCount                   | Int64             | Сумма разовых запланированных, повторяющихся, разовых и неклассифицированных собраний, организованных пользователем. |
| meetingsAttendedCount                    | Int64             | Сумма разовых, повторяющихся, разовых и неклассифицированных собраний, в которые принимал участие пользователь. |
| adHocMeetingsOrganizedCount              | Int64             | Количество организованных пользователем собраний.              |
| adHocMeetingsAttendedCount               | Int64             | Количество разных собраний, в которые принимал участие пользователь.        |
| scheduledOneTimeMeetingsOrganizedCount   | Int64             | Количество разовых запланированных собраний, организованных пользователем.  |
| scheduledOneTimeMeetingsAttendedCount    | Int64             | Количество разовых запланированных собраний, в которые принимал участие пользователь. |
| scheduledRecurringMeetingsOrganizedCount | Int64             | Количество повторных собраний, организованных пользователем.           |
| scheduledRecurringMeetingsAttendedCount  | Int64             | Количество повторяющихся собраний, в которые принимал участие пользователь. |
| audioDuration                            | Duration          | Продолжительность звука, в который принимал участие пользователь.                     |
| videoDuration                            | Duration          | Продолжительность видео, в котором участвовал пользователь.                     |
| screenShareDuration                      | Duration          | Продолжительность совместного доступа к экранам, в чем участвовал пользователь.            |
| hasOtherAction                           | Логический           | Пользователь активен, но выполняет другие действия, чем выставленные типы действий, предлагаемые в отчете (отправка или ответ на сообщения канала и сообщения чата, планирование или участие в вызовах и собраниях 1:1). Примеры действий, когда пользователь меняет состояние Teams или сообщение о состоянии Teams или открывает сообщение сообщения канала, но не отвечает. |
| reportPeriod                             | String            | Количество дней, которые охватывает отчет.                        |

## <a name="json-representation"></a>Представление JSON

Ниже приводится JSON representaion ресурса.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "isLicensed": true, 
  "lastActivityDate": "Date", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "assignedProducts": ["String"],
  "teamChatMessageCount": 1024, 
  "privateChatMessageCount": 1024, 
  "callCount": 1024, 
  "meetingCount": 1024, 
  "meetingsOrganizedCount": 1024, 
  "meetingsAttendedCount": 1024, 
  "adHocMeetingsOrganizedCount": 1024, 
  "adHocMeetingsAttendedCount": 1024, 
  "scheduledOneTimeMeetingsOrganizedCount": 1024, 
  "scheduledOneTimeMeetingsAttendedCount": 1024, 
  "scheduledRecurringMeetingsOrganizedCount": 1024, 
  "scheduledRecurringMeetingsAttendedCount": 1024, 
  "audioDuration": "Duration", 
  "videoDuration": "Duration", 
  "screenShareDuration": "Duration", 
  "hasOtherAction": true, 
  "reportPeriod": "String"
}
```


