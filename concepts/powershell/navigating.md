---
title: Навигация по пакету SDK для Microsoft Graph PowerShell
description: Пакет SDK для Microsoft Graph PowerShell содержит большое количество команд. Узнайте, как найти нужную команду для достижения необходимых действий.
localization_priority: Normal
author: jasonjoh
ms.openlocfilehash: ceb4b0f783d1ad9a24cfc196d4099d5e67b3f273
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193712"
---
# <a name="navigating-the-microsoft-graph-powershell-sdk"></a>Навигация по пакету SDK для Microsoft Graph PowerShell

API Microsoft Graph огромный и все время растет. Из-за этого количество команд в пакете SDK PowerShell для Microsoft Graph также очень велико. Если вы еще не знакомы с Microsoft Graph, вы можете найти нужную команду. Рассмотрим несколько способов, которые помогут найти определенную команду.

## <a name="command-naming-conventions"></a>Соглашения об именовании команд

Команды в пакете SDK создаются непосредственно из [REST API](/graph/api/overview?view=graph-rest-1.0), поэтому API на имена влияют. Вам не нужно знать сведения об интерфейсе API, чтобы использовать этот пакет SDK, но он помогает определить соглашение об именовании.

Командам PowerShell присвоено имя с помощью команды существительное, например `Get-Command` OR `Update-List` . Давайте начнем с команды.

### <a name="command-verbs"></a>Команды

Для основных операций REST команда определяется методом HTTP, используемым для API.

| Метод HTTP | Командная команда | Пример |
|-------------|--------------|---|
| GET         | Получение          | `Get-MgUser` [Справочные материалы по API](/graph/api/user-get?view=graph-rest-1.0) |
| POST        | Новое          | `New-MgUserMessage` [Справочные материалы по API](/graph/api/user-post-messages?view=graph-rest-1.0) |
| PUT         | Новое          | `New-MgTeam` [Справочные материалы по API](/graph/api/team-put-teams?view=graph-rest-1.0) |
| PATCH       | Update       | `Update-MgUserEvent` [Справочные материалы по API](/graph/api/event-update?view=graph-rest-1.0) |
| DELETE      | Удалить       | `Remove-MgDriveItem` [Справочные материалы по API](/graph/api/driveitem-delete?view=graph-rest-1.0) |

Для функций и действий это немного сложнее. API в Microsoft Graph, реализованные как функции OData или действия, обычно именуются по крайней мере с помощью команды. Команда, соответствующая команде, основана на команде в имени функции или действия. Тем не менее, команды в PowerShell должны соответствовать определенным [правилам именования](/powershell/scripting/developer/cmdlet/approved-verbs-for-windows-powershell-commands), поэтому это может привести к неинтуитивным сопоставлениям имен и команд.

Рассмотрим несколько примеров. API [-](/graph/api/calendar-getschedule?view=graph-rest-1.0) интерфейсом, который использует API `get` , и `Get` является утвержденной командой PowerShell, поэтому команда выполняется `Get-MgUserCalendarSchedule` . API [отмены](/graph/api/event-cancel?view=graph-rest-beta) для события с другой стороны, использует неутвержденную команду `cancel` . Утвержденная команда для отмены или отмены чего-либо `Stop` , поэтому она выглядит так `Stop-MgUserEvent` : Наконец, глагол API [снузереминдер](/graph/api/event-snoozereminder?view=graph-rest-1.0) , не `snooze` имеет эквивалентного утверждению PowerShell. Для API аналогично, в пакете SDK используется команда `Invoke` , поэтому эта команда API является `Invoke-MgSnoozeUserEventReminder` .

### <a name="command-nouns"></a>Существительные команды

Теперь вы могли заметить, что все существительные в командах пакета SDK начинаются с `Mg` . Этот префикс помогает избежать конфликтов имен с другими модулями PowerShell. С учетом этого следует иметь в виду, что `Get-MgUser` для получения пользователя используются команды, такие как. И следующее соглашение PowerShell, несмотря на то, что существительное в единственном числе, эти команды могут возвращать несколько результатов, если не запрашивается определенный экземпляр.

Но что делать с командами, такими как `Get-MgUserMessage` или `Get-MgUserMailFolderMessage` ? Оба эти объекта получают объект [Message](/graph/api/resources/message?view=graph-rest-1.0) , поэтому почему `Get-MgMessage` ? Ответ берется из [API получения сообщений](/graph/api/message-get?view=graph-rest-1.0).

Просмотрите HTTP-запросы для этого API. Игнорируя запросы, содержащиеся `/me` в URL-адресе, существует два других способа вызова этого API.

```http
GET /users/{id | userPrincipalName}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

Пути совпадают с существительными. Для первой формы следует начать с `users` , а затем выполнить `messages` команду `Get-MgUserMessage` . Во второй форме сначала следует начать с `users` , а затем — `mailFolders` сообщения, чтобы сделать команду `Get-MgUserMailFolderMessage` .

Еще один способ взглянуть на это — это то, что является владельцем или содержит. Пользователь владеет почтовыми папками, а почтовые папки содержат сообщения. Добавьте префикс и получите его `Get-MgUserMailFolderMessage` .

## <a name="finding-available-commands"></a>Поиск доступных команд

Иногда достаточно знать соглашение об именовании, чтобы угадать правильную команду. В этом случае можно использовать `Get-Command` команду для поиска доступных команд в пакете SDK. Например, если вы ищете команды, связанные с Microsoft Teams, вы можете выполнить следующую команду:

```powershell
Get-Command -Module Microsoft.Graph* *team*
```
