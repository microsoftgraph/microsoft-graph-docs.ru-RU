---
title: Начало работы с пакетом SDK PowerShell для Microsoft Graph
description: Приступая к работе с пакетом SDK PowerShell для Microsoft Graph, используя его, выполните некоторые основные задачи.
localization_priority: Normal
author: jasonjoh
ms.openlocfilehash: ab4a0c5a65dc752116d3622f71e024e039d90675
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193780"
---
# <a name="get-started-with-the-microsoft-graph-powershell-sdk"></a><span data-ttu-id="f9b8c-103">Начало работы с пакетом SDK PowerShell для Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="f9b8c-103">Get started with the Microsoft Graph PowerShell SDK</span></span>

<span data-ttu-id="f9b8c-104">В этом руководстве описывается использование SDK Microsoft Graph PowerShell для выполнения некоторых основных задач.</span><span class="sxs-lookup"><span data-stu-id="f9b8c-104">In this guide you'll use the Microsoft Graph PowerShell SDK to perform some basic tasks.</span></span> <span data-ttu-id="f9b8c-105">Если вы еще не [установили пакет SDK](installation.md), сделайте это, прежде чем приступить к работе с этим руководством.</span><span class="sxs-lookup"><span data-stu-id="f9b8c-105">If you haven't already [installed the SDK](installation.md), please do so before following this guide.</span></span>

## <a name="api-version"></a><span data-ttu-id="f9b8c-106">Версия API</span><span class="sxs-lookup"><span data-stu-id="f9b8c-106">API version</span></span>

<span data-ttu-id="f9b8c-107">По умолчанию пакет SDK использует [REST API Microsoft Graph версии 1.0](/graph/api/overview?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="f9b8c-107">By default, the SDK uses the [Microsoft Graph REST API v1.0](/graph/api/overview?view=graph-rest-1.0).</span></span> <span data-ttu-id="f9b8c-108">Его можно изменить с помощью `Select-MgProfile` команды.</span><span class="sxs-lookup"><span data-stu-id="f9b8c-108">You can change this by using the `Select-MgProfile` command.</span></span>

```powershell
Select-MgProfile -Name "beta"
```

## <a name="authentication"></a><span data-ttu-id="f9b8c-109">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="f9b8c-109">Authentication</span></span>

<span data-ttu-id="f9b8c-110">Пакет SDK для PowerShell поддерживает два типа проверки подлинности: делегированный доступ и доступ только для приложений.</span><span class="sxs-lookup"><span data-stu-id="f9b8c-110">The PowerShell SDK supports two types of authentication: delegated access, and app-only access.</span></span> <span data-ttu-id="f9b8c-111">В этом руководстве вы будете использовать делегированный доступ для входа в качестве пользователя, предоставления согласия с пакетом SDK для выполнения действий от вашего имени и вызова Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f9b8c-111">In this guide, you will use delegated access to login as a user, grant consent to the SDK to act on your behalf, and call the Microsoft Graph.</span></span>

<span data-ttu-id="f9b8c-112">Дополнительные сведения об использовании доступа только к приложениям для автоматических сценариев можно найти в [статье Использование проверки подлинности только для приложений с помощью SDK Microsoft Graph PowerShell](app-only.md).</span><span class="sxs-lookup"><span data-stu-id="f9b8c-112">For details on using app-only access for unattended scenarios, see [Use app-only authentication with the Microsoft Graph PowerShell SDK](app-only.md).</span></span>

### <a name="determine-required-permission-scopes"></a><span data-ttu-id="f9b8c-113">Определение необходимых областей разрешений</span><span class="sxs-lookup"><span data-stu-id="f9b8c-113">Determine required permission scopes</span></span>

<span data-ttu-id="f9b8c-114">Каждый API в Microsoft Graph защищен одной или несколькими областями разрешений.</span><span class="sxs-lookup"><span data-stu-id="f9b8c-114">Each API in the Microsoft Graph is protected by one or more permission scopes.</span></span> <span data-ttu-id="f9b8c-115">Пользователь, вошедшего в систему, должен согласиться с одной из требуемых областей для API, которые планируется использовать.</span><span class="sxs-lookup"><span data-stu-id="f9b8c-115">The user logging in must consent to one of the required scopes for the APIs you plan to use.</span></span> <span data-ttu-id="f9b8c-116">В этом примере мы будем использовать указанные ниже API.</span><span class="sxs-lookup"><span data-stu-id="f9b8c-116">In this example, we'll use the following APIs.</span></span>

- <span data-ttu-id="f9b8c-117">[Перечисление пользователей](/graph/api/user-list?view=graph-rest-1.0) , чтобы найти идентификатор пользователя, вошедшего в систему</span><span class="sxs-lookup"><span data-stu-id="f9b8c-117">[List users](/graph/api/user-list?view=graph-rest-1.0) to find the user ID of the logged-in user</span></span>
- <span data-ttu-id="f9b8c-118">[Список жоинедтеамс](/graph/api/user-list-joinedteams?view=graph-rest-1.0) для получения команд, участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="f9b8c-118">[List joinedTeams](/graph/api/user-list-joinedteams?view=graph-rest-1.0) to get the Teams the user is a member of.</span></span>
- <span data-ttu-id="f9b8c-119">[Перечислите каналы](/graph/api/channel-list?view=graph-rest-1.0) , чтобы получить каналы в команде.</span><span class="sxs-lookup"><span data-stu-id="f9b8c-119">[List channels](/graph/api/channel-list?view=graph-rest-1.0) to get the channels in a Team.</span></span>
- <span data-ttu-id="f9b8c-120">[Отправьте сообщение](/graph/api/channel-post-messages?view=graph-rest-1.0) , чтобы отправить сообщение в канал команд.</span><span class="sxs-lookup"><span data-stu-id="f9b8c-120">[Send message](/graph/api/channel-post-messages?view=graph-rest-1.0) to send a message to a Team channel.</span></span>

<span data-ttu-id="f9b8c-121">`User.Read.All`Область разрешений включит первые два вызова, а `Group.ReadWrite.All` область будет включать функцию REST.</span><span class="sxs-lookup"><span data-stu-id="f9b8c-121">The `User.Read.All` permission scope will enable the first two calls, and the `Group.ReadWrite.All` scope will enable the rest.</span></span> <span data-ttu-id="f9b8c-122">Для этих разрешений требуется учетная запись администратора.</span><span class="sxs-lookup"><span data-stu-id="f9b8c-122">These permissions require an admin account.</span></span>

### <a name="sign-in"></a><span data-ttu-id="f9b8c-123">Вход</span><span class="sxs-lookup"><span data-stu-id="f9b8c-123">Sign in</span></span>

<span data-ttu-id="f9b8c-124">Используйте `Connect-Graph` команду для входа с использованием требуемых областей.</span><span class="sxs-lookup"><span data-stu-id="f9b8c-124">Use the `Connect-Graph` command to sign in with the required scopes.</span></span> <span data-ttu-id="f9b8c-125">Необходимо войти в учетную запись администратора, чтобы получить согласие на требуемые области.</span><span class="sxs-lookup"><span data-stu-id="f9b8c-125">You'll need to sign in with an admin account to consent to the required scopes.</span></span>

```powershell
Connect-Graph -Scopes "User.Read.All","Group.ReadWrite.All"
```

<span data-ttu-id="f9b8c-126">В командной строке предлагается перейти на веб-страницу, чтобы войти в систему с помощью кода устройства.</span><span class="sxs-lookup"><span data-stu-id="f9b8c-126">The command prompts you to go to a web page to sign in using a device code.</span></span> <span data-ttu-id="f9b8c-127">После этого команда указывает на успешное выполнение с `Welcome To Microsoft Graph!` сообщением.</span><span class="sxs-lookup"><span data-stu-id="f9b8c-127">Once you've done that, the command indicates success with a `Welcome To Microsoft Graph!` message.</span></span> <span data-ttu-id="f9b8c-128">Это необходимо сделать только один раз для каждого сеанса.</span><span class="sxs-lookup"><span data-stu-id="f9b8c-128">You only need to do this once per session.</span></span>

> [!TIP]
> <span data-ttu-id="f9b8c-129">Чтобы добавить дополнительные разрешения, повторите `Connect-Graph` команду с новыми областями разрешений.</span><span class="sxs-lookup"><span data-stu-id="f9b8c-129">You can add additional permissions by repeating the `Connect-Graph` command with the new permission scopes.</span></span>

## <a name="call-microsoft-graph"></a><span data-ttu-id="f9b8c-130">Вызов Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="f9b8c-130">Call Microsoft Graph</span></span>

<span data-ttu-id="f9b8c-131">Теперь, когда вы вошли в систему, вы можете начать совершать вызовы в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f9b8c-131">Now that you're signed in, you can start making calls to Microsoft Graph.</span></span>

### <a name="get-the-signed-in-user"></a><span data-ttu-id="f9b8c-132">Получение пользователя, выполнившего вход</span><span class="sxs-lookup"><span data-stu-id="f9b8c-132">Get the signed-in user</span></span>

<span data-ttu-id="f9b8c-133">В этом разделе описывается, как найти пользователя, выполнившего вход, и получить идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="f9b8c-133">In this section you'll locate the signed-in user and get her user ID.</span></span> <span data-ttu-id="f9b8c-134">Вам потребуется использовать в качестве параметра другие команды, которые будут использоваться позже.</span><span class="sxs-lookup"><span data-stu-id="f9b8c-134">You'll need that to use as a parameter to the other commands you'll use later.</span></span> <span data-ttu-id="f9b8c-135">Начните с запуска следующей команды.</span><span class="sxs-lookup"><span data-stu-id="f9b8c-135">Start by running the following command.</span></span>

```powershell
Get-MgUser
```

<span data-ttu-id="f9b8c-136">При этом выводится список пользователей в организации Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="f9b8c-136">This outputs a listing of users in your Microsoft 365 organization.</span></span>

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

<span data-ttu-id="f9b8c-137">Вы можете использовать [Фильтр OData](../query-parameters.md#filter-parameter) , чтобы помочь вам определить требуемого пользователя.</span><span class="sxs-lookup"><span data-stu-id="f9b8c-137">You can use an [OData filter](../query-parameters.md#filter-parameter) to help locate the specific user you want.</span></span> <span data-ttu-id="f9b8c-138">Выполните следующую команду, заменив `Megan Bowen` Отображаемое имя пользователя, с которым вы выполнили вход.</span><span class="sxs-lookup"><span data-stu-id="f9b8c-138">Run the following command, replacing `Megan Bowen` with the display name of the user you signed in with.</span></span>

```powershell
$user = Get-MgUser -Filter "displayName eq 'Megan Bowen'"
```

<span data-ttu-id="f9b8c-139">Для проверки работоспособности введите следующее:</span><span class="sxs-lookup"><span data-stu-id="f9b8c-139">Verify that worked by entering the following.</span></span>

```powershell
$user.DisplayName
```

### <a name="list-the-users-joined-teams"></a><span data-ttu-id="f9b8c-140">Перечисление связанных с пользователем групп</span><span class="sxs-lookup"><span data-stu-id="f9b8c-140">List the user's joined Teams</span></span>

<span data-ttu-id="f9b8c-141">Теперь используйте идентификатор пользователя в качестве параметра для `Get-MgUserJoinedTeam` команды.</span><span class="sxs-lookup"><span data-stu-id="f9b8c-141">Now use the user's ID as a parameter to the `Get-MgUserJoinedTeam` command.</span></span>

```powershell
Get-MgUserJoinedTeam -UserId $user.Id
```

<span data-ttu-id="f9b8c-142">Как и в `Get-MgUser` случае команды, он предоставляет список команд.</span><span class="sxs-lookup"><span data-stu-id="f9b8c-142">Just like the `Get-MgUser` command, this gives a list of Teams.</span></span> <span data-ttu-id="f9b8c-143">Выберите одну из присоединенных к группе пользователей и используйте ее `DisplayName` для фильтрации списка.</span><span class="sxs-lookup"><span data-stu-id="f9b8c-143">Select one of the user's joined Teams and use its `DisplayName` to filter the list.</span></span>

```powershell
$team = Get-MgUserJoinedTeam -UserId $user.Id -Filter "displayName eq 'Sales and Marketing'"
```

### <a name="list-team-channels"></a><span data-ttu-id="f9b8c-144">Перечисление каналов группы</span><span class="sxs-lookup"><span data-stu-id="f9b8c-144">List Team channels</span></span>

<span data-ttu-id="f9b8c-145">Теперь используйте идентификатор группы в качестве параметра `Get-MgTeamChannel` команды, следуя аналогичным шаблонам для перечисления всех каналов, а затем отфильтруя список, чтобы получить нужный канал.</span><span class="sxs-lookup"><span data-stu-id="f9b8c-145">Now use the Team's ID as a parameter to the `Get-MgTeamChannel` command, following a similar pattern of listing all channels, then filtering the list to get the specific channel you want.</span></span>

```powershell
Get-MgTeamChannel -TeamId $team.Id
$channel = Get-MgTeamChannel -TeamId $team.Id -Filter "displayName eq 'General'"
```

### <a name="send-a-message"></a><span data-ttu-id="f9b8c-146">Отправка сообщения</span><span class="sxs-lookup"><span data-stu-id="f9b8c-146">Send a message</span></span>

<span data-ttu-id="f9b8c-147">Теперь, когда у вас есть идентификатор группы и идентификатор канала, вы можете разместить сообщение в канале.</span><span class="sxs-lookup"><span data-stu-id="f9b8c-147">Now that you have both the Team ID and the channel ID, you can post a message to the channel.</span></span> <span data-ttu-id="f9b8c-148">Используйте следующую команду для отправки сообщения.</span><span class="sxs-lookup"><span data-stu-id="f9b8c-148">Use the following command to send the message.</span></span>

```powershell
New-MgTeamChannelMessage -TeamId $team.Id -ChannelId $channel.Id -Body @{ Content="Hello World" }
```

<span data-ttu-id="f9b8c-149">Эта команда отличается от предыдущих используемых команд.</span><span class="sxs-lookup"><span data-stu-id="f9b8c-149">This command differs from the previous commands you used.</span></span> <span data-ttu-id="f9b8c-150">Вместо того чтобы запрашивать данные, фактически создается что-то.</span><span class="sxs-lookup"><span data-stu-id="f9b8c-150">Instead of just querying data, it's actually creating something.</span></span> <span data-ttu-id="f9b8c-151">В Microsoft Graph это преобразование в HTTP `POST` и требует наличия объекта в теле этой записи.</span><span class="sxs-lookup"><span data-stu-id="f9b8c-151">In Microsoft Graph, this translates to an HTTP `POST`, and it requires an object in the body of that post.</span></span> <span data-ttu-id="f9b8c-152">В этом случае объект является [chatMessage](/graph/resources/chatmessage?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="f9b8c-152">In this case, the object is a [chatMessage](/graph/resources/chatmessage?view=graph-rest-1.0).</span></span> <span data-ttu-id="f9b8c-153">Обратите внимание, что `-Body` параметр для команды сопоставлен со `body` свойством `chatMessage` .</span><span class="sxs-lookup"><span data-stu-id="f9b8c-153">Note that the `-Body` parameter to the command maps to the `body` property on `chatMessage`.</span></span> <span data-ttu-id="f9b8c-154">Другие свойства сопоставляются подобным образом, поэтому вы можете изменить отправляемое сообщение.</span><span class="sxs-lookup"><span data-stu-id="f9b8c-154">Other properties are mapped in a similar way, so you can change the message you send.</span></span> <span data-ttu-id="f9b8c-155">Например, чтобы отправить срочное сообщение, используйте следующую команду:</span><span class="sxs-lookup"><span data-stu-id="f9b8c-155">For example, to send an urgent message use the following command.</span></span>

```powershell
New-MgTeamChannelMessage -TeamId $team.Id -ChannelId $channel.Id -Body @{ Content="Hello World" } -Importance "urgent"
```

## <a name="next-steps"></a><span data-ttu-id="f9b8c-156">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="f9b8c-156">Next steps</span></span>

- [<span data-ttu-id="f9b8c-157">Узнайте, как перейти к пакету SDK</span><span class="sxs-lookup"><span data-stu-id="f9b8c-157">Learn how to navigate the SDK</span></span>](navigating.md)
- [<span data-ttu-id="f9b8c-158">Использование проверки подлинности только для приложений с помощью SDK Microsoft Graph PowerShell</span><span class="sxs-lookup"><span data-stu-id="f9b8c-158">Use app-only authentication with the Microsoft Graph PowerShell SDK</span></span>](app-only.md)
