---
title: Начало работы с SDK Microsoft Graph PowerShell
description: Приступить к работе с microsoft Graph PowerShell SDK, используя его для выполнения некоторых базовых задач.
localization_priority: Normal
author: jasonjoh
ms.openlocfilehash: 44ae296a7e4beae08e5e47561097d7011012d2f3bfbc9c45b12dcf5059bba13e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54168999"
---
# <a name="get-started-with-the-microsoft-graph-powershell-sdk"></a>Начало работы с SDK Microsoft Graph PowerShell

В этом руководстве вы будете использовать SDK microsoft Graph PowerShell для выполнения некоторых базовых задач. Если вы еще не установили [SDK,](installation.md)сделайте это, прежде чем следовать этому руководству.

## <a name="api-version"></a>Версия API

По умолчанию SDK использует [API Graph REST v1.0.](/graph/api/overview?view=graph-rest-1.0&preserve-view=true) Это можно изменить с помощью `Select-MgProfile` команды.

```powershell
Select-MgProfile -Name "beta"
```

## <a name="authentication"></a>Проверка подлинности

SDK PowerShell поддерживает два типа проверки подлинности: делегированную и доступ только для приложений. В этом руководстве вы будете использовать делегированную возможность входа в систему в качестве пользователя, предоставить согласие SDK для действий от вашего имени и вызвать службу Microsoft Graph.

Сведения об использовании доступа только для приложений для неохваченных сценариев см. в материале [Use app-only authentication with the Microsoft Graph PowerShell SDK.](app-only.md)

### <a name="determine-required-permission-scopes"></a>Определение необходимых областей разрешений

Каждый API в microsoft Graph защищен одной или более областью разрешений. Вход пользователя должен дать согласие на один из необходимых областей для API, которые вы планируете использовать. В этом примере мы будем использовать следующие API.

- [Список пользователей,](/graph/api/user-list?view=graph-rest-1.0&preserve-view=true) чтобы найти пользовательский ID пользователя, вошел в систему
- [Список joinedTeams,](/graph/api/user-list-joinedteams?view=graph-rest-1.0&preserve-view=true) чтобы Teams пользователь является членом.
- [Список каналов](/graph/api/channel-list?view=graph-rest-1.0&preserve-view=true) для получения каналов в команде.
- [Отправка сообщения](/graph/api/channel-post-messages?view=graph-rest-1.0&preserve-view=true) для отправки сообщения на канал Team.

Область разрешений позволит включить первые два вызова, а остальные - `User.Read.All` `Group.ReadWrite.All` область. Эти разрешения требуют учетной записи администратора.

### <a name="sign-in"></a>Выполнение входа

Используйте команду `Connect-MgGraph` для входов с требуемой областью. Чтобы согласиться на необходимые области, необходимо войти в учетную запись администратора.

```powershell
Connect-MgGraph -Scopes "User.Read.All","Group.ReadWrite.All"
```

Команда побуждает вас перейти на веб-страницу, чтобы войти в код устройства. После этого команда указывает на успех с `Welcome To Microsoft Graph!` сообщением. Это нужно делать только один раз за сеанс.

> [!TIP]
> Дополнительные разрешения можно добавить, повторив команду `Connect-MgGraph` с помощью новых областей разрешений.

## <a name="call-microsoft-graph"></a>Вызов Microsoft Graph

Теперь, когда вы подписаны, вы можете начать звонить в Microsoft Graph.

### <a name="get-the-signed-in-user"></a>Get the signed-in user

В этом разделе вы найдете пользователя, вписав его, и получите его пользовательский ID. Это необходимо для использования в качестве параметра для других команд, которые будут использовать позже. Начните с запуска следующей команды.

```powershell
Get-MgUser
```

Это выводит список пользователей в вашей Microsoft 365 организации.

```powershell
Id                                   DisplayName              Mail                                  UserPrincipalName
--                                   -----------              ----                                  -----------------
88d1ba68-8ff5-4de2-90ed-768c00abcfae Conf Room Adams          Adams@contoso.onmicrosoft.com         Adams@contoso.…
3103c7b9-cfe6-4cd3-a696-f88909b9a609 Adele Vance              AdeleV@contoso.OnMicrosoft.com        AdeleV@contoso…
da3a885e-2d97-41de-9347-5271ef321b58 MOD Administrator        admin@contoso.OnMicrosoft.com         admin@contoso.…
e0c6ee40-e105-476d-9597-acd061d21fcb Alex Wilber              AlexW@contoso.OnMicrosoft.com         AlexW@contoso.…
17c6bdee-8ed3-49af-a65e-71b64cca8382 Allan Deyoung            AllanD@contoso.OnMicrosoft.com        AllanD@contoso…
e5b78950-27cd-4f01-b083-eab4da97ca6a Conf Room Baker          Baker@contoso.onmicrosoft.com         Baker@contoso.…
40467725-1a58-495d-9e2f-5970c6306d8d Bianca Pisani                                                  BiancaP@contoso…
ce73bdb5-bf12-405e-ab85-40122fdd6eb7 Brian Johnson (TAILSPIN) BrianJ@contoso.onmicrosoft.com        BrianJ@contoso…
df1347a3-7ce7-4b4d-8aab-7c65b5c907b9 Cameron White                                                  CameronW@contoso…
```

Вы можете использовать [фильтр OData,](../query-parameters.md#filter-parameter) чтобы помочь найти нужного пользователя. Запустите следующую команду, заменив имя пользователя, с которого `Megan Bowen` вы подписались.

```powershell
$user = Get-MgUser -Filter "displayName eq 'Megan Bowen'"
```

Убедитесь, что сработало, введите следующее.

```powershell
$user.DisplayName
```

### <a name="list-the-users-joined-teams"></a>Список присоединились к пользователю Teams

Теперь используйте ID пользователя в качестве параметра для `Get-MgUserJoinedTeam` команды.

```powershell
Get-MgUserJoinedTeam -UserId $user.Id
```

Так же, `Get-MgUser` как и в команде, это дает список Teams. Выберите один из присоединяемого пользователя Teams и используйте его для `DisplayName` фильтрации списка.

```powershell
$team = Get-MgUserJoinedTeam -UserId $user.Id -Filter "displayName eq 'Sales and Marketing'"
```

### <a name="list-team-channels"></a>Каналы list Team

Теперь используйте ID команды в качестве параметра для команды, следуя аналогичной схеме перечисления всех каналов, затем фильтруя список, чтобы получить нужный `Get-MgTeamChannel` канал.

```powershell
Get-MgTeamChannel -TeamId $team.Id
$channel = Get-MgTeamChannel -TeamId $team.Id -Filter "displayName eq 'General'"
```

### <a name="send-a-message"></a>Отправка сообщения

Теперь, когда у вас есть ИД команды и ИД канала, вы можете отправить сообщение на канал. Для отправки сообщения используйте следующую команду.

```powershell
New-MgTeamChannelMessage -TeamId $team.Id -ChannelId $channel.Id -Body @{ Content="Hello World" }
```

Эта команда отличается от предыдущих команд, которые вы использовали. Вместо того чтобы просто запрашивать данные, он фактически создает что-то. В microsoft Graph это переводится как HTTP, и для этого требуется объект `POST` в теле этой должности. В этом случае объектом является [chatMessage.](/graph/resources/chatmessage?view=graph-rest-1.0&preserve-view=true) Обратите внимание, `-Body` что параметр командной карты для `body` свойства на `chatMessage` . Другие свойства соедаются аналогичным образом, поэтому вы можете изменить отправимые сообщения. Например, для отправки экстренного сообщения используйте следующую команду.

```powershell
New-MgTeamChannelMessage -TeamId $team.Id -ChannelId $channel.Id -Body @{ Content="Hello World" } -Importance "urgent"
```

### <a name="sign-out"></a>Sign out

Чтобы `Disconnect-MgGraph` выйти из нее, используйте команду.

```powershell
Disconnect-MgGraph
```

## <a name="next-steps"></a>Дальнейшие действия

- [Узнайте, как перемещаться по SDK](navigating.md)
- [Использование проверки подлинности только для приложений с помощью SDK microsoft Graph PowerShell](app-only.md)
