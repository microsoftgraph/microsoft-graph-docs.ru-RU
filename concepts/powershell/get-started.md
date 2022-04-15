---
title: Начало работы с пакетом SDK Microsoft Graph PowerShell
description: начало работы с пакетом SDK Microsoft Graph PowerShell, используя его для выполнения некоторых основных задач.
ms.localizationpriority: medium
author: jasonjoh
ms.openlocfilehash: d92a6057b9c7df7df4f9a7014df20e7a21bfe923
ms.sourcegitcommit: 19558bd9de9b717e7a36bfce1d6d84d0132e2697
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/15/2022
ms.locfileid: "64883397"
---
# <a name="get-started-with-the-microsoft-graph-powershell-sdk"></a>Начало работы с пакетом SDK Microsoft Graph PowerShell

В этом руководстве вы будете использовать пакет SDK Microsoft Graph PowerShell для выполнения некоторых основных задач. Если вы еще не установили [пакет SDK](installation.md), сделайте это перед выполнением этого руководства.

## <a name="api-version"></a>Версия API

По умолчанию пакет SDK использует [REST API Microsoft Graph версии 1.0](/graph/api/overview?view=graph-rest-1.0&preserve-view=true). Это можно изменить с помощью команды `Select-MgProfile` .

```powershell
Select-MgProfile -Name "beta"
```

## <a name="authentication"></a>Проверка подлинности

Пакет SDK powerShell поддерживает два типа проверки подлинности: делегированный доступ и доступ только для приложений. В этом руководстве вы будете использовать делегированный доступ для входа в систему от имени пользователя, предоставить пакету SDK согласие на действия от вашего имени и вызвать microsoft Graph.

Дополнительные сведения об использовании доступа только для приложений для автоматических сценариев см. в статье "Использование проверки подлинности только для приложений с помощью пакета [SDK PowerShell Graph](app-only.md) Microsoft Graph".

### <a name="determine-required-permission-scopes"></a>Определение необходимых областей разрешений

Каждый API в microsoft Graph защищен одной или несколькими областями разрешений. Пользователь, войдите в систему, должен дать согласие на одну из необходимых областей для API, которые вы планируете использовать. В этом примере мы будем использовать следующие API.

- [Вывод списка пользователей](/graph/api/user-list?view=graph-rest-1.0&preserve-view=true) для поиска идентификатора пользователя, выполнив вход
- [Перечисление joinedTeams](/graph/api/user-list-joinedteams?view=graph-rest-1.0&preserve-view=true) для Teams, в который входит пользователь.
- [Список каналов](/graph/api/channel-list?view=graph-rest-1.0&preserve-view=true) для получения каналов в команде.
- [Отправка](/graph/api/channel-post-messages?view=graph-rest-1.0&preserve-view=true) сообщения для отправки сообщения в канал группы.

Область `User.Read.All` разрешений включает первые два вызова, `Group.ReadWrite.All` а остальные — область. Для этих разрешений требуется учетная запись администратора.

### <a name="sign-in"></a>Выполните вход

Используйте команду `Connect-MgGraph` для входа с необходимыми областями. Вам потребуется войти с помощью учетной записи администратора, чтобы дать согласие на необходимые области.

```powershell
Connect-MgGraph -Scopes "User.Read.All","Group.ReadWrite.All"
```

Команда предложит перейти на веб-страницу для входа с помощью кода устройства. После этого команда сообщает об успешном выполнении сообщения `Welcome To Microsoft Graph!` . Это необходимо сделать только один раз для каждого сеанса.

> [!TIP]
> Вы можете добавить дополнительные разрешения, повторив команду `Connect-MgGraph` с новыми областями разрешений.

## <a name="call-microsoft-graph"></a>Вызов Microsoft Graph

Теперь, когда вы вошли в систему, вы можете начать совершать вызовы в Microsoft Graph.

[!INCLUDE [aad-advanced-queries-note](../../includes/aad-advanced-queries-note.md)]

### <a name="get-the-signed-in-user"></a>Получение пользователя, выполнившего вход

В этом разделе описано, как найти пользователя, выполнившего вход, и получить его идентификатор. Он понадобится для использования в качестве параметра для других команд, которые будут использоваться позже. Начните с выполнения следующей команды.

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

Вы можете использовать [фильтр OData,](../query-parameters.md#filter-parameter) чтобы найти нужного пользователя. Выполните следующую команду, заменив `Megan Bowen` отображаемое имя пользователя, выполнившего вход.

```powershell
$user = Get-MgUser -Filter "displayName eq 'Megan Bowen'"
```

Убедитесь, что сработало, введя следующую команду.

```powershell
$user.DisplayName
```

### <a name="list-the-users-joined-teams"></a>Вывод списка команд, присоединенных к пользователю

Теперь используйте идентификатор пользователя в качестве параметра для команды `Get-MgUserJoinedTeam` .

```powershell
Get-MgUserJoinedTeam -UserId $user.Id
```

Как и в случае `Get-MgUser` с командой, вы можете получить список команд. Выберите одну из команд, присоединенных к пользователю, и скопируйте ее `Id`.

### <a name="list-team-channels"></a>Перечисление каналов группы

Теперь используйте идентификатор команды `Get-MgTeamChannel` в качестве параметра для команды, следуя аналогичному шаблону перечисления всех каналов, а затем отфильтруйте список, чтобы получить нужный канал.

```powershell
Get-MgTeamChannel -TeamId $team.Id
$channel = Get-MgTeamChannel -TeamId ID_FROM_PREVIOUS_STEP -Filter "displayName eq 'General'"
```

### <a name="send-a-message"></a>Отправка сообщения

Теперь, когда у вас есть идентификатор команды и идентификатор канала, вы можете опубликовать сообщение в канале. Для отправки сообщения используйте следующую команду.

```powershell
New-MgTeamChannelMessage -TeamId $team.Id -ChannelId $channel.Id -Body @{ Content="Hello World" }
```

Эта команда отличается от предыдущих команд, которые вы использовали. Вместо того чтобы просто запрашивать данные, он фактически создает что-то. В Microsoft Graph это преобразуется в HTTP`POST`, и для этого требуется объект в тексте этой записи. В этом случае объектом является [chatMessage](/graph/resources/chatmessage?view=graph-rest-1.0&preserve-view=true). Обратите внимание, что `-Body` параметр с командой сопоставляется со свойством `body` в `chatMessage`. Другие свойства сопоставляются аналогичным образом, поэтому вы можете изменить отправленное сообщение. Например, чтобы отправить срочное сообщение, используйте следующую команду.

```powershell
New-MgTeamChannelMessage -TeamId $team.Id -ChannelId $channel.Id -Body @{ Content="Hello World" } -Importance "urgent"
```

### <a name="sign-out"></a>Выход

Используйте команду `Disconnect-MgGraph` , чтобы выйти из системы.

```powershell
Disconnect-MgGraph
```

## <a name="next-steps"></a>Дальнейшие действия

- [Узнайте, как перемещаться по пакету SDK](navigating.md)
- [Использование проверки подлинности только для приложений с помощью пакета SDK Microsoft Graph PowerShell](app-only.md)
