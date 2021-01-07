---
title: Навигация по Microsoft Graph PowerShell SDK
description: Microsoft Graph PowerShell SDK содержит большое количество команд. Узнайте, как найти правильные команды для достижения нужных результатов.
localization_priority: Normal
author: jasonjoh
ms.openlocfilehash: 79c5ce415d00ba63ed6007e21248d51e721035c4
ms.sourcegitcommit: 7732d20bd99a125118f7cea146c3f2416879f949
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/07/2021
ms.locfileid: "49777591"
---
# <a name="navigating-the-microsoft-graph-powershell-sdk"></a>Навигация по Microsoft Graph PowerShell SDK

API Microsoft Graph является огромной и постоянно растет. По этой причине количество команд в Microsoft Graph PowerShell SDK также очень большое. Поиск нужной команды может быть сложной задачей, особенно если вы еще не знакомы с Microsoft Graph. Рассмотрим несколько способов поиска определенной команды.

## <a name="command-naming-conventions"></a>Соглашения об именовании команд

Команды в SDK создаются непосредственно из [REST API,](/graph/api/overview?view=graph-rest-1.0&preserve-view=true)поэтому на имена влияет API. Вам не нужно понимать сведения об API для использования этого SDK, но это помогает понять соглашение об именовке.

Команды PowerShell именуются с помощью пары "глагол-существительное", например `Get-Command` или `Update-List` . Начнем с глагола.

### <a name="command-verbs"></a>Команды

Для базовых операций REST глагол определяется методом HTTP, используемым для API.

| Метод HTTP | Команда | Пример |
|-------------|--------------|---|
| GET         | Получение          | `Get-MgUser` [Справочные материалы по API](/graph/api/user-get?view=graph-rest-1.0&preserve-view=true) |
| POST        | Новое          | `New-MgUserMessage` [Справочные материалы по API](/graph/api/user-post-messages?view=graph-rest-1.0&preserve-view=true) |
| PUT         | Новое          | `New-MgTeam` [Справочные материалы по API](/graph/api/team-put-teams?view=graph-rest-1.0&preserve-view=true) |
| PATCH       | Update       | `Update-MgUserEvent` [Справочные материалы по API](/graph/api/event-update?view=graph-rest-1.0&preserve-view=true) |
| DELETE      | Удалить       | `Remove-MgDriveItem` [Справочные материалы по API](/graph/api/driveitem-delete?view=graph-rest-1.0&preserve-view=true) |

Для функций и действий это немного сложнее. API в Microsoft Graph, реализованные как функции или действия OData, обычно именуются по крайней мере с помощью команды. Глагол соответствующей команды основан на глаголе в имени функции или действия. Однако команды в PowerShell должны соответствовать [](/powershell/scripting/developer/cmdlet/approved-verbs-for-windows-powershell-commands)определенным правилам именования, поэтому это может привести к неинтуитивным сопоставлениям имен и команд.

Рассмотрим несколько примеров. API [getSchedule](/graph/api/calendar-getschedule?view=graph-rest-1.0&preserve-view=true) использует и является утвержденной командой `get` `Get` PowerShell, поэтому это `Get-MgUserCalendarSchedule` команда. С [другой](/graph/api/event-cancel?view=graph-rest-beta&preserve-view=true) стороны, API отмены для события использует не утвержденные `cancel` команды. Утвержденная команда для отмены или прекращения действия чего-либо `Stop` есть, поэтому это `Stop-MgUserEvent` команда. Наконец, глагол API [snoozeReminder](/graph/api/event-snoozereminder?view=graph-rest-1.0&preserve-view=true) не имеет эквивалента, утвержденного `snooze` PowerShell. Для таких API SDK использует глагол, чтобы команда `Invoke` API была `Invoke-MgSnoozeUserEventReminder` .

### <a name="command-nouns"></a>Существии команд

Возможно, вы уже заметили, что все существии в командах SDK начинаются с `Mg` . Этот префикс помогает избежать конфликтов имен с другими модулями PowerShell. С учетом этого следует иметь в виду, что такие команды используются `Get-MgUser` для получения пользователя. И следуя соглашению PowerShell, хотя существительное является единым, эти же команды могут возвращать несколько результатов, если не запрашивается ни один экземпляр.

Но что насчет таких `Get-MgUserMessage` `Get-MgUserMailFolderMessage` команд? Оба этих объекта получают [объект сообщения,](/graph/api/resources/message?view=graph-rest-1.0&preserve-view=true) так почему бы и `Get-MgMessage` нет? Ответ поступает из [API получения сообщения.](/graph/api/message-get?view=graph-rest-1.0&preserve-view=true)

Посмотрите на HTTP-запросы для этого API. Игнорируя запросы в URL-адресе, можно вызвать этот API двумя `/me` другими способами.

```http
GET /users/{id | userPrincipalName}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

Пути совпадают с существительным. Для первой формы вы начинаете с `users` , затем , поэтому команда является `messages` `Get-MgUserMessage` . Во второй форме вы начинаете с `users` ,then `mailFolders` , then messages, поэтому команда будет `Get-MgUserMailFolderMessage` .

Еще один способ посмотреть на то, что принадлежит или содержит что. Пользователь владеет почтовыми папками, а почтовые папки содержат сообщения. Добавьте префикс и получите `Get-MgUserMailFolderMessage` .

### <a name="listing-parameters"></a>Параметры списка

После того как вы нашли подытную команду, вы можете проверить все доступные параметры с помощью `Get-Help` этой команды. Например, следующая команда перечисляет все доступные параметры `Get-MgUser` для команды.

```powershell
Get-Help Get-MgUser -Detailed
```

## <a name="finding-available-commands"></a>Поиск доступных команд

Иногда просто знать соглашения об именовании недостаточно, чтобы угадать подымену нужной команды. В этом случае можно использовать команду для поиска доступных команд `Get-Command` в SDK. Например, если вы ищете команды, связанные с Microsoft Teams, можно выполнить следующую команду.

```powershell
Get-Command -Module Microsoft.Graph* *team*
```
