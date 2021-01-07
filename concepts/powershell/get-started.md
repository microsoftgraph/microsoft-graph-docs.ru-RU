---
title: Начало работы с Microsoft Graph PowerShell SDK
description: Приступить к работе с Microsoft Graph PowerShell SDK, используя его для выполнения некоторых основных задач.
localization_priority: Normal
author: jasonjoh
ms.openlocfilehash: 6f5ee22960f9bf33156807f9f55f49e6e4aa17b5
ms.sourcegitcommit: 7732d20bd99a125118f7cea146c3f2416879f949
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/07/2021
ms.locfileid: "49777577"
---
# <a name="get-started-with-the-microsoft-graph-powershell-sdk"></a>Начало работы с Microsoft Graph PowerShell SDK

В этом руководстве вы будете использовать Microsoft Graph PowerShell SDK для выполнения некоторых основных задач. Если вы еще не установили [SDK,](installation.md)сделайте это перед тем, как следовать этому руководству.

## <a name="api-version"></a>Версия API

По умолчанию SDK использует [REST API Microsoft Graph 1.0.](/graph/api/overview?view=graph-rest-1.0&preserve-view=true) Это можно изменить с помощью `Select-MgProfile` команды.

```powershell
Select-MgProfile -Name "beta"
```

## <a name="authentication"></a>Проверка подлинности

SDK PowerShell поддерживает два типа проверки подлинности: делегированную проверку подлинности и доступ только для приложений. В этом руководстве вы будете использовать делегирование доступа для входа в качестве пользователя, предоставить SDK согласие на действия от вашего имени и вызвать Microsoft Graph.

Подробные сведения об использовании доступа только для приложений для сценариев с использованием службы проверки подлинности только для приложений см. в microsoft [Graph PowerShell SDK.](app-only.md)

### <a name="determine-required-permission-scopes"></a>Определение необходимых областей разрешений

Каждый API в Microsoft Graph защищен одной или более областью разрешений. Войдя в систему, пользователь должен согласиться на одну из необходимых областей для API, которые вы планируете использовать. В этом примере мы будем использовать следующие API.

- [Список пользователей,](/graph/api/user-list?view=graph-rest-1.0&preserve-view=true) которые могут найти ИД войдите в систему
- [Список joinedTeams,](/graph/api/user-list-joinedteams?view=graph-rest-1.0&preserve-view=true) чтобы получить Teams, в который входит пользователь.
- [Список каналов](/graph/api/channel-list?view=graph-rest-1.0&preserve-view=true) для получения каналов в команде.
- [Отправьте сообщение](/graph/api/channel-post-messages?view=graph-rest-1.0&preserve-view=true) для отправки сообщения в канал группы.

Область разрешений включает первые два вызова, а остальные `User.Read.All` `Group.ReadWrite.All` вызовы включает область. Для этих разрешений требуется учетная запись администратора.

### <a name="sign-in"></a>Вход

Используйте команду `Connect-MgGraph` для входов с требуемой областью. Вам потребуется войти с помощью учетной записи администратора, чтобы согласиться на необходимые области.

```powershell
Connect-MgGraph -Scopes "User.Read.All","Group.ReadWrite.All"
```

Команда позволяет перейти на веб-страницу, чтобы войти с помощью кода устройства. После этого команда указывает на успех `Welcome To Microsoft Graph!` сообщения. Это необходимо сделать только один раз в сеансе.

> [!TIP]
> Можно добавить дополнительные разрешения, повторив команду с `Connect-MgGraph` новыми разрешениями.

## <a name="call-microsoft-graph"></a>Вызов Microsoft Graph

Теперь, когда вы вписались, вы можете начать звонить в Microsoft Graph.

### <a name="get-the-signed-in-user"></a>Get the signed-in user

В этом разделе вы найдете войдите пользователя и получите его ИД пользователя. Это необходимо для использования в качестве параметра для других команд, которые вы будете использовать позже. Для начала запустите следующую команду.

```powershell
Get-MgUser
```

Это выводит список пользователей в вашей организации Microsoft 365.

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

Вы можете использовать [фильтр OData для](../query-parameters.md#filter-parameter) поиска нужного пользователя. Запустите следующую команду, заменив отображаемую именем пользователя, с которого вы `Megan Bowen` вписались.

```powershell
$user = Get-MgUser -Filter "displayName eq 'Megan Bowen'"
```

Убедитесь, что все сработало, введите следующую информацию.

```powershell
$user.DisplayName
```

### <a name="list-the-users-joined-teams"></a>Список пользователей, которые присоединились к Teams

Теперь используйте в команде в качестве параметра ИД `Get-MgUserJoinedTeam` пользователя.

```powershell
Get-MgUserJoinedTeam -UserId $user.Id
```

Так `Get-MgUser` же, как и команда, вы предоставляете список Teams. Выберите один из пользователей, присоединив Teams, и используйте его для `DisplayName` фильтрации списка.

```powershell
$team = Get-MgUserJoinedTeam -UserId $user.Id -Filter "displayName eq 'Sales and Marketing'"
```

### <a name="list-team-channels"></a>Список каналов группы

Теперь используйте в команде в качестве параметра ИД команды, следуя аналогичной схеме перечисления всех каналов, а затем отфильтруя список, чтобы получить нужный `Get-MgTeamChannel` канал.

```powershell
Get-MgTeamChannel -TeamId $team.Id
$channel = Get-MgTeamChannel -TeamId $team.Id -Filter "displayName eq 'General'"
```

### <a name="send-a-message"></a>Отправка сообщения

Теперь, когда у вас есть ИД команды и ИД канала, вы можете опубликовать сообщение в канале. Для отправки сообщения используйте следующую команду.

```powershell
New-MgTeamChannelMessage -TeamId $team.Id -ChannelId $channel.Id -Body @{ Content="Hello World" }
```

Эта команда отличается от предыдущих команд, которые вы использовали. Вместо запроса данных фактически создается что-то. В Microsoft Graph это преобразуется в HTTP, и для него требуется объект `POST` в тексте этой записи. В этом случае объектом является [chatMessage.](/graph/resources/chatmessage?view=graph-rest-1.0&preserve-view=true) Обратите `-Body` внимание, что параметр с командой сопомечает `body` свойство `chatMessage` on. Другие свойства сослаться аналогичным образом, поэтому вы можете изменить сообщение, которое вы отправляете. Например, чтобы отправить экстренное сообщение, используйте следующую команду.

```powershell
New-MgTeamChannelMessage -TeamId $team.Id -ChannelId $channel.Id -Body @{ Content="Hello World" } -Importance "urgent"
```

### <a name="sign-out"></a>Выход

Используйте `Disconnect-MgGraph` команду, чтобы выйти из нее.

```powershell
Disconnect-MgGraph
```

## <a name="next-steps"></a>Дальнейшие действия

- [Узнайте, как перемещаться по SDK](navigating.md)
- [Использование проверки подлинности только для приложений с помощью Microsoft Graph PowerShell SDK](app-only.md)
