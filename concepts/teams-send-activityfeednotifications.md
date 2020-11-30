---
title: Отправка уведомлений о каналах активности пользователям в Microsoft Teams
description: Отправлять уведомления о каналах активности пользователям в Microsoft Teams с помощью приложений Teams и Microsoft Graph.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 33a44ef158a1336e198e7382e144efed11ff35e7
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377455"
---
# <a name="send-activity-feed-notifications-to-users-in-microsoft-teams"></a><span data-ttu-id="c8836-103">Отправка уведомлений о каналах активности пользователям в Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="c8836-103">Send activity feed notifications to users in Microsoft Teams</span></span>

<span data-ttu-id="c8836-104">Канал активности Microsoft Teams позволяет пользователям рассматривать элементы, требующие внимания, уведомляя их об изменениях.</span><span class="sxs-lookup"><span data-stu-id="c8836-104">The Microsoft Teams activity feed enables users to triage items that require attention by notifying them of changes.</span></span> <span data-ttu-id="c8836-105">Вы можете использовать API уведомления о каналах активности в Microsoft Graph, чтобы расширить эту функциональность для ваших приложений.</span><span class="sxs-lookup"><span data-stu-id="c8836-105">You can use the activity feed notification APIs in Microsoft Graph to extend this functionality to your apps.</span></span> <span data-ttu-id="c8836-106">Это позволит вашим приложениям предоставлять более широкие возможности и лучше привлекать пользователей, помогая поддерживать их в соответствии с изменениями в средствах и рабочих процессах, которые они используют.</span><span class="sxs-lookup"><span data-stu-id="c8836-106">This allows your apps to provide richer experiences and better engage users by helping to keep them up to date with changes in the tools and workflows they use.</span></span>

## <a name="understanding-the-basics-of-activity-feed-notification"></a><span data-ttu-id="c8836-107">Основные сведения об уведомлении канала активности</span><span class="sxs-lookup"><span data-stu-id="c8836-107">Understanding the basics of activity feed notification</span></span>

<span data-ttu-id="c8836-108">Уведомления канала активности в Microsoft Teams состоят из нескольких битов данных, которые отображаются вместе, как показано на следующем рисунке.</span><span class="sxs-lookup"><span data-stu-id="c8836-108">Activity feed notifications in Microsoft Teams are comprised of multiple bits of information, displayed together, as shown in the following image.</span></span>

![Изображение, на котором показаны компоненты уведомления веб-канала активности](images/teams-activityfeednotifications/notificationtemplate.png)

<span data-ttu-id="c8836-110">К компонентам относятся:</span><span class="sxs-lookup"><span data-stu-id="c8836-110">The components include:</span></span>
- <span data-ttu-id="c8836-111">Субъект, который инициировал действие</span><span class="sxs-lookup"><span data-stu-id="c8836-111">The actor who initiated the activity</span></span>
- <span data-ttu-id="c8836-112">Значок, представляющий тип действия</span><span class="sxs-lookup"><span data-stu-id="c8836-112">An icon that represents the activity type</span></span>
- <span data-ttu-id="c8836-113">Причина, по которой субъект выполнил действие</span><span class="sxs-lookup"><span data-stu-id="c8836-113">The reason the actor did the activity</span></span>
- <span data-ttu-id="c8836-114">Предварительный просмотр текста</span><span class="sxs-lookup"><span data-stu-id="c8836-114">A text preview</span></span>
- <span data-ttu-id="c8836-115">Отметка времени</span><span class="sxs-lookup"><span data-stu-id="c8836-115">A time stamp</span></span>
- <span data-ttu-id="c8836-116">Расположение действия</span><span class="sxs-lookup"><span data-stu-id="c8836-116">The location of the activity</span></span>

<span data-ttu-id="c8836-117">В следующем примере показано, как эти компоненты совместно предоставляют сведения об уведомлении.</span><span class="sxs-lookup"><span data-stu-id="c8836-117">The following example shows how these components together provide the details about a notification.</span></span> <span data-ttu-id="c8836-118">В этом примере отображается уведомление о пользователе, упомянутом в сообществе Yammer.</span><span class="sxs-lookup"><span data-stu-id="c8836-118">This example is a notification about a user mentioned in a Yammer community.</span></span>

![Пример уведомления актифити Yammer](images/teams-activityfeednotifications/examplefeednotification.png)

## <a name="requirements-for-using-the-activity-feed-notification-apis"></a><span data-ttu-id="c8836-120">Требования для использования API уведомления канала активности</span><span class="sxs-lookup"><span data-stu-id="c8836-120">Requirements for using the activity feed notification APIs</span></span>

<span data-ttu-id="c8836-121">API веб-каналов активности работают с [приложением Teams](/microsoftteams/platform/overview).</span><span class="sxs-lookup"><span data-stu-id="c8836-121">Activity feed APIs work with a [Teams app](/microsoftteams/platform/overview).</span></span> <span data-ttu-id="c8836-122">Ниже приведены требования для отправки уведомлений о каналах активности:</span><span class="sxs-lookup"><span data-stu-id="c8836-122">The following are the requirements for sending activity feed notifications:</span></span>

- <span data-ttu-id="c8836-123">Манифест приложения Teams должен иметь идентификатор приложения Azure AD, добавленный в `webApplicationInfo` раздел.</span><span class="sxs-lookup"><span data-stu-id="c8836-123">The Teams app manifest must have the Azure AD app ID added to the `webApplicationInfo` section.</span></span> <span data-ttu-id="c8836-124">Дополнительные сведения см. в статье [схема манифеста](/microsoftteams/platform/resources/schema/manifest-schema).</span><span class="sxs-lookup"><span data-stu-id="c8836-124">For details, see [manifest schema](/microsoftteams/platform/resources/schema/manifest-schema).</span></span>
- <span data-ttu-id="c8836-125">Типы действий должны быть объявлены в `activities` разделе.</span><span class="sxs-lookup"><span data-stu-id="c8836-125">Activity types must be declared in the `activities` section.</span></span> <span data-ttu-id="c8836-126">Дополнительные сведения см. в статье [схема манифеста](/microsoftteams/platform/resources/schema/manifest-schema).</span><span class="sxs-lookup"><span data-stu-id="c8836-126">For details, see [manifest schema](/microsoftteams/platform/resources/schema/manifest-schema).</span></span>
- <span data-ttu-id="c8836-127">Приложение Teams должно быть установлено для получателя, либо для личного, либо для [группы](/graph/api/resources/team?preserve-view=true) или [чата](/graph/api/resources/chat?preserve-view=true) .</span><span class="sxs-lookup"><span data-stu-id="c8836-127">The Teams app must be installed for the recipient, either personally, or in a [team](/graph/api/resources/team?preserve-view=true) or [chat](/graph/api/resources/chat?preserve-view=true) they are part of.</span></span> <span data-ttu-id="c8836-128">Дополнительные [сведения см.](/graph/api/resources/teamsappinstallation?preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="c8836-128">For more information, see [Teams app installation](/graph/api/resources/teamsappinstallation?preserve-view=true).</span></span>

### <a name="teams-app-manifest-changes"></a><span data-ttu-id="c8836-129">Изменения в манифесте приложения Teams</span><span class="sxs-lookup"><span data-stu-id="c8836-129">Teams app manifest changes</span></span>

<span data-ttu-id="c8836-130">В этом разделе описываются изменения, которые необходимо добавить в манифест приложения Teams.</span><span class="sxs-lookup"><span data-stu-id="c8836-130">This section describes the changes that need to be added to Teams app manifest.</span></span> <span data-ttu-id="c8836-131">Обратите внимание, что необходимо использовать [манифест приложения Teams](/microsoftteams/platform/resources/schema/manifest-schema) `1.7` или более поздней версии.</span><span class="sxs-lookup"><span data-stu-id="c8836-131">Note that you must be using the [Teams app manifest](/microsoftteams/platform/resources/schema/manifest-schema) version `1.7` or greater.</span></span>

```json
"$schema": "https://developer.microsoft.com/json-schemas/teams/v1.7/MicrosoftTeams.schema.json",
"manifestVersion": "1.7",
````

#### <a name="webapplicationinfo-section-changes"></a><span data-ttu-id="c8836-132">изменения в разделе webApplicationInfo</span><span class="sxs-lookup"><span data-stu-id="c8836-132">webApplicationInfo section changes</span></span>

```json
"webApplicationInfo":
{
    "id": "a3111f15-658e-457c-9689-fd20fe907330",
    "resource": "https://contosoapp.com"
}
```

|<span data-ttu-id="c8836-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="c8836-133">Parameter</span></span>|<span data-ttu-id="c8836-134">Тип</span><span class="sxs-lookup"><span data-stu-id="c8836-134">Type</span></span>|<span data-ttu-id="c8836-135">Описание</span><span class="sxs-lookup"><span data-stu-id="c8836-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8836-136">id</span><span class="sxs-lookup"><span data-stu-id="c8836-136">id</span></span>|<span data-ttu-id="c8836-137">string</span><span class="sxs-lookup"><span data-stu-id="c8836-137">string</span></span>|<span data-ttu-id="c8836-138">Идентификатор приложения Azure AD (идентификатор клиента).</span><span class="sxs-lookup"><span data-stu-id="c8836-138">Azure AD app ID (client ID).</span></span>|
|<span data-ttu-id="c8836-139">resource</span><span class="sxs-lookup"><span data-stu-id="c8836-139">resource</span></span>|<span data-ttu-id="c8836-140">string</span><span class="sxs-lookup"><span data-stu-id="c8836-140">string</span></span>|<span data-ttu-id="c8836-141">Ресурс, связанный с приложением Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c8836-141">Resource associated with the Azure AD app.</span></span> <span data-ttu-id="c8836-142">Также называется URL-адресом ответа или перенаправлением на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="c8836-142">Also known as reply or redirect URL in the Azure Portal.</span></span>|

> <span data-ttu-id="c8836-143">**Примечание:** Вы можете получить сообщение об ошибке, если несколько приложений Teams в одной области (группа, чат или пользователь) используют одно и то же приложение Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c8836-143">**Note:** You might get an error if multiple Teams apps in the same scope (team, chat or user) are using the same Azure AD app.</span></span> <span data-ttu-id="c8836-144">Убедитесь, что вы используете уникальные приложения Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c8836-144">Make sure that you're using unique Azure AD apps.</span></span>

#### <a name="activities-section-changes"></a><span data-ttu-id="c8836-145">изменения в разделе "действия"</span><span class="sxs-lookup"><span data-stu-id="c8836-145">activities section changes</span></span>

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

|<span data-ttu-id="c8836-146">Параметр</span><span class="sxs-lookup"><span data-stu-id="c8836-146">Parameter</span></span>|<span data-ttu-id="c8836-147">Тип</span><span class="sxs-lookup"><span data-stu-id="c8836-147">Type</span></span>|<span data-ttu-id="c8836-148">Описание</span><span class="sxs-lookup"><span data-stu-id="c8836-148">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8836-149">type</span><span class="sxs-lookup"><span data-stu-id="c8836-149">type</span></span>|<span data-ttu-id="c8836-150">string</span><span class="sxs-lookup"><span data-stu-id="c8836-150">string</span></span>|<span data-ttu-id="c8836-151">Тип действия.</span><span class="sxs-lookup"><span data-stu-id="c8836-151">Type of activity.</span></span> <span data-ttu-id="c8836-152">Они должны быть уникальными в определенном манифесте.</span><span class="sxs-lookup"><span data-stu-id="c8836-152">This needs to be unique in a specific manifest.</span></span>|
|<span data-ttu-id="c8836-153">description</span><span class="sxs-lookup"><span data-stu-id="c8836-153">description</span></span>|<span data-ttu-id="c8836-154">string</span><span class="sxs-lookup"><span data-stu-id="c8836-154">string</span></span>|<span data-ttu-id="c8836-155">Понятное для человека краткое описание.</span><span class="sxs-lookup"><span data-stu-id="c8836-155">Human-readable short description.</span></span> <span data-ttu-id="c8836-156">Он будет отображаться в клиенте Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="c8836-156">This will be visible on the Microsoft Teams client.</span></span>|
|<span data-ttu-id="c8836-157">темплатетекст</span><span class="sxs-lookup"><span data-stu-id="c8836-157">templateText</span></span>|<span data-ttu-id="c8836-158">string</span><span class="sxs-lookup"><span data-stu-id="c8836-158">string</span></span>|<span data-ttu-id="c8836-159">Текст шаблона для уведомления о действии.</span><span class="sxs-lookup"><span data-stu-id="c8836-159">Template text for the activity notification.</span></span> <span data-ttu-id="c8836-160">Вы можете объявить параметры с помощью инкапсуляции параметров в `{}` .</span><span class="sxs-lookup"><span data-stu-id="c8836-160">You can declare your parameters by encapsulating parameters in `{}`.</span></span>|

><span data-ttu-id="c8836-161">**Примечание:** `actor` — Это особый параметр, который всегда принимает имя вызывающего абонента.</span><span class="sxs-lookup"><span data-stu-id="c8836-161">**Note:** `actor` is a special parameter that always takes the name of the caller.</span></span> <span data-ttu-id="c8836-162">В случае делегированных вызовов `actor` — это имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="c8836-162">In delegated calls, `actor` is the user's name.</span></span> <span data-ttu-id="c8836-163">В вызовах, использующих только приложения, он принимает имя приложения Teams.</span><span class="sxs-lookup"><span data-stu-id="c8836-163">In application-only calls, it takes the name of the Teams app.</span></span>

### <a name="installing-the-teams-app"></a><span data-ttu-id="c8836-164">Установка приложения Teams</span><span class="sxs-lookup"><span data-stu-id="c8836-164">Installing the Teams app</span></span>

<span data-ttu-id="c8836-165">Приложения Teams могут быть установлены в команде, в чате или для пользователя лично и могут распространяться несколькими способами.</span><span class="sxs-lookup"><span data-stu-id="c8836-165">Teams apps can be installed in a team, a chat, or for a user personally, and can be distributed in multiple ways.</span></span> <span data-ttu-id="c8836-166">Подробнее: [методы распространения приложений Teams](/microsoftteams/platform/concepts/deploy-and-publish/overview).</span><span class="sxs-lookup"><span data-stu-id="c8836-166">For details, see [Teams app distribution methods](/microsoftteams/platform/concepts/deploy-and-publish/overview).</span></span> <span data-ttu-id="c8836-167">Как правило, для целей разработки рекомендуется использовать загрузку [неопубликованных приложений](/microsoftteams/platform/concepts/deploy-and-publish/apps-upload) .</span><span class="sxs-lookup"><span data-stu-id="c8836-167">Typically, [sideloading](/microsoftteams/platform/concepts/deploy-and-publish/apps-upload) is preferred for development purposes.</span></span> <span data-ttu-id="c8836-168">После разработки можно выбрать правильный метод распространения в зависимости от того, хотите ли вы распределить их по одному клиенту или всем клиентам.</span><span class="sxs-lookup"><span data-stu-id="c8836-168">After development, you can choose the right distribution method based on whether you want to distribute to one tenant or to all tenants.</span></span>

<span data-ttu-id="c8836-169">Вы также можете использовать API [установки приложений Teams](/graph/api/resources/teamsappinstallation?preserve-view=true) для управления установками приложений Teams.</span><span class="sxs-lookup"><span data-stu-id="c8836-169">You can also use [Teams app installation](/graph/api/resources/teamsappinstallation?preserve-view=true) APIs to manage Teams app installations.</span></span>

## <a name="sending-activity-feed-notifications-to-users"></a><span data-ttu-id="c8836-170">Отправка уведомлений о каналах активности пользователям</span><span class="sxs-lookup"><span data-stu-id="c8836-170">Sending activity feed notifications to users</span></span>

<span data-ttu-id="c8836-171">Поскольку приложение Teams можно установить для пользователя, в команде или в чате, уведомления можно отправлять в этих трех контекстах:</span><span class="sxs-lookup"><span data-stu-id="c8836-171">Because a Teams app can be installed for a user, in a team, or in a chat, the notifications can be sent in these three contexts as well:</span></span>

- [<span data-ttu-id="c8836-172">Отправка уведомления пользователю в чате</span><span class="sxs-lookup"><span data-stu-id="c8836-172">Send notification to user in a chat</span></span>](/graph/api/chat-sendactivitynotification)
- [<span data-ttu-id="c8836-173">Отправка уведомления пользователю команды</span><span class="sxs-lookup"><span data-stu-id="c8836-173">Send notification to user in a team</span></span>](/graph/api/team-sendactivitynotification)
- [<span data-ttu-id="c8836-174">Отправка уведомления пользователю</span><span class="sxs-lookup"><span data-stu-id="c8836-174">Send notification to user</span></span>](/graph/api/userteamwork-sendactivitynotification)

<span data-ttu-id="c8836-175">Сведения о том, какие разделы поддерживаются для каждого сценария, можно найти в указанных API.</span><span class="sxs-lookup"><span data-stu-id="c8836-175">For details about what topics are supported for each scenario, see the specific APIs.</span></span> <span data-ttu-id="c8836-176">Настраиваемые текстовые разделы поддерживаются для всех сценариев.</span><span class="sxs-lookup"><span data-stu-id="c8836-176">Custom text-based topics are supported for all scenarios.</span></span>

### <a name="example-1-notify-a-user-about-a-task-created-in-a-chat"></a><span data-ttu-id="c8836-177">Пример 1: уведомление пользователя о задаче, созданной в чате</span><span class="sxs-lookup"><span data-stu-id="c8836-177">Example 1: Notify a user about a task created in a chat</span></span>

<span data-ttu-id="c8836-178">В этом примере показано, как можно отправить уведомление веб-канала активности для новой задачи, созданной в чате.</span><span class="sxs-lookup"><span data-stu-id="c8836-178">This example shows how you can send an activity feed notification for a new task created in a chat.</span></span> <span data-ttu-id="c8836-179">В этом случае приложение Teams должно быть установлено в чате с идентификатором, `chatId` а пользователь `569363e2-4e49-4661-87f2-16f245c5d66a` также должен входить в чат.</span><span class="sxs-lookup"><span data-stu-id="c8836-179">In this case, the Teams app must be installed in a chat with Id `chatId` and user `569363e2-4e49-4661-87f2-16f245c5d66a` must be part of the chat as well.</span></span>

#### <a name="request"></a><span data-ttu-id="c8836-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8836-180">Request</span></span>
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

#### <a name="response"></a><span data-ttu-id="c8836-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8836-181">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-2--notify-a-user-about-a-task-created-in-a-team"></a><span data-ttu-id="c8836-182">Пример 2: уведомление пользователя о задаче, созданной в команде</span><span class="sxs-lookup"><span data-stu-id="c8836-182">Example 2 : Notify a user about a task created in a team</span></span>

<span data-ttu-id="c8836-183">В этом примере показано, как можно отправить уведомление веб-канала активности для команды.</span><span class="sxs-lookup"><span data-stu-id="c8836-183">This example shows how you can send an activity feed notification for a team.</span></span> <span data-ttu-id="c8836-184">В этом примере владелец команды уведомляется о новой созданной задаче, требующей внимания.</span><span class="sxs-lookup"><span data-stu-id="c8836-184">This example notifies the team owner about a new task created that requires their attention.</span></span>

#### <a name="request"></a><span data-ttu-id="c8836-185">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8836-185">Request</span></span>
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

#### <a name="response"></a><span data-ttu-id="c8836-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8836-186">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-3-notify-a-user-about-an-event-using-a-custom-topic"></a><span data-ttu-id="c8836-187">Пример 3: уведомление пользователя о событии с помощью настраиваемого раздела</span><span class="sxs-lookup"><span data-stu-id="c8836-187">Example 3: Notify a user about an event using a custom topic</span></span>

<span data-ttu-id="c8836-188">Как показано в предыдущих примерах, вы можете ссылаться на различные аспекты команды или чата.</span><span class="sxs-lookup"><span data-stu-id="c8836-188">As seen in the previous examples, you can link to different aspects of a team or a chat.</span></span> <span data-ttu-id="c8836-189">Тем не менее, если вы хотите создать ссылку на аспект, который не является частью команды или не представлен в Microsoft Graph, или если вы хотите настроить это имя, вы можете задать для `topic` `text` него значение и передать его настраиваемое значение.</span><span class="sxs-lookup"><span data-stu-id="c8836-189">However, if you want to link to an aspect that is not part of the team or is not represented by Microsoft Graph, or if you want to customize the name, you can set the source of the `topic` to `text` and pass in a custom value for it.</span></span> <span data-ttu-id="c8836-190">Кроме того, `webUrl` является обязательным, если используется `topic` источник AS `text` .</span><span class="sxs-lookup"><span data-stu-id="c8836-190">Additionally, `webUrl` is required when you use `topic` source as `text`.</span></span>

<span data-ttu-id="c8836-191">В примере уведомления Yammer, показанном ранее, используется настраиваемый раздел, так как в Microsoft Graph ресурсы Yammer не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="c8836-191">The Yammer notification example shown earlier uses a custom topic because Yammer's resources are not supported by Microsoft Graph.</span></span>

> <span data-ttu-id="c8836-192">**Примечание:** `webUrl` должна начинаться с домена Microsoft Teams (например, teams.microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="c8836-192">**Note:** `webUrl` must start with the Microsoft Teams domain (teams.microsoft.com for example).</span></span>

#### <a name="request"></a><span data-ttu-id="c8836-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="c8836-193">Request</span></span>
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

#### <a name="response"></a><span data-ttu-id="c8836-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="c8836-194">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

## <a name="customizing-how-the-notifications-alert-you"></a><span data-ttu-id="c8836-195">Настройка оповещения о том, как вы</span><span class="sxs-lookup"><span data-stu-id="c8836-195">Customizing how the notifications alert you</span></span>

<span data-ttu-id="c8836-196">Пользователи Microsoft Teams могут настраивать уведомления, которые они видят в веб-канале, в виде баннера и т. д.</span><span class="sxs-lookup"><span data-stu-id="c8836-196">Microsoft Teams users can customize the notifications they see in their feed, as a banner, and so on.</span></span> <span data-ttu-id="c8836-197">Уведомления, созданные через API веб-каналов активности, также могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c8836-197">Notifications generated through activity feed APIs can also be customized.</span></span> <span data-ttu-id="c8836-198">Пользователи могут выбрать способ уведомления с помощью параметров в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="c8836-198">Users can choose how they are notified via settings in Microsoft Teams.</span></span> <span data-ttu-id="c8836-199">Приложения Teams отобразятся в списке, чтобы выбрать пользователя, как показано на следующем снимке экрана.</span><span class="sxs-lookup"><span data-stu-id="c8836-199">Teams apps will appear in the list for the user to choose from, as shown in the following screenshot.</span></span>

![Снимок экрана с параметрами уведомлений в Teams с выделенным настраиваемым параметром](images/teams-activityfeednotifications/notificationsettings.png)

<span data-ttu-id="c8836-201">Пользователи могут нажать кнопку **изменить** рядом с приложением и настроить уведомления, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="c8836-201">Users can click **Edit** next to an app and customize the notifications, as shown in the following example.</span></span> <span data-ttu-id="c8836-202">`description`Отображается поле в манифесте приложения Teams.</span><span class="sxs-lookup"><span data-stu-id="c8836-202">The `description` field in the Teams app manifest is displayed.</span></span>

![Снимок экрана, на котором показаны уведомления, измененные на баннер и веб-канал для приложения Teams](images/teams-activityfeednotifications/applevelnotificationsettings.png)
