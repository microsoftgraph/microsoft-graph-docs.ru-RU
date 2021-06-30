---
title: Отправка уведомлений о канале активности пользователям в Microsoft Teams
description: Отправка уведомлений о канале активности пользователям в Microsoft Teams с помощью Teams приложения и microsoft graph.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 5923b706321c9180fba8833aab029bf2396ecaff
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210201"
---
# <a name="send-activity-feed-notifications-to-users-in-microsoft-teams"></a><span data-ttu-id="8486f-103">Отправка уведомлений о канале активности пользователям в Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="8486f-103">Send activity feed notifications to users in Microsoft Teams</span></span>

<span data-ttu-id="8486f-104">Канал Microsoft Teams позволяет пользователям делить элементы, которые требуют внимания, уведомляя их об изменениях.</span><span class="sxs-lookup"><span data-stu-id="8486f-104">The Microsoft Teams activity feed enables users to triage items that require attention by notifying them of changes.</span></span> <span data-ttu-id="8486f-105">Вы можете использовать API уведомлений о каналах действий в Microsoft Graph, чтобы распространить эту функцию на приложения.</span><span class="sxs-lookup"><span data-stu-id="8486f-105">You can use the activity feed notification APIs in Microsoft Graph to extend this functionality to your apps.</span></span> <span data-ttu-id="8486f-106">Это позволяет приложениям предоставлять более богатые впечатления и лучше привлекать пользователей, помогая поддерживать их в курсе изменений в инструментах и рабочего процессах, которые они используют.</span><span class="sxs-lookup"><span data-stu-id="8486f-106">This allows your apps to provide richer experiences and better engage users by helping to keep them up to date with changes in the tools and workflows they use.</span></span>

## <a name="understanding-the-basics-of-activity-feed-notification"></a><span data-ttu-id="8486f-107">Понимание основ уведомления о канале активности</span><span class="sxs-lookup"><span data-stu-id="8486f-107">Understanding the basics of activity feed notification</span></span>

<span data-ttu-id="8486f-108">Уведомления каналов активности в Microsoft Teams состоят из нескольких битов информации, отображаемой вместе, как показано на следующем изображении.</span><span class="sxs-lookup"><span data-stu-id="8486f-108">Activity feed notifications in Microsoft Teams are comprised of multiple bits of information, displayed together, as shown in the following image.</span></span>

![Изображение, показывающая компоненты уведомления о канале действий](images/teams-activityfeednotifications/notificationtemplate.png)

<span data-ttu-id="8486f-110">Компоненты включают в себя:</span><span class="sxs-lookup"><span data-stu-id="8486f-110">The components include:</span></span>
- <span data-ttu-id="8486f-111">Актер, который инициировал действие</span><span class="sxs-lookup"><span data-stu-id="8486f-111">The actor who initiated the activity</span></span>
- <span data-ttu-id="8486f-112">Значок, который представляет тип действия</span><span class="sxs-lookup"><span data-stu-id="8486f-112">An icon that represents the activity type</span></span>
- <span data-ttu-id="8486f-113">Причина, по которой актер сделал действие</span><span class="sxs-lookup"><span data-stu-id="8486f-113">The reason the actor did the activity</span></span>
- <span data-ttu-id="8486f-114">Предварительный просмотр текста</span><span class="sxs-lookup"><span data-stu-id="8486f-114">A text preview</span></span>
- <span data-ttu-id="8486f-115">Отметка времени</span><span class="sxs-lookup"><span data-stu-id="8486f-115">A time stamp</span></span>
- <span data-ttu-id="8486f-116">Расположение действия</span><span class="sxs-lookup"><span data-stu-id="8486f-116">The location of the activity</span></span>

<span data-ttu-id="8486f-117">В следующем примере показано, как эти компоненты вместе предоставляют сведения об уведомлении.</span><span class="sxs-lookup"><span data-stu-id="8486f-117">The following example shows how these components together provide the details about a notification.</span></span> <span data-ttu-id="8486f-118">Этот пример — уведомление о пользователе, упомянутом в Yammer сообществе.</span><span class="sxs-lookup"><span data-stu-id="8486f-118">This example is a notification about a user mentioned in a Yammer community.</span></span>

![Yammer уведомлений об актификальности](images/teams-activityfeednotifications/examplefeednotification.png)

## <a name="requirements-for-using-the-activity-feed-notification-apis"></a><span data-ttu-id="8486f-120">Требования к использованию API уведомлений о подаче уведомлений о действиях</span><span class="sxs-lookup"><span data-stu-id="8486f-120">Requirements for using the activity feed notification APIs</span></span>

<span data-ttu-id="8486f-121">API каналов активности работают с [приложением Teams.](/microsoftteams/platform/overview)</span><span class="sxs-lookup"><span data-stu-id="8486f-121">Activity feed APIs work with a [Teams app](/microsoftteams/platform/overview).</span></span> <span data-ttu-id="8486f-122">Ниже приводится требование к отправке уведомлений о ленте действий:</span><span class="sxs-lookup"><span data-stu-id="8486f-122">The following are the requirements for sending activity feed notifications:</span></span>

- <span data-ttu-id="8486f-123">В манифесте Teams приложения должен быть добавлен ID приложения Azure AD в `webApplicationInfo` разделе.</span><span class="sxs-lookup"><span data-stu-id="8486f-123">The Teams app manifest must have the Azure AD app ID added to the `webApplicationInfo` section.</span></span> <span data-ttu-id="8486f-124">Подробные сведения см. в [схеме манифеста.](/microsoftteams/platform/resources/schema/manifest-schema)</span><span class="sxs-lookup"><span data-stu-id="8486f-124">For details, see [manifest schema](/microsoftteams/platform/resources/schema/manifest-schema).</span></span>
- <span data-ttu-id="8486f-125">Типы действий должны быть объявлены в `activities` разделе.</span><span class="sxs-lookup"><span data-stu-id="8486f-125">Activity types must be declared in the `activities` section.</span></span> <span data-ttu-id="8486f-126">Подробные сведения см. в [схеме манифеста.](/microsoftteams/platform/resources/schema/manifest-schema)</span><span class="sxs-lookup"><span data-stu-id="8486f-126">For details, see [manifest schema](/microsoftteams/platform/resources/schema/manifest-schema).</span></span>
- <span data-ttu-id="8486f-127">Приложение Teams должно быть установлено для получателя лично, [](/graph/api/resources/team?preserve-view=true) или в группе или чате, [в](/graph/api/resources/chat?preserve-view=true) который они входит.</span><span class="sxs-lookup"><span data-stu-id="8486f-127">The Teams app must be installed for the recipient, either personally, or in a [team](/graph/api/resources/team?preserve-view=true) or [chat](/graph/api/resources/chat?preserve-view=true) they are part of.</span></span> <span data-ttu-id="8486f-128">Дополнительные сведения см. [в Teams установки приложения.](/graph/api/resources/teamsappinstallation?preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="8486f-128">For more information, see [Teams app installation](/graph/api/resources/teamsappinstallation?preserve-view=true).</span></span>

### <a name="teams-app-manifest-changes"></a><span data-ttu-id="8486f-129">Teams изменения манифеста приложения</span><span class="sxs-lookup"><span data-stu-id="8486f-129">Teams app manifest changes</span></span>

<span data-ttu-id="8486f-130">В этом разделе описываются изменения, которые необходимо добавить в манифест Teams приложения.</span><span class="sxs-lookup"><span data-stu-id="8486f-130">This section describes the changes that need to be added to Teams app manifest.</span></span> <span data-ttu-id="8486f-131">Обратите внимание, что необходимо использовать версию манифеста [Teams или](/microsoftteams/platform/resources/schema/manifest-schema) `1.7` больше.</span><span class="sxs-lookup"><span data-stu-id="8486f-131">Note that you must be using the [Teams app manifest](/microsoftteams/platform/resources/schema/manifest-schema) version `1.7` or greater.</span></span>

```json
"$schema": "https://developer.microsoft.com/json-schemas/teams/v1.7/MicrosoftTeams.schema.json",
"manifestVersion": "1.7",
````

#### <a name="webapplicationinfo-section-changes"></a><span data-ttu-id="8486f-132">Изменения раздела webApplicationInfo</span><span class="sxs-lookup"><span data-stu-id="8486f-132">webApplicationInfo section changes</span></span>

```json
"webApplicationInfo":
{
    "id": "a3111f15-658e-457c-9689-fd20fe907330",
    "resource": "https://contosoapp.com"
}
```

|<span data-ttu-id="8486f-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="8486f-133">Parameter</span></span>|<span data-ttu-id="8486f-134">Тип</span><span class="sxs-lookup"><span data-stu-id="8486f-134">Type</span></span>|<span data-ttu-id="8486f-135">Описание</span><span class="sxs-lookup"><span data-stu-id="8486f-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8486f-136">id</span><span class="sxs-lookup"><span data-stu-id="8486f-136">id</span></span>|<span data-ttu-id="8486f-137">строка</span><span class="sxs-lookup"><span data-stu-id="8486f-137">string</span></span>|<span data-ttu-id="8486f-138">ID приложения Azure AD (client ID).</span><span class="sxs-lookup"><span data-stu-id="8486f-138">Azure AD app ID (client ID).</span></span>|
|<span data-ttu-id="8486f-139">resource</span><span class="sxs-lookup"><span data-stu-id="8486f-139">resource</span></span>|<span data-ttu-id="8486f-140">строка</span><span class="sxs-lookup"><span data-stu-id="8486f-140">string</span></span>|<span data-ttu-id="8486f-141">Ресурс, связанный с приложением Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8486f-141">Resource associated with the Azure AD app.</span></span> <span data-ttu-id="8486f-142">Также известен как URL-адрес ответа или перенаправления на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="8486f-142">Also known as reply or redirect URL in the Azure Portal.</span></span>|

> <span data-ttu-id="8486f-143">**Примечание:** Вы можете получить ошибку, если Teams приложений в одной области (команда, чат или пользователь) используют одно и то же приложение Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8486f-143">**Note:** You might get an error if multiple Teams apps in the same scope (team, chat or user) are using the same Azure AD app.</span></span> <span data-ttu-id="8486f-144">Убедитесь, что вы используете уникальные приложения Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8486f-144">Make sure that you're using unique Azure AD apps.</span></span>

#### <a name="activities-section-changes"></a><span data-ttu-id="8486f-145">Изменения раздела действий</span><span class="sxs-lookup"><span data-stu-id="8486f-145">activities section changes</span></span>

```json
"activities":
{
  "activityTypes": [
    {
      "type": "taskCreated",
      "description": "Task Created Activity",
      "templateText": "{actor} created task {taskId} for you"
    },
    {
      "type": "approvalRequired",
      "description": "Deployment requires your approval",
      "templateText": "{actor} created a new deployment {deploymentId}"
    }
  ]
}
```

|<span data-ttu-id="8486f-146">Параметр</span><span class="sxs-lookup"><span data-stu-id="8486f-146">Parameter</span></span>|<span data-ttu-id="8486f-147">Тип</span><span class="sxs-lookup"><span data-stu-id="8486f-147">Type</span></span>|<span data-ttu-id="8486f-148">Описание</span><span class="sxs-lookup"><span data-stu-id="8486f-148">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8486f-149">type</span><span class="sxs-lookup"><span data-stu-id="8486f-149">type</span></span>|<span data-ttu-id="8486f-150">string</span><span class="sxs-lookup"><span data-stu-id="8486f-150">string</span></span>|<span data-ttu-id="8486f-151">Тип действия.</span><span class="sxs-lookup"><span data-stu-id="8486f-151">Type of activity.</span></span> <span data-ttu-id="8486f-152">Это должно быть уникальным в определенном манифесте.</span><span class="sxs-lookup"><span data-stu-id="8486f-152">This needs to be unique in a specific manifest.</span></span>|
|<span data-ttu-id="8486f-153">description</span><span class="sxs-lookup"><span data-stu-id="8486f-153">description</span></span>|<span data-ttu-id="8486f-154">строка</span><span class="sxs-lookup"><span data-stu-id="8486f-154">string</span></span>|<span data-ttu-id="8486f-155">Краткое описание, считываемым человеком.</span><span class="sxs-lookup"><span data-stu-id="8486f-155">Human-readable short description.</span></span> <span data-ttu-id="8486f-156">Это будет видно на Microsoft Teams клиенте.</span><span class="sxs-lookup"><span data-stu-id="8486f-156">This will be visible on the Microsoft Teams client.</span></span>|
|<span data-ttu-id="8486f-157">templateText</span><span class="sxs-lookup"><span data-stu-id="8486f-157">templateText</span></span>|<span data-ttu-id="8486f-158">строка</span><span class="sxs-lookup"><span data-stu-id="8486f-158">string</span></span>|<span data-ttu-id="8486f-159">Текст шаблона для уведомления о действии.</span><span class="sxs-lookup"><span data-stu-id="8486f-159">Template text for the activity notification.</span></span> <span data-ttu-id="8486f-160">Вы можете объявить параметры, инкапсулируя параметры `{}` в .</span><span class="sxs-lookup"><span data-stu-id="8486f-160">You can declare your parameters by encapsulating parameters in `{}`.</span></span>|

><span data-ttu-id="8486f-161">**Примечание:** `actor` это специальный параметр, который всегда принимает имя вызываемого.</span><span class="sxs-lookup"><span data-stu-id="8486f-161">**Note:** `actor` is a special parameter that always takes the name of the caller.</span></span> <span data-ttu-id="8486f-162">В делегировании звонков имя `actor` пользователя.</span><span class="sxs-lookup"><span data-stu-id="8486f-162">In delegated calls, `actor` is the user's name.</span></span> <span data-ttu-id="8486f-163">В вызовах только для приложений оно принимает имя Teams приложения.</span><span class="sxs-lookup"><span data-stu-id="8486f-163">In application-only calls, it takes the name of the Teams app.</span></span>

### <a name="installing-the-teams-app"></a><span data-ttu-id="8486f-164">Установка приложения Teams</span><span class="sxs-lookup"><span data-stu-id="8486f-164">Installing the Teams app</span></span>

<span data-ttu-id="8486f-165">Teams приложения могут быть установлены в команде, чате или лично для пользователя и могут распространяться несколькими способами.</span><span class="sxs-lookup"><span data-stu-id="8486f-165">Teams apps can be installed in a team, a chat, or for a user personally, and can be distributed in multiple ways.</span></span> <span data-ttu-id="8486f-166">Подробные сведения см. [в Teams методах распространения приложений.](/microsoftteams/platform/concepts/deploy-and-publish/overview)</span><span class="sxs-lookup"><span data-stu-id="8486f-166">For details, see [Teams app distribution methods](/microsoftteams/platform/concepts/deploy-and-publish/overview).</span></span> <span data-ttu-id="8486f-167">Как правило, [для целей](/microsoftteams/platform/concepts/deploy-and-publish/apps-upload) разработки предпочтительна побочная загрузка.</span><span class="sxs-lookup"><span data-stu-id="8486f-167">Typically, [sideloading](/microsoftteams/platform/concepts/deploy-and-publish/apps-upload) is preferred for development purposes.</span></span> <span data-ttu-id="8486f-168">После разработки вы можете выбрать правильный метод распространения в зависимости от того, хотите ли вы распространять среди одного клиента или всех клиентов.</span><span class="sxs-lookup"><span data-stu-id="8486f-168">After development, you can choose the right distribution method based on whether you want to distribute to one tenant or to all tenants.</span></span>

<span data-ttu-id="8486f-169">Вы также можете [использовать Teams API](/graph/api/resources/teamsappinstallation?preserve-view=true) установки приложений для управления Teams установок приложений.</span><span class="sxs-lookup"><span data-stu-id="8486f-169">You can also use [Teams app installation](/graph/api/resources/teamsappinstallation?preserve-view=true) APIs to manage Teams app installations.</span></span>

## <a name="sending-activity-feed-notifications-to-users"></a><span data-ttu-id="8486f-170">Отправка уведомлений о канале активности пользователям</span><span class="sxs-lookup"><span data-stu-id="8486f-170">Sending activity feed notifications to users</span></span>

<span data-ttu-id="8486f-171">Так как Teams приложение можно установить для пользователя, в команде или в чате, уведомления можно отправить и в этих трех контекстах:</span><span class="sxs-lookup"><span data-stu-id="8486f-171">Because a Teams app can be installed for a user, in a team, or in a chat, the notifications can be sent in these three contexts as well:</span></span>

- [<span data-ttu-id="8486f-172">Отправка уведомления пользователю в чате</span><span class="sxs-lookup"><span data-stu-id="8486f-172">Send notification to user in a chat</span></span>](/graph/api/chat-sendactivitynotification)
- [<span data-ttu-id="8486f-173">Отправка уведомления пользователю в команде</span><span class="sxs-lookup"><span data-stu-id="8486f-173">Send notification to user in a team</span></span>](/graph/api/team-sendactivitynotification)
- [<span data-ttu-id="8486f-174">Отправка уведомления пользователю</span><span class="sxs-lookup"><span data-stu-id="8486f-174">Send notification to user</span></span>](/graph/api/userteamwork-sendactivitynotification)

<span data-ttu-id="8486f-175">Сведения о том, какие темы поддерживаются для каждого сценария, см. в конкретных API.</span><span class="sxs-lookup"><span data-stu-id="8486f-175">For details about what topics are supported for each scenario, see the specific APIs.</span></span> <span data-ttu-id="8486f-176">Настраиваемые текстовые темы поддерживаются для всех сценариев.</span><span class="sxs-lookup"><span data-stu-id="8486f-176">Custom text-based topics are supported for all scenarios.</span></span>

### <a name="example-1-notify-a-user-about-a-task-created-in-a-chat"></a><span data-ttu-id="8486f-177">Пример 1. Уведомление пользователя о задаче, созданной в чате</span><span class="sxs-lookup"><span data-stu-id="8486f-177">Example 1: Notify a user about a task created in a chat</span></span>

<span data-ttu-id="8486f-178">В этом примере показано, как можно отправить уведомление о ленте действий для новой задачи, созданной в чате.</span><span class="sxs-lookup"><span data-stu-id="8486f-178">This example shows how you can send an activity feed notification for a new task created in a chat.</span></span> <span data-ttu-id="8486f-179">В этом случае Teams приложение должно быть установлено в чате с ИД, а пользователь также должен быть частью `chatId` `569363e2-4e49-4661-87f2-16f245c5d66a` чата.</span><span class="sxs-lookup"><span data-stu-id="8486f-179">In this case, the Teams app must be installed in a chat with Id `chatId` and user `569363e2-4e49-4661-87f2-16f245c5d66a` must be part of the chat as well.</span></span>

#### <a name="request"></a><span data-ttu-id="8486f-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="8486f-180">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "chat_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/beta/chats/{chatId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/beta/chats/{chatId}"
    },
    "activityType": "taskCreated",
    "previewText": {
        "content": "New Task Created"
    },
    "recipient": {
        "@odata.type": "microsoft.graph.aadUserNotificationRecipient",
        "userId": "569363e2-4e49-4661-87f2-16f245c5d66a"
    },
    "templateParameters": [
        {
            "name": "taskId",
            "value": "12322"
        }
    ]
}
```

#### <a name="response"></a><span data-ttu-id="8486f-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="8486f-181">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-notify-a-user-about-a-task-created-in-a-team"></a><span data-ttu-id="8486f-182">Пример 2. Уведомление пользователя о задаче, созданной в команде</span><span class="sxs-lookup"><span data-stu-id="8486f-182">Example 2: Notify a user about a task created in a team</span></span>

<span data-ttu-id="8486f-183">В этом примере показано, как можно отправить уведомление о канале действий для группы.</span><span class="sxs-lookup"><span data-stu-id="8486f-183">This example shows how you can send an activity feed notification for a team.</span></span> <span data-ttu-id="8486f-184">В этом примере владелец группы сообщает о новой задаче, которая требует их внимания.</span><span class="sxs-lookup"><span data-stu-id="8486f-184">This example notifies the team owner about a new task created that requires their attention.</span></span>

#### <a name="request"></a><span data-ttu-id="8486f-185">Запрос</span><span class="sxs-lookup"><span data-stu-id="8486f-185">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/{teamId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/beta/teams/{teamId}"
    },
    "activityType": "taskCreated",
    "previewText": {
        "content": "New Task Created"
    },
    "recipient": {
        "@odata.type": "microsoft.graph.aadUserNotificationRecipient",
        "userId": "569363e2-4e49-4661-87f2-16f245c5d66a"
    },
    "templateParameters": [
        {
            "name": "taskId",
            "value": "12322"
        }
    ]
}
```

#### <a name="response"></a><span data-ttu-id="8486f-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="8486f-186">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-3-notify-a-user-about-an-event-using-a-custom-topic"></a><span data-ttu-id="8486f-187">Пример 3. Уведомление пользователя о событии с использованием настраиваемой темы</span><span class="sxs-lookup"><span data-stu-id="8486f-187">Example 3: Notify a user about an event using a custom topic</span></span>

<span data-ttu-id="8486f-188">Как повествуют в предыдущих примерах, вы можете ссылаться на различные аспекты группы или чата.</span><span class="sxs-lookup"><span data-stu-id="8486f-188">As seen in the previous examples, you can link to different aspects of a team or a chat.</span></span> <span data-ttu-id="8486f-189">Однако, если вы хотите связаться с аспектом, который не входит в команду или не представлен Microsoft Graph, или если вы хотите настроить имя, вы можете установить источник и передать в настраиваемом значении для `topic` `text` него.</span><span class="sxs-lookup"><span data-stu-id="8486f-189">However, if you want to link to an aspect that is not part of the team or is not represented by Microsoft Graph, or if you want to customize the name, you can set the source of the `topic` to `text` and pass in a custom value for it.</span></span> <span data-ttu-id="8486f-190">Кроме того, `webUrl` требуется, когда вы используете `topic` источник в качестве `text` .</span><span class="sxs-lookup"><span data-stu-id="8486f-190">Additionally, `webUrl` is required when you use `topic` source as `text`.</span></span>

<span data-ttu-id="8486f-191">В Yammer, показанного ранее, используется настраиваемая тема, так как Yammer ресурсы Майкрософт не поддерживаются Graph.</span><span class="sxs-lookup"><span data-stu-id="8486f-191">The Yammer notification example shown earlier uses a custom topic because Yammer's resources are not supported by Microsoft Graph.</span></span>

> <span data-ttu-id="8486f-192">**Примечание:** `webUrl` должен начинаться с Microsoft Teams домена (например teams.microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="8486f-192">**Note:** `webUrl` must start with the Microsoft Teams domain (teams.microsoft.com for example).</span></span>

#### <a name="request"></a><span data-ttu-id="8486f-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="8486f-193">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/{teamId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "text",
        "value": "Deployment Approvals Channel",
        "webUrl": "https://teams.microsoft.com/l/message/19:448cfd2ac2a7490a9084a9ed14cttr78c@thread.skype/1605223780000?tenantId=c8b1bf45-3834-4ecf-971a-b4c755ee677d&groupId=d4c2a937-f097-435a-bc91-5c1683ca7245&parentMessageId=1605223771864&teamName=Approvals&channelName=Azure%20DevOps&createdTime=1605223780000"
    },
    "activityType": "approvalRequired",
    "previewText": {
        "content": "New deployment requires your approval"
    },
    "recipient": {
        "@odata.type": "Microsoft.Teams.GraphSvc.aadUserNotificationRecipient",
        "userId": "569363e2-4e49-4661-87f2-16f245c5d66a"
    },
    "templateParameters": [
        {
            "name": "deploymentId",
            "value": "6788662"
        }
    ]
}
```

#### <a name="response"></a><span data-ttu-id="8486f-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="8486f-194">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-4-notify-the-team-members-about-an-event"></a><span data-ttu-id="8486f-195">Пример 4. Уведомление участников группы о событии</span><span class="sxs-lookup"><span data-stu-id="8486f-195">Example 4: Notify the team members about an event</span></span>

<span data-ttu-id="8486f-196">В этом примере показано, как можно отправить уведомление о канале действий всем участникам группы.</span><span class="sxs-lookup"><span data-stu-id="8486f-196">This example shows how you can send an activity feed notification to all team members.</span></span> <span data-ttu-id="8486f-197">В этом примере участники группы будут изве-за нового события.</span><span class="sxs-lookup"><span data-stu-id="8486f-197">This example notifies the team members about a new event.</span></span> 

> <span data-ttu-id="8486f-198">**Примечание:** Возможность отправки уведомлений всем участникам группы в настоящее время доступна только в бета-версии.</span><span class="sxs-lookup"><span data-stu-id="8486f-198">**Note:** The ability to send notifications to all team members is currently only available in beta.</span></span>

#### <a name="request"></a><span data-ttu-id="8486f-199">Запрос</span><span class="sxs-lookup"><span data-stu-id="8486f-199">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/7155e3c8-175e-4311-97ef-572edc3aa3db/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "text",
        "value": "Weekly Virtual Social",
        "webUrl": "Teams webUrl"
    },
    "previewText": {
        "content": "It will be fun!"
    },
    "activityType": "eventCreated",
    "recipient": {
        "@odata.type": "microsoft.graph.teamMembersNotificationRecipient",
        "teamId": "7155e3c8-175e-4311-97ef-572edc3aa3db"
    }
}
```

#### <a name="response"></a><span data-ttu-id="8486f-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="8486f-200">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-5-notify-the-channel-members-about-an-event"></a><span data-ttu-id="8486f-201">Пример 5. Уведомление участников канала о событии</span><span class="sxs-lookup"><span data-stu-id="8486f-201">Example 5: Notify the channel members about an event</span></span>

<span data-ttu-id="8486f-202">В этом примере показано, как можно отправить уведомление о канале действий всем участникам канала.</span><span class="sxs-lookup"><span data-stu-id="8486f-202">This example shows how you can send an activity feed notification to all channel members.</span></span> <span data-ttu-id="8486f-203">В этом примере участникам канала сообщается о новом событии.</span><span class="sxs-lookup"><span data-stu-id="8486f-203">This example notifies the channel members about a new event.</span></span> 

> <span data-ttu-id="8486f-204">**Примечание:** Возможность отправки уведомлений всем участникам канала в настоящее время доступна только в бета-версии.</span><span class="sxs-lookup"><span data-stu-id="8486f-204">**Note:** The ability to send notifications to all channel members is currently only available in beta.</span></span>

#### <a name="request"></a><span data-ttu-id="8486f-205">Запрос</span><span class="sxs-lookup"><span data-stu-id="8486f-205">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/7155e3c8-175e-4311-97ef-572edc3aa3db/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "text",
        "value": "Weekly Virtual Social",
        "webUrl": "Teams webUrl"
    },
    "previewText": {
        "content": "It will be fun!"
    },
    "activityType": "eventCreated",
    "recipient": {
        "@odata.type": "microsoft.graph.channelMembersNotificationRecipient",
        "teamId": "7155e3c8-175e-4311-97ef-572edc3aa3db",
        "channelId": "19:0ea5de04de4743bcb4cd20cb99235d99@thread.tacv2"
    }
}
```

#### <a name="response"></a><span data-ttu-id="8486f-206">Отклик</span><span class="sxs-lookup"><span data-stu-id="8486f-206">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-6-notify-the-chat-members-about-an-event"></a><span data-ttu-id="8486f-207">Пример 6. Уведомление участников чата о событии</span><span class="sxs-lookup"><span data-stu-id="8486f-207">Example 6: Notify the chat members about an event</span></span>

<span data-ttu-id="8486f-208">В этом примере показано, как можно отправить уведомление о канале действий всем участникам чата.</span><span class="sxs-lookup"><span data-stu-id="8486f-208">This example shows how you can send an activity feed notification to all chat members.</span></span> <span data-ttu-id="8486f-209">В этом примере участники чата извечат о новом событии.</span><span class="sxs-lookup"><span data-stu-id="8486f-209">This example notifies the chat members about a new event.</span></span> 

> <span data-ttu-id="8486f-210">**Примечание:** Возможность отправлять уведомления всем участникам чата в настоящее время доступна только в бета-версии.</span><span class="sxs-lookup"><span data-stu-id="8486f-210">**Note:** The ability to send notifications to all chat members is currently only available in beta.</span></span>

#### <a name="request"></a><span data-ttu-id="8486f-211">Запрос</span><span class="sxs-lookup"><span data-stu-id="8486f-211">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "chat_sendactivitynotification"
}
-->

``` http
POST https://graph.microsoft.com/beta/chats/19:d65713bc498c4a428c71ef9353e6ce20@thread.v2/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "text",
        "value": "Weekly Virtual Social",
        "webUrl": "Teams webUrl"
    },
    "previewText": {
        "content": "It will be fun!"
    },
    "activityType": "eventCreated",
    "recipient": {
        "@odata.type": "microsoft.graph.chatMembersNotificationRecipient",
        "chatId": "19:d65713bc498c4a428c71ef9353e6ce20@thread.v2"
    }
}
```

#### <a name="response"></a><span data-ttu-id="8486f-212">Отклик</span><span class="sxs-lookup"><span data-stu-id="8486f-212">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

## <a name="customizing-how-the-notifications-alert-you"></a><span data-ttu-id="8486f-213">Настройка оповещения уведомлений</span><span class="sxs-lookup"><span data-stu-id="8486f-213">Customizing how the notifications alert you</span></span>

<span data-ttu-id="8486f-214">Microsoft Teams пользователи могут настраивать уведомления, которые они видят в своем канале, в качестве баннера и так далее.</span><span class="sxs-lookup"><span data-stu-id="8486f-214">Microsoft Teams users can customize the notifications they see in their feed, as a banner, and so on.</span></span> <span data-ttu-id="8486f-215">Также можно настроить уведомления, созданные с помощью API-каналов активности.</span><span class="sxs-lookup"><span data-stu-id="8486f-215">Notifications generated through activity feed APIs can also be customized.</span></span> <span data-ttu-id="8486f-216">Пользователи могут выбрать, как они уведомлены с помощью параметров в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="8486f-216">Users can choose how they are notified via settings in Microsoft Teams.</span></span> <span data-ttu-id="8486f-217">Teams приложения будут отображаться в списке для выбора пользователя, как показано на следующем скриншоте.</span><span class="sxs-lookup"><span data-stu-id="8486f-217">Teams apps will appear in the list for the user to choose from, as shown in the following screenshot.</span></span>

![Снимок экрана параметров уведомлений в Teams с выделенной опцией Custom](images/teams-activityfeednotifications/notificationsettings.png)

<span data-ttu-id="8486f-219">Пользователи могут нажать **кнопку Изменить** рядом с приложением и настроить уведомления, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="8486f-219">Users can click **Edit** next to an app and customize the notifications, as shown in the following example.</span></span> <span data-ttu-id="8486f-220">Отображается `description` поле в манифесте Teams приложения.</span><span class="sxs-lookup"><span data-stu-id="8486f-220">The `description` field in the Teams app manifest is displayed.</span></span>

![Снимок экрана, показывающий уведомления, настроенные на Баннер и канал для Teams приложения](images/teams-activityfeednotifications/applevelnotificationsettings.png)

## <a name="faqs"></a><span data-ttu-id="8486f-222">Вопросы и ответы</span><span class="sxs-lookup"><span data-stu-id="8486f-222">FAQs</span></span>

### <a name="who-needs-to-install-the-teams-app"></a><span data-ttu-id="8486f-223">Кто необходимо установить приложение Teams?</span><span class="sxs-lookup"><span data-stu-id="8486f-223">Who needs to install the Teams app?</span></span>

<span data-ttu-id="8486f-224">Целевой пользователь должен иметь Teams, которое отправляет уведомления.</span><span class="sxs-lookup"><span data-stu-id="8486f-224">The target user must have the Teams app that is sending notifications installed.</span></span>

### <a name="can-a-user-send-notifications-to-themselves"></a><span data-ttu-id="8486f-225">Может ли пользователь отправлять уведомления самим себе?</span><span class="sxs-lookup"><span data-stu-id="8486f-225">Can a user send notifications to themselves?</span></span>

<span data-ttu-id="8486f-226">Нет, пользователь не может отправлять уведомления себе.</span><span class="sxs-lookup"><span data-stu-id="8486f-226">No, a user cannot send notifications to themselves.</span></span> <span data-ttu-id="8486f-227">Для этого сценария используйте разрешения приложений.</span><span class="sxs-lookup"><span data-stu-id="8486f-227">For this scenario, use application permissions.</span></span>

### <a name="can-a-teams-app-control-how-the-notifications-are-shown-to-the-user"></a><span data-ttu-id="8486f-228">Может ли Teams управлять тем, как показываются уведомления пользователю?</span><span class="sxs-lookup"><span data-stu-id="8486f-228">Can a Teams app control how the notifications are shown to the user?</span></span>

<span data-ttu-id="8486f-229">Нет, только пользователям разрешено изменять параметры уведомлений.</span><span class="sxs-lookup"><span data-stu-id="8486f-229">No, only users are allowed to change notification settings.</span></span>

### <a name="i-installed-my-app-why-dont-i-see-notification-settings-under-the-user-account"></a><span data-ttu-id="8486f-230">Я установила приложение, почему я не вижу параметры уведомлений в учетной записи пользователя?</span><span class="sxs-lookup"><span data-stu-id="8486f-230">I installed my app, why don't I see notification settings under the user account?</span></span>

<span data-ttu-id="8486f-231">Параметры будут отображаться после того, как первое уведомление будет отправлено Teams приложением.</span><span class="sxs-lookup"><span data-stu-id="8486f-231">The settings will appear after the first notification is sent by the Teams app.</span></span> <span data-ttu-id="8486f-232">Это уменьшает количество параметров, которые видят пользователи.</span><span class="sxs-lookup"><span data-stu-id="8486f-232">This reduces the number of settings that users see.</span></span>

### <a name="i-started-getting-a-409-conflict-error-how-do-i-resolve-it"></a><span data-ttu-id="8486f-233">Я начал получать ошибку 409 (конфликт), как ее разрешить?</span><span class="sxs-lookup"><span data-stu-id="8486f-233">I started getting a 409 (conflict) error, how do I resolve it?</span></span>

<span data-ttu-id="8486f-234">`Conflict`Ошибки в основном возникают, когда несколько Teams приложений, установленных в одной области (команда, чат, пользователь и так далее), имеют один и тот же appId Azure AD в разделе `webApplicationInfo` манифеста.</span><span class="sxs-lookup"><span data-stu-id="8486f-234">`Conflict` errors primarily occur when multiple Teams apps installed in the same scope (team, chat, user, and so on) have the same Azure AD appId in the `webApplicationInfo` section of the manifest.</span></span> <span data-ttu-id="8486f-235">Когда это произойдет, вы получите ошибку, такую как `Found multiple applications with the same Azure AD App ID 'Your AzureAD AppId'.` .</span><span class="sxs-lookup"><span data-stu-id="8486f-235">When this happens, you will get an error such as `Found multiple applications with the same Azure AD App ID 'Your AzureAD AppId'.`.</span></span> <span data-ttu-id="8486f-236">Убедитесь, что вы используете уникальные приложения Azure AD для уникальных Teams приложений.</span><span class="sxs-lookup"><span data-stu-id="8486f-236">Make sure that you use unique Azure AD apps for unique Teams apps.</span></span> <span data-ttu-id="8486f-237">Обратите внимание, что вы можете установить одно Teams в нескольких сферах (например, team + user).</span><span class="sxs-lookup"><span data-stu-id="8486f-237">Note that you can have the same Teams app installed in multiple scopes (team + user for example).</span></span>

## <a name="see-also"></a><span data-ttu-id="8486f-238">См. также</span><span class="sxs-lookup"><span data-stu-id="8486f-238">See also</span></span>

<span data-ttu-id="8486f-239">[Лучшие практики для использования Microsoft Teams каналов активности.](activity-feed-notifications-best-practices.md)</span><span class="sxs-lookup"><span data-stu-id="8486f-239">[Best practices for using Microsoft Teams activity feed notifications](activity-feed-notifications-best-practices.md).</span></span>