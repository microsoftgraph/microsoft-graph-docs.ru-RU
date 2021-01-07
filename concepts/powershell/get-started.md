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
# <a name="get-started-with-the-microsoft-graph-powershell-sdk"></a><span data-ttu-id="b3474-103">Начало работы с Microsoft Graph PowerShell SDK</span><span class="sxs-lookup"><span data-stu-id="b3474-103">Get started with the Microsoft Graph PowerShell SDK</span></span>

<span data-ttu-id="b3474-104">В этом руководстве вы будете использовать Microsoft Graph PowerShell SDK для выполнения некоторых основных задач.</span><span class="sxs-lookup"><span data-stu-id="b3474-104">In this guide you'll use the Microsoft Graph PowerShell SDK to perform some basic tasks.</span></span> <span data-ttu-id="b3474-105">Если вы еще не установили [SDK,](installation.md)сделайте это перед тем, как следовать этому руководству.</span><span class="sxs-lookup"><span data-stu-id="b3474-105">If you haven't already [installed the SDK](installation.md), please do so before following this guide.</span></span>

## <a name="api-version"></a><span data-ttu-id="b3474-106">Версия API</span><span class="sxs-lookup"><span data-stu-id="b3474-106">API version</span></span>

<span data-ttu-id="b3474-107">По умолчанию SDK использует [REST API Microsoft Graph 1.0.](/graph/api/overview?view=graph-rest-1.0&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="b3474-107">By default, the SDK uses the [Microsoft Graph REST API v1.0](/graph/api/overview?view=graph-rest-1.0&preserve-view=true).</span></span> <span data-ttu-id="b3474-108">Это можно изменить с помощью `Select-MgProfile` команды.</span><span class="sxs-lookup"><span data-stu-id="b3474-108">You can change this by using the `Select-MgProfile` command.</span></span>

```powershell
Select-MgProfile -Name "beta"
```

## <a name="authentication"></a><span data-ttu-id="b3474-109">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="b3474-109">Authentication</span></span>

<span data-ttu-id="b3474-110">SDK PowerShell поддерживает два типа проверки подлинности: делегированную проверку подлинности и доступ только для приложений.</span><span class="sxs-lookup"><span data-stu-id="b3474-110">The PowerShell SDK supports two types of authentication: delegated access, and app-only access.</span></span> <span data-ttu-id="b3474-111">В этом руководстве вы будете использовать делегирование доступа для входа в качестве пользователя, предоставить SDK согласие на действия от вашего имени и вызвать Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b3474-111">In this guide, you will use delegated access to login as a user, grant consent to the SDK to act on your behalf, and call the Microsoft Graph.</span></span>

<span data-ttu-id="b3474-112">Подробные сведения об использовании доступа только для приложений для сценариев с использованием службы проверки подлинности только для приложений см. в microsoft [Graph PowerShell SDK.](app-only.md)</span><span class="sxs-lookup"><span data-stu-id="b3474-112">For details on using app-only access for unattended scenarios, see [Use app-only authentication with the Microsoft Graph PowerShell SDK](app-only.md).</span></span>

### <a name="determine-required-permission-scopes"></a><span data-ttu-id="b3474-113">Определение необходимых областей разрешений</span><span class="sxs-lookup"><span data-stu-id="b3474-113">Determine required permission scopes</span></span>

<span data-ttu-id="b3474-114">Каждый API в Microsoft Graph защищен одной или более областью разрешений.</span><span class="sxs-lookup"><span data-stu-id="b3474-114">Each API in the Microsoft Graph is protected by one or more permission scopes.</span></span> <span data-ttu-id="b3474-115">Войдя в систему, пользователь должен согласиться на одну из необходимых областей для API, которые вы планируете использовать.</span><span class="sxs-lookup"><span data-stu-id="b3474-115">The user logging in must consent to one of the required scopes for the APIs you plan to use.</span></span> <span data-ttu-id="b3474-116">В этом примере мы будем использовать следующие API.</span><span class="sxs-lookup"><span data-stu-id="b3474-116">In this example, we'll use the following APIs.</span></span>

- <span data-ttu-id="b3474-117">[Список пользователей,](/graph/api/user-list?view=graph-rest-1.0&preserve-view=true) которые могут найти ИД войдите в систему</span><span class="sxs-lookup"><span data-stu-id="b3474-117">[List users](/graph/api/user-list?view=graph-rest-1.0&preserve-view=true) to find the user ID of the logged-in user</span></span>
- <span data-ttu-id="b3474-118">[Список joinedTeams,](/graph/api/user-list-joinedteams?view=graph-rest-1.0&preserve-view=true) чтобы получить Teams, в который входит пользователь.</span><span class="sxs-lookup"><span data-stu-id="b3474-118">[List joinedTeams](/graph/api/user-list-joinedteams?view=graph-rest-1.0&preserve-view=true) to get the Teams the user is a member of.</span></span>
- <span data-ttu-id="b3474-119">[Список каналов](/graph/api/channel-list?view=graph-rest-1.0&preserve-view=true) для получения каналов в команде.</span><span class="sxs-lookup"><span data-stu-id="b3474-119">[List channels](/graph/api/channel-list?view=graph-rest-1.0&preserve-view=true) to get the channels in a Team.</span></span>
- <span data-ttu-id="b3474-120">[Отправьте сообщение](/graph/api/channel-post-messages?view=graph-rest-1.0&preserve-view=true) для отправки сообщения в канал группы.</span><span class="sxs-lookup"><span data-stu-id="b3474-120">[Send message](/graph/api/channel-post-messages?view=graph-rest-1.0&preserve-view=true) to send a message to a Team channel.</span></span>

<span data-ttu-id="b3474-121">Область разрешений включает первые два вызова, а остальные `User.Read.All` `Group.ReadWrite.All` вызовы включает область.</span><span class="sxs-lookup"><span data-stu-id="b3474-121">The `User.Read.All` permission scope will enable the first two calls, and the `Group.ReadWrite.All` scope will enable the rest.</span></span> <span data-ttu-id="b3474-122">Для этих разрешений требуется учетная запись администратора.</span><span class="sxs-lookup"><span data-stu-id="b3474-122">These permissions require an admin account.</span></span>

### <a name="sign-in"></a><span data-ttu-id="b3474-123">Вход</span><span class="sxs-lookup"><span data-stu-id="b3474-123">Sign in</span></span>

<span data-ttu-id="b3474-124">Используйте команду `Connect-MgGraph` для входов с требуемой областью.</span><span class="sxs-lookup"><span data-stu-id="b3474-124">Use the `Connect-MgGraph` command to sign in with the required scopes.</span></span> <span data-ttu-id="b3474-125">Вам потребуется войти с помощью учетной записи администратора, чтобы согласиться на необходимые области.</span><span class="sxs-lookup"><span data-stu-id="b3474-125">You'll need to sign in with an admin account to consent to the required scopes.</span></span>

```powershell
Connect-MgGraph -Scopes "User.Read.All","Group.ReadWrite.All"
```

<span data-ttu-id="b3474-126">Команда позволяет перейти на веб-страницу, чтобы войти с помощью кода устройства.</span><span class="sxs-lookup"><span data-stu-id="b3474-126">The command prompts you to go to a web page to sign in using a device code.</span></span> <span data-ttu-id="b3474-127">После этого команда указывает на успех `Welcome To Microsoft Graph!` сообщения.</span><span class="sxs-lookup"><span data-stu-id="b3474-127">Once you've done that, the command indicates success with a `Welcome To Microsoft Graph!` message.</span></span> <span data-ttu-id="b3474-128">Это необходимо сделать только один раз в сеансе.</span><span class="sxs-lookup"><span data-stu-id="b3474-128">You only need to do this once per session.</span></span>

> [!TIP]
> <span data-ttu-id="b3474-129">Можно добавить дополнительные разрешения, повторив команду с `Connect-MgGraph` новыми разрешениями.</span><span class="sxs-lookup"><span data-stu-id="b3474-129">You can add additional permissions by repeating the `Connect-MgGraph` command with the new permission scopes.</span></span>

## <a name="call-microsoft-graph"></a><span data-ttu-id="b3474-130">Вызов Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b3474-130">Call Microsoft Graph</span></span>

<span data-ttu-id="b3474-131">Теперь, когда вы вписались, вы можете начать звонить в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b3474-131">Now that you're signed in, you can start making calls to Microsoft Graph.</span></span>

### <a name="get-the-signed-in-user"></a><span data-ttu-id="b3474-132">Get the signed-in user</span><span class="sxs-lookup"><span data-stu-id="b3474-132">Get the signed-in user</span></span>

<span data-ttu-id="b3474-133">В этом разделе вы найдете войдите пользователя и получите его ИД пользователя.</span><span class="sxs-lookup"><span data-stu-id="b3474-133">In this section you'll locate the signed-in user and get her user ID.</span></span> <span data-ttu-id="b3474-134">Это необходимо для использования в качестве параметра для других команд, которые вы будете использовать позже.</span><span class="sxs-lookup"><span data-stu-id="b3474-134">You'll need that to use as a parameter to the other commands you'll use later.</span></span> <span data-ttu-id="b3474-135">Для начала запустите следующую команду.</span><span class="sxs-lookup"><span data-stu-id="b3474-135">Start by running the following command.</span></span>

```powershell
Get-MgUser
```

<span data-ttu-id="b3474-136">Это выводит список пользователей в вашей организации Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="b3474-136">This outputs a listing of users in your Microsoft 365 organization.</span></span>

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

<span data-ttu-id="b3474-137">Вы можете использовать [фильтр OData для](../query-parameters.md#filter-parameter) поиска нужного пользователя.</span><span class="sxs-lookup"><span data-stu-id="b3474-137">You can use an [OData filter](../query-parameters.md#filter-parameter) to help locate the specific user you want.</span></span> <span data-ttu-id="b3474-138">Запустите следующую команду, заменив отображаемую именем пользователя, с которого вы `Megan Bowen` вписались.</span><span class="sxs-lookup"><span data-stu-id="b3474-138">Run the following command, replacing `Megan Bowen` with the display name of the user you signed in with.</span></span>

```powershell
$user = Get-MgUser -Filter "displayName eq 'Megan Bowen'"
```

<span data-ttu-id="b3474-139">Убедитесь, что все сработало, введите следующую информацию.</span><span class="sxs-lookup"><span data-stu-id="b3474-139">Verify that worked by entering the following.</span></span>

```powershell
$user.DisplayName
```

### <a name="list-the-users-joined-teams"></a><span data-ttu-id="b3474-140">Список пользователей, которые присоединились к Teams</span><span class="sxs-lookup"><span data-stu-id="b3474-140">List the user's joined Teams</span></span>

<span data-ttu-id="b3474-141">Теперь используйте в команде в качестве параметра ИД `Get-MgUserJoinedTeam` пользователя.</span><span class="sxs-lookup"><span data-stu-id="b3474-141">Now use the user's ID as a parameter to the `Get-MgUserJoinedTeam` command.</span></span>

```powershell
Get-MgUserJoinedTeam -UserId $user.Id
```

<span data-ttu-id="b3474-142">Так `Get-MgUser` же, как и команда, вы предоставляете список Teams.</span><span class="sxs-lookup"><span data-stu-id="b3474-142">Just like the `Get-MgUser` command, this gives a list of Teams.</span></span> <span data-ttu-id="b3474-143">Выберите один из пользователей, присоединив Teams, и используйте его для `DisplayName` фильтрации списка.</span><span class="sxs-lookup"><span data-stu-id="b3474-143">Select one of the user's joined Teams and use its `DisplayName` to filter the list.</span></span>

```powershell
$team = Get-MgUserJoinedTeam -UserId $user.Id -Filter "displayName eq 'Sales and Marketing'"
```

### <a name="list-team-channels"></a><span data-ttu-id="b3474-144">Список каналов группы</span><span class="sxs-lookup"><span data-stu-id="b3474-144">List Team channels</span></span>

<span data-ttu-id="b3474-145">Теперь используйте в команде в качестве параметра ИД команды, следуя аналогичной схеме перечисления всех каналов, а затем отфильтруя список, чтобы получить нужный `Get-MgTeamChannel` канал.</span><span class="sxs-lookup"><span data-stu-id="b3474-145">Now use the Team's ID as a parameter to the `Get-MgTeamChannel` command, following a similar pattern of listing all channels, then filtering the list to get the specific channel you want.</span></span>

```powershell
Get-MgTeamChannel -TeamId $team.Id
$channel = Get-MgTeamChannel -TeamId $team.Id -Filter "displayName eq 'General'"
```

### <a name="send-a-message"></a><span data-ttu-id="b3474-146">Отправка сообщения</span><span class="sxs-lookup"><span data-stu-id="b3474-146">Send a message</span></span>

<span data-ttu-id="b3474-147">Теперь, когда у вас есть ИД команды и ИД канала, вы можете опубликовать сообщение в канале.</span><span class="sxs-lookup"><span data-stu-id="b3474-147">Now that you have both the Team ID and the channel ID, you can post a message to the channel.</span></span> <span data-ttu-id="b3474-148">Для отправки сообщения используйте следующую команду.</span><span class="sxs-lookup"><span data-stu-id="b3474-148">Use the following command to send the message.</span></span>

```powershell
New-MgTeamChannelMessage -TeamId $team.Id -ChannelId $channel.Id -Body @{ Content="Hello World" }
```

<span data-ttu-id="b3474-149">Эта команда отличается от предыдущих команд, которые вы использовали.</span><span class="sxs-lookup"><span data-stu-id="b3474-149">This command differs from the previous commands you used.</span></span> <span data-ttu-id="b3474-150">Вместо запроса данных фактически создается что-то.</span><span class="sxs-lookup"><span data-stu-id="b3474-150">Instead of just querying data, it's actually creating something.</span></span> <span data-ttu-id="b3474-151">В Microsoft Graph это преобразуется в HTTP, и для него требуется объект `POST` в тексте этой записи.</span><span class="sxs-lookup"><span data-stu-id="b3474-151">In Microsoft Graph, this translates to an HTTP `POST`, and it requires an object in the body of that post.</span></span> <span data-ttu-id="b3474-152">В этом случае объектом является [chatMessage.](/graph/resources/chatmessage?view=graph-rest-1.0&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="b3474-152">In this case, the object is a [chatMessage](/graph/resources/chatmessage?view=graph-rest-1.0&preserve-view=true).</span></span> <span data-ttu-id="b3474-153">Обратите `-Body` внимание, что параметр с командой сопомечает `body` свойство `chatMessage` on.</span><span class="sxs-lookup"><span data-stu-id="b3474-153">Note that the `-Body` parameter to the command maps to the `body` property on `chatMessage`.</span></span> <span data-ttu-id="b3474-154">Другие свойства сослаться аналогичным образом, поэтому вы можете изменить сообщение, которое вы отправляете.</span><span class="sxs-lookup"><span data-stu-id="b3474-154">Other properties are mapped in a similar way, so you can change the message you send.</span></span> <span data-ttu-id="b3474-155">Например, чтобы отправить экстренное сообщение, используйте следующую команду.</span><span class="sxs-lookup"><span data-stu-id="b3474-155">For example, to send an urgent message use the following command.</span></span>

```powershell
New-MgTeamChannelMessage -TeamId $team.Id -ChannelId $channel.Id -Body @{ Content="Hello World" } -Importance "urgent"
```

### <a name="sign-out"></a><span data-ttu-id="b3474-156">Выход</span><span class="sxs-lookup"><span data-stu-id="b3474-156">Sign out</span></span>

<span data-ttu-id="b3474-157">Используйте `Disconnect-MgGraph` команду, чтобы выйти из нее.</span><span class="sxs-lookup"><span data-stu-id="b3474-157">Use the `Disconnect-MgGraph` command to sign out.</span></span>

```powershell
Disconnect-MgGraph
```

## <a name="next-steps"></a><span data-ttu-id="b3474-158">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="b3474-158">Next steps</span></span>

- [<span data-ttu-id="b3474-159">Узнайте, как перемещаться по SDK</span><span class="sxs-lookup"><span data-stu-id="b3474-159">Learn how to navigate the SDK</span></span>](navigating.md)
- [<span data-ttu-id="b3474-160">Использование проверки подлинности только для приложений с помощью Microsoft Graph PowerShell SDK</span><span class="sxs-lookup"><span data-stu-id="b3474-160">Use app-only authentication with the Microsoft Graph PowerShell SDK</span></span>](app-only.md)
