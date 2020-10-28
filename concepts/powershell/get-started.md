---
title: Начало работы с пакетом SDK PowerShell для Microsoft Graph
description: Приступая к работе с пакетом SDK PowerShell для Microsoft Graph, используя его, выполните некоторые основные задачи.
localization_priority: Normal
author: jasonjoh
ms.openlocfilehash: eeeaee7bf45e3b8d17f866425556102eef2c1cae
ms.sourcegitcommit: 60ced1be6ed8dd2d23263090a1cfbc16689bb043
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/28/2020
ms.locfileid: "48782888"
---
# <a name="get-started-with-the-microsoft-graph-powershell-sdk"></a>Начало работы с пакетом SDK PowerShell для Microsoft Graph

В этом руководстве описывается использование SDK Microsoft Graph PowerShell для выполнения некоторых основных задач. Если вы еще не [установили пакет SDK](installation.md), сделайте это, прежде чем приступить к работе с этим руководством.

## <a name="api-version"></a>Версия API

По умолчанию пакет SDK использует [REST API Microsoft Graph версии 1.0](/graph/api/overview?view=graph-rest-1.0). Его можно изменить с помощью `Select-MgProfile` команды.

```powershell
Select-MgProfile -Name "beta"
```

## <a name="authentication"></a>Проверка подлинности

Пакет SDK для PowerShell поддерживает два типа проверки подлинности: делегированный доступ и доступ только для приложений. В этом руководстве вы будете использовать делегированный доступ для входа в качестве пользователя, предоставления согласия с пакетом SDK для выполнения действий от вашего имени и вызова Microsoft Graph.

Дополнительные сведения об использовании доступа только к приложениям для автоматических сценариев можно найти в [статье Использование проверки подлинности только для приложений с помощью SDK Microsoft Graph PowerShell](app-only.md).

### <a name="determine-required-permission-scopes"></a>Определение необходимых областей разрешений

Каждый API в Microsoft Graph защищен одной или несколькими областями разрешений. Пользователь, вошедшего в систему, должен согласиться с одной из требуемых областей для API, которые планируется использовать. В этом примере мы будем использовать указанные ниже API.

- [Перечисление пользователей](/graph/api/user-list?view=graph-rest-1.0) , чтобы найти идентификатор пользователя, вошедшего в систему
- [Список жоинедтеамс](/graph/api/user-list-joinedteams?view=graph-rest-1.0) для получения команд, участником которых является пользователь.
- [Перечислите каналы](/graph/api/channel-list?view=graph-rest-1.0) , чтобы получить каналы в команде.
- [Отправьте сообщение](/graph/api/channel-post-messages?view=graph-rest-1.0) , чтобы отправить сообщение в канал команд.

`User.Read.All`Область разрешений включит первые два вызова, а `Group.ReadWrite.All` область будет включать функцию REST. Для этих разрешений требуется учетная запись администратора.

### <a name="sign-in"></a>Вход

Используйте `Connect-MgGraph` команду для входа с использованием требуемых областей. Необходимо войти в учетную запись администратора, чтобы получить согласие на требуемые области.

```powershell
Connect-MgGraph -Scopes "User.Read.All","Group.ReadWrite.All"
```

В командной строке предлагается перейти на веб-страницу, чтобы войти в систему с помощью кода устройства. После этого команда указывает на успешное выполнение с `Welcome To Microsoft Graph!` сообщением. Это необходимо сделать только один раз для каждого сеанса.

> [!TIP]
> Чтобы добавить дополнительные разрешения, повторите `Connect-MgGraph` команду с новыми областями разрешений.

## <a name="call-microsoft-graph"></a>Вызов Microsoft Graph

Теперь, когда вы вошли в систему, вы можете начать совершать вызовы в Microsoft Graph.

### <a name="get-the-signed-in-user"></a>Получение пользователя, выполнившего вход

В этом разделе описывается, как найти пользователя, выполнившего вход, и получить идентификатор пользователя. Вам потребуется использовать в качестве параметра другие команды, которые будут использоваться позже. Начните с запуска следующей команды.

```powershell
Get-MgUser
```

При этом выводится список пользователей в организации Microsoft 365.

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

Вы можете использовать [Фильтр OData](../query-parameters.md#filter-parameter) , чтобы помочь вам определить требуемого пользователя. Выполните следующую команду, заменив `Megan Bowen` Отображаемое имя пользователя, с которым вы выполнили вход.

```powershell
$user = Get-MgUser -Filter "displayName eq 'Megan Bowen'"
```

Для проверки работоспособности введите следующее:

```powershell
$user.DisplayName
```

### <a name="list-the-users-joined-teams"></a>Перечисление связанных с пользователем групп

Теперь используйте идентификатор пользователя в качестве параметра для `Get-MgUserJoinedTeam` команды.

```powershell
Get-MgUserJoinedTeam -UserId $user.Id
```

Как и в `Get-MgUser` случае команды, он предоставляет список команд. Выберите одну из присоединенных к группе пользователей и используйте ее `DisplayName` для фильтрации списка.

```powershell
$team = Get-MgUserJoinedTeam -UserId $user.Id -Filter "displayName eq 'Sales and Marketing'"
```

### <a name="list-team-channels"></a>Перечисление каналов группы

Теперь используйте идентификатор группы в качестве параметра `Get-MgTeamChannel` команды, следуя аналогичным шаблонам для перечисления всех каналов, а затем отфильтруя список, чтобы получить нужный канал.

```powershell
Get-MgTeamChannel -TeamId $team.Id
$channel = Get-MgTeamChannel -TeamId $team.Id -Filter "displayName eq 'General'"
```

### <a name="send-a-message"></a>Отправка сообщения

Теперь, когда у вас есть идентификатор группы и идентификатор канала, вы можете разместить сообщение в канале. Используйте следующую команду для отправки сообщения.

```powershell
New-MgTeamChannelMessage -TeamId $team.Id -ChannelId $channel.Id -Body @{ Content="Hello World" }
```

Эта команда отличается от предыдущих используемых команд. Вместо того чтобы запрашивать данные, фактически создается что-то. В Microsoft Graph это преобразование в HTTP `POST` и требует наличия объекта в теле этой записи. В этом случае объект является [chatMessage](/graph/resources/chatmessage?view=graph-rest-1.0). Обратите внимание, что `-Body` параметр для команды сопоставлен со `body` свойством `chatMessage` . Другие свойства сопоставляются подобным образом, поэтому вы можете изменить отправляемое сообщение. Например, чтобы отправить срочное сообщение, используйте следующую команду:

```powershell
New-MgTeamChannelMessage -TeamId $team.Id -ChannelId $channel.Id -Body @{ Content="Hello World" } -Importance "urgent"
```

## <a name="next-steps"></a>Дальнейшие действия

- [Узнайте, как перейти к пакету SDK](navigating.md)
- [Использование проверки подлинности только для приложений с помощью SDK Microsoft Graph PowerShell](app-only.md)
