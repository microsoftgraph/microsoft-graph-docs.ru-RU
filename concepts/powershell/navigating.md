---
title: Навигация по пакету SDK Microsoft Graph PowerShell
description: Пакет SDK Microsoft Graph PowerShell содержит большое количество команд. Узнайте, как найти подгоную команду для достижения поставленных целей.
ms.localizationpriority: medium
author: jasonjoh
ms.openlocfilehash: 2c4135691712bcc6cbe8a32a776aa40844ec668e
ms.sourcegitcommit: 19558bd9de9b717e7a36bfce1d6d84d0132e2697
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2022
ms.locfileid: "64883404"
---
# <a name="navigating-the-microsoft-graph-powershell-sdk"></a>Навигация по пакету SDK Microsoft Graph PowerShell

Корпорация Майкрософт API Graph и постоянно растет. По этой причине количество команд в пакете SDK Microsoft Graph PowerShell также очень велико. Поиск нужной команды может оказаться сложной задачей, особенно если вы еще не знакомы с microsoft Graph. Давайте рассмотрим несколько способов поиска определенной команды.

[!INCLUDE [aad-advanced-queries-note](../../includes/aad-advanced-queries-note.md)]

## <a name="command-naming-conventions"></a>Соглашения об именовании команд

Команды в пакете SDK создаются непосредственно из [REST API](/graph/api/overview?view=graph-rest-1.0&preserve-view=true), поэтому на имена влияет API. Вам не нужно понимать сведения об API для использования этого пакета SDK, но это помогает понять соглашение об именовании.

Команды PowerShell именуются с помощью пары глагол-существительное, например или `Get-Command` `Update-List`. Начнем с команды.

### <a name="command-verbs"></a>Команды

Для основных операций REST команда определяется методом HTTP, используемым для API.

| Метод HTTP | Команда | Пример |
|-------------|--------------|---|
| GET         | Получение          | `Get-MgUser` [Справочные материалы по API](/graph/api/user-get?view=graph-rest-1.0&preserve-view=true) |
| POST        | Новое          | `New-MgUserMessage` [Справочные материалы по API](/graph/api/user-post-messages?view=graph-rest-1.0&preserve-view=true) |
| PUT         | Новое          | `New-MgTeam` [Справочные материалы по API](/graph/api/team-put-teams?view=graph-rest-1.0&preserve-view=true) |
| PATCH       | Update       | `Update-MgUserEvent` [Справочные материалы по API](/graph/api/event-update?view=graph-rest-1.0&preserve-view=true) |
| DELETE      | Удалить       | `Remove-MgDriveItem` [Справочные материалы по API](/graph/api/driveitem-delete?view=graph-rest-1.0&preserve-view=true) |

Для функций и действий это немного сложнее. Интерфейсы API в Microsoft Graph, реализованные как функции или действия OData, обычно именуются по крайней мере командой. Команда соответствующей команды основана на глаголе в имени функции или действия. Однако командные команды в PowerShell должны соответствовать определенным правилам именования [, поэтому](/powershell/scripting/developer/cmdlet/approved-verbs-for-windows-powershell-commands) это может привести к неинтуативным сопоставлениям имен и команд.

Рассмотрим некоторые примеры. API [getSchedule](/graph/api/calendar-getschedule?view=graph-rest-1.0&preserve-view=true) использует `get``Get` и является утвержденной командой PowerShell, поэтому это команда `Get-MgUserCalendarSchedule`. С [другой стороны](/graph/api/event-cancel?view=graph-rest-beta&preserve-view=true) , API отмены для события использует не утвержденную команду `cancel`. Утвержденная команда для отмены или отмены чего-либо является `Stop`, поэтому команда имеет значение `Stop-MgUserEvent`. Наконец, команда API [snoozeReminder](/graph/api/event-snoozereminder?view=graph-rest-1.0&preserve-view=true) не имеет эквивалента, `snooze`утвержденного PowerShell. Для таких API пакет SDK `Invoke`использует команду, чтобы команда API была такой `Invoke-MgSnoozeUserEventReminder`.

### <a name="command-nouns"></a>Существительные команд

К настоящему моменту вы могли заметить, что все существительные в командах пакета SDK начинаются с `Mg`. Этот префикс помогает избежать конфликтов именования с другими модулями PowerShell. Учитывая это, имеет смысл `Get-MgUser` , что такие команды используются для получения пользователя. Кроме того, несмотря на то, что существительное является единым, эти же команды могут возвращать несколько результатов, если конкретный экземпляр не запрашивается.

Но как насчет таких команд `Get-MgUserMessage` `Get-MgUserMailFolderMessage`? И то, и другое получает [объект сообщения](/graph/api/resources/message?view=graph-rest-1.0&preserve-view=true) , так почему бы и нет `Get-MgMessage`? Ответ поступает из [API получения сообщения](/graph/api/message-get?view=graph-rest-1.0&preserve-view=true).

Просмотрите HTTP-запросы для этого API. Игнорируя запросы в `/me` URL-адресе, можно вызвать этот API двумя другими способами.

```http
GET /users/{id | userPrincipalName}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

Пути соответствуют существительным. Для первой формы вы начинаете с `users`, а затем `messages`, поэтому команда имеет значение `Get-MgUserMessage`. Во второй форме вы начинаете с `users`сообщения`mailFolders`, а затем сообщения, поэтому команда будет .`Get-MgUserMailFolderMessage`

Другим способом просмотра является то, что является владельцем или содержит то, что. Пользователь владеет почтовыми папками, а почтовые папки содержат сообщения. Добавьте префикс и получите .`Get-MgUserMailFolderMessage`

### <a name="listing-parameters"></a>Перечисление параметров

После поиска нужной команды можно проверить все доступные параметры с помощью этой `Get-Help` команды. Например, приведенная ниже команда выводит список всех доступных параметров для `Get-MgUser` команды.

```powershell
Get-Help Get-MgUser -Detailed
```

## <a name="finding-available-commands"></a>Поиск доступных команд

Иногда просто знать соглашения об именовании недостаточно, чтобы угадать подголовную команду. В этом случае можно использовать команду `Get-Command` для поиска доступных команд в пакете SDK. Например, если вы ищете команды, связанные с Microsoft Teams, можно выполнить следующую команду.

```powershell
Get-Command -Module Microsoft.Graph* *team*
```
