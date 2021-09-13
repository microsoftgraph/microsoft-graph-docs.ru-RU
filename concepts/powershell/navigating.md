---
title: Навигация по SDK Graph PowerShell
description: SDK Graph PowerShell содержит большое количество команд. Узнайте, как найти нужные команды для того, чего вы хотите достичь.
ms.localizationpriority: medium
author: jasonjoh
ms.openlocfilehash: 2c231ca186e9274a09500247827141cbf03e0e7c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59139039"
---
# <a name="navigating-the-microsoft-graph-powershell-sdk"></a>Навигация по SDK Graph PowerShell

API Graph Microsoft является огромным и постоянно растет. Из-за этого количество команд в microsoft Graph PowerShell SDK также очень большое. Поиск правильной команды для того, чего вы хотите добиться, может быть сложной задачей, особенно если вы еще не знакомы с Microsoft Graph. Рассмотрим несколько способов поиска определенной команды.

## <a name="command-naming-conventions"></a>Соглашения о именовании команд

Команды в SDK создаются непосредственно из [API REST,](/graph/api/overview?view=graph-rest-1.0&preserve-view=true)поэтому на имена влияет API. Чтобы использовать этот SDK, не нужно разбираться в деталях API, но это помогает понять конвенцию именования.

Команды PowerShell именуются с помощью пары существительное глагола, например `Get-Command` или `Update-List` . Начнем с глагола.

### <a name="command-verbs"></a>Командные глаголы

Для основных операций REST глагол определяется методом HTTP, используемым для API.

| Метод HTTP | Командный глагол | Пример |
|-------------|--------------|---|
| GET         | Получение          | `Get-MgUser` [Справочные материалы по API](/graph/api/user-get?view=graph-rest-1.0&preserve-view=true) |
| POST        | Новое          | `New-MgUserMessage` [Справочные материалы по API](/graph/api/user-post-messages?view=graph-rest-1.0&preserve-view=true) |
| PUT         | Новая          | `New-MgTeam` [Справочные материалы по API](/graph/api/team-put-teams?view=graph-rest-1.0&preserve-view=true) |
| PATCH       | Update       | `Update-MgUserEvent` [Справочные материалы по API](/graph/api/event-update?view=graph-rest-1.0&preserve-view=true) |
| DELETE      | Удалить       | `Remove-MgDriveItem` [Справочные материалы по API](/graph/api/driveitem-delete?view=graph-rest-1.0&preserve-view=true) |

Для функций и действий это немного сложнее. API в Microsoft Graph, которые реализуются в качестве функций или действий OData, обычно называются с по крайней мере глаголом. Глагол соответствующей команды основан на глаголе в имени функции или действия. Однако глаголы команд в PowerShell должны соответствовать определенным правилам [именования,](/powershell/scripting/developer/cmdlet/approved-verbs-for-windows-powershell-commands)поэтому это может привести к неинтуитивным сопоставлениям между именами и командами.

Рассмотрим несколько примеров. API [getSchedule](/graph/api/calendar-getschedule?view=graph-rest-1.0&preserve-view=true) использует и является утвержденным глаголом `get` `Get` PowerShell, поэтому его командой является `Get-MgUserCalendarSchedule` . [API](/graph/api/event-cancel?view=graph-rest-beta&preserve-view=true) отмены события, с другой стороны, использует не утвержденный глагол `cancel` . Утвержденный глагол для отмены или прекращения что-то есть, так `Stop` что это команда `Stop-MgUserEvent` . Наконец, [глагол API snoozeReminder](/graph/api/event-snoozereminder?view=graph-rest-1.0&preserve-view=true) не имеет эквивалента, утвержденного `snooze` PowerShell. Для API используется глагол SDK, чтобы команда API была `Invoke` `Invoke-MgSnoozeUserEventReminder` .

### <a name="command-nouns"></a>Существимы команды

Возможно, вы уже заметили, что все существии в командах SDK начинаются с `Mg` . Этот префикс помогает избежать конфликтов именования с другими модулями PowerShell. С учетом этого следует иметь в виду, что такие команды используются `Get-MgUser` для получения пользователя. И в соответствии с конвенцией PowerShell, даже если существительное является исключительным, эти же команды могут возвращать несколько результатов, если не запрашивается конкретный экземпляр.

Но как насчет команд, как `Get-MgUserMessage` `Get-MgUserMailFolderMessage` или? Оба из них получают [объект сообщения,](/graph/api/resources/message?view=graph-rest-1.0&preserve-view=true) так почему бы и `Get-MgMessage` нет? Ответ приходит из [API получения сообщения](/graph/api/message-get?view=graph-rest-1.0&preserve-view=true).

Посмотрите на запросы HTTP для этого API. Игнорируя запросы в URL-адресе, можно вызвать этот API двумя `/me` другими способами.

```http
GET /users/{id | userPrincipalName}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

Пути совпадают с существительным. Для первой формы, вы начинаете с `users` , то , так что команда `messages` `Get-MgUserMessage` . Во второй форме вы начинаете с `users` , а затем `mailFolders` сообщения, поэтому команда `Get-MgUserMailFolderMessage` .

Другой способ посмотреть на это является то, что владеет или содержит то, что. Пользователь владеет почтовыми папками, а почтовые папки содержат сообщения. Добавьте префикс и получите `Get-MgUserMailFolderMessage` .

### <a name="listing-parameters"></a>Параметры перечисления

После того, как вы находили нужные команды, вы можете изучить все доступные параметры с помощью `Get-Help` команды. Например, в следующей команде перечислены все доступные параметры `Get-MgUser` для команды.

```powershell
Get-Help Get-MgUser -Detailed
```

## <a name="finding-available-commands"></a>Поиск доступных команд

Иногда просто знать конвенции имен не достаточно, чтобы угадать правую команду. В этом случае можно использовать команду для поиска доступных команд в `Get-Command` SDK. Например, если вы ищете команды, связанные с Microsoft Teams, можно запустить следующую команду.

```powershell
Get-Command -Module Microsoft.Graph* *team*
```
