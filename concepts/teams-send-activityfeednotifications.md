---
title: Отправка уведомлений веб-канала активности пользователям в Microsoft Teams
description: Отправка уведомлений веб-канала активности пользователям в Microsoft Teams с помощью приложения Teams и Microsoft Graph.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 940ffba39293a3b01df67c47b6ff6b5e09821767
ms.sourcegitcommit: d02c438bcd58e8f64bfcd5fba0b40e436b46570e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/04/2021
ms.locfileid: "50101897"
---
# <a name="send-activity-feed-notifications-to-users-in-microsoft-teams"></a><span data-ttu-id="1e6ff-103">Отправка уведомлений веб-канала активности пользователям в Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="1e6ff-103">Send activity feed notifications to users in Microsoft Teams</span></span>

<span data-ttu-id="1e6ff-104">Веб-канал активности Microsoft Teams позволяет пользователям делить элементы, которые требуют внимания, уведомляя их об изменениях.</span><span class="sxs-lookup"><span data-stu-id="1e6ff-104">The Microsoft Teams activity feed enables users to triage items that require attention by notifying them of changes.</span></span> <span data-ttu-id="1e6ff-105">Вы можете использовать API уведомлений веб-канала активности в Microsoft Graph, чтобы расширить эту функциональность для ваших приложений.</span><span class="sxs-lookup"><span data-stu-id="1e6ff-105">You can use the activity feed notification APIs in Microsoft Graph to extend this functionality to your apps.</span></span> <span data-ttu-id="1e6ff-106">Это позволяет приложениям предоставлять более богатые опытом и лучше привлекать пользователей, помогая поддерживать их в курсе изменений в средствах и рабочего процессах, которые они используют.</span><span class="sxs-lookup"><span data-stu-id="1e6ff-106">This allows your apps to provide richer experiences and better engage users by helping to keep them up to date with changes in the tools and workflows they use.</span></span>

## <a name="understanding-the-basics-of-activity-feed-notification"></a><span data-ttu-id="1e6ff-107">Основные принципы уведомлений веб-канала активности</span><span class="sxs-lookup"><span data-stu-id="1e6ff-107">Understanding the basics of activity feed notification</span></span>

<span data-ttu-id="1e6ff-108">Уведомления веб-канала активности в Microsoft Teams состоят из нескольких битов информации, отображаемой вместе, как показано на следующем изображении.</span><span class="sxs-lookup"><span data-stu-id="1e6ff-108">Activity feed notifications in Microsoft Teams are comprised of multiple bits of information, displayed together, as shown in the following image.</span></span>

![Изображение, на котором показаны компоненты уведомления веб-канала активности](images/teams-activityfeednotifications/notificationtemplate.png)

<span data-ttu-id="1e6ff-110">К компонентам относятся:</span><span class="sxs-lookup"><span data-stu-id="1e6ff-110">The components include:</span></span>
- <span data-ttu-id="1e6ff-111">Субъект, иницивший действие</span><span class="sxs-lookup"><span data-stu-id="1e6ff-111">The actor who initiated the activity</span></span>
- <span data-ttu-id="1e6ff-112">Значок, который представляет тип действия</span><span class="sxs-lookup"><span data-stu-id="1e6ff-112">An icon that represents the activity type</span></span>
- <span data-ttu-id="1e6ff-113">Причина, по которой субъект сделал действие</span><span class="sxs-lookup"><span data-stu-id="1e6ff-113">The reason the actor did the activity</span></span>
- <span data-ttu-id="1e6ff-114">Предварительный просмотр текста</span><span class="sxs-lookup"><span data-stu-id="1e6ff-114">A text preview</span></span>
- <span data-ttu-id="1e6ff-115">Отметка времени</span><span class="sxs-lookup"><span data-stu-id="1e6ff-115">A time stamp</span></span>
- <span data-ttu-id="1e6ff-116">Расположение действия</span><span class="sxs-lookup"><span data-stu-id="1e6ff-116">The location of the activity</span></span>

<span data-ttu-id="1e6ff-117">В следующем примере показано, как эти компоненты предоставляют сведения об уведомлении.</span><span class="sxs-lookup"><span data-stu-id="1e6ff-117">The following example shows how these components together provide the details about a notification.</span></span> <span data-ttu-id="1e6ff-118">Этот пример является уведомлением о пользователе, упомянутом в сообществе Yammer.</span><span class="sxs-lookup"><span data-stu-id="1e6ff-118">This example is a notification about a user mentioned in a Yammer community.</span></span>

![Пример уведомления о действиях Yammer](images/teams-activityfeednotifications/examplefeednotification.png)

## <a name="requirements-for-using-the-activity-feed-notification-apis"></a><span data-ttu-id="1e6ff-120">Требования для использования API уведомлений веб-канала активности</span><span class="sxs-lookup"><span data-stu-id="1e6ff-120">Requirements for using the activity feed notification APIs</span></span>

<span data-ttu-id="1e6ff-121">API веб-каналов активности работают с [приложением Teams.](/microsoftteams/platform/overview)</span><span class="sxs-lookup"><span data-stu-id="1e6ff-121">Activity feed APIs work with a [Teams app](/microsoftteams/platform/overview).</span></span> <span data-ttu-id="1e6ff-122">Ниже следующую следующую следующую погони за требованиями для отправки уведомлений веб-канала активности:</span><span class="sxs-lookup"><span data-stu-id="1e6ff-122">The following are the requirements for sending activity feed notifications:</span></span>

- <span data-ttu-id="1e6ff-123">Манифест приложения Teams должен иметь добавленный в раздел ИД приложения Azure `webApplicationInfo` AD.</span><span class="sxs-lookup"><span data-stu-id="1e6ff-123">The Teams app manifest must have the Azure AD app ID added to the `webApplicationInfo` section.</span></span> <span data-ttu-id="1e6ff-124">Подробные сведения [см. в схеме манифеста.](/microsoftteams/platform/resources/schema/manifest-schema)</span><span class="sxs-lookup"><span data-stu-id="1e6ff-124">For details, see [manifest schema](/microsoftteams/platform/resources/schema/manifest-schema).</span></span>
- <span data-ttu-id="1e6ff-125">Типы действий должны быть объявлены в `activities` разделе.</span><span class="sxs-lookup"><span data-stu-id="1e6ff-125">Activity types must be declared in the `activities` section.</span></span> <span data-ttu-id="1e6ff-126">Подробные сведения [см. в схеме манифеста.](/microsoftteams/platform/resources/schema/manifest-schema)</span><span class="sxs-lookup"><span data-stu-id="1e6ff-126">For details, see [manifest schema](/microsoftteams/platform/resources/schema/manifest-schema).</span></span>
- <span data-ttu-id="1e6ff-127">Приложение Teams должно быть установлено для получателя либо [](/graph/api/resources/team?preserve-view=true) лично, либо в команде или чате, [в](/graph/api/resources/chat?preserve-view=true) составе группы.</span><span class="sxs-lookup"><span data-stu-id="1e6ff-127">The Teams app must be installed for the recipient, either personally, or in a [team](/graph/api/resources/team?preserve-view=true) or [chat](/graph/api/resources/chat?preserve-view=true) they are part of.</span></span> <span data-ttu-id="1e6ff-128">Дополнительные сведения см. в [установке приложения Teams.](/graph/api/resources/teamsappinstallation?preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="1e6ff-128">For more information, see [Teams app installation](/graph/api/resources/teamsappinstallation?preserve-view=true).</span></span>

### <a name="teams-app-manifest-changes"></a><span data-ttu-id="1e6ff-129">Изменения манифеста приложения Teams</span><span class="sxs-lookup"><span data-stu-id="1e6ff-129">Teams app manifest changes</span></span>

<span data-ttu-id="1e6ff-130">В этом разделе описываются изменения, которые необходимо добавить в манифест приложения Teams.</span><span class="sxs-lookup"><span data-stu-id="1e6ff-130">This section describes the changes that need to be added to Teams app manifest.</span></span> <span data-ttu-id="1e6ff-131">Обратите внимание, что необходимо использовать версию манифеста [приложения Teams](/microsoftteams/platform/resources/schema/manifest-schema) или `1.7` более новую.</span><span class="sxs-lookup"><span data-stu-id="1e6ff-131">Note that you must be using the [Teams app manifest](/microsoftteams/platform/resources/schema/manifest-schema) version `1.7` or greater.</span></span>

```json
"$schema": "https://developer.microsoft.com/json-schemas/teams/v1.7/MicrosoftTeams.schema.json",
"manifestVersion": "1.7",
````

#### <a name="webapplicationinfo-section-changes"></a><span data-ttu-id="1e6ff-132">Изменения раздела webApplicationInfo</span><span class="sxs-lookup"><span data-stu-id="1e6ff-132">webApplicationInfo section changes</span></span>

```json
"webApplicationInfo":
{
    "id": "a3111f15-658e-457c-9689-fd20fe907330",
    "resource": "https://contosoapp.com"
}
```

|<span data-ttu-id="1e6ff-133">Параметр</span><span class="sxs-lookup"><span data-stu-id="1e6ff-133">Parameter</span></span>|<span data-ttu-id="1e6ff-134">Тип</span><span class="sxs-lookup"><span data-stu-id="1e6ff-134">Type</span></span>|<span data-ttu-id="1e6ff-135">Описание</span><span class="sxs-lookup"><span data-stu-id="1e6ff-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e6ff-136">id</span><span class="sxs-lookup"><span data-stu-id="1e6ff-136">id</span></span>|<span data-ttu-id="1e6ff-137">string</span><span class="sxs-lookup"><span data-stu-id="1e6ff-137">string</span></span>|<span data-ttu-id="1e6ff-138">ИД приложения Azure AD (ИД клиента).</span><span class="sxs-lookup"><span data-stu-id="1e6ff-138">Azure AD app ID (client ID).</span></span>|
|<span data-ttu-id="1e6ff-139">resource</span><span class="sxs-lookup"><span data-stu-id="1e6ff-139">resource</span></span>|<span data-ttu-id="1e6ff-140">string</span><span class="sxs-lookup"><span data-stu-id="1e6ff-140">string</span></span>|<span data-ttu-id="1e6ff-141">Ресурс, связанный с приложением Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1e6ff-141">Resource associated with the Azure AD app.</span></span> <span data-ttu-id="1e6ff-142">Также называется URL-адресом ответа или перенаправления на портале Azure.</span><span class="sxs-lookup"><span data-stu-id="1e6ff-142">Also known as reply or redirect URL in the Azure Portal.</span></span>|

> <span data-ttu-id="1e6ff-143">**Примечание.** Ошибка может возникнуть, если несколько приложений Teams в одной области (команда, чат или пользователь) используют одно и то же приложение Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1e6ff-143">**Note:** You might get an error if multiple Teams apps in the same scope (team, chat or user) are using the same Azure AD app.</span></span> <span data-ttu-id="1e6ff-144">Убедитесь, что вы используете уникальные приложения Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1e6ff-144">Make sure that you're using unique Azure AD apps.</span></span>

#### <a name="activities-section-changes"></a><span data-ttu-id="1e6ff-145">изменения раздела действий</span><span class="sxs-lookup"><span data-stu-id="1e6ff-145">activities section changes</span></span>

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

|<span data-ttu-id="1e6ff-146">Параметр</span><span class="sxs-lookup"><span data-stu-id="1e6ff-146">Parameter</span></span>|<span data-ttu-id="1e6ff-147">Тип</span><span class="sxs-lookup"><span data-stu-id="1e6ff-147">Type</span></span>|<span data-ttu-id="1e6ff-148">Описание</span><span class="sxs-lookup"><span data-stu-id="1e6ff-148">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e6ff-149">type</span><span class="sxs-lookup"><span data-stu-id="1e6ff-149">type</span></span>|<span data-ttu-id="1e6ff-150">string</span><span class="sxs-lookup"><span data-stu-id="1e6ff-150">string</span></span>|<span data-ttu-id="1e6ff-151">Тип действия.</span><span class="sxs-lookup"><span data-stu-id="1e6ff-151">Type of activity.</span></span> <span data-ttu-id="1e6ff-152">Это должно быть уникальным в определенном манифесте.</span><span class="sxs-lookup"><span data-stu-id="1e6ff-152">This needs to be unique in a specific manifest.</span></span>|
|<span data-ttu-id="1e6ff-153">description</span><span class="sxs-lookup"><span data-stu-id="1e6ff-153">description</span></span>|<span data-ttu-id="1e6ff-154">string</span><span class="sxs-lookup"><span data-stu-id="1e6ff-154">string</span></span>|<span data-ttu-id="1e6ff-155">Краткое описание, понятное человеку.</span><span class="sxs-lookup"><span data-stu-id="1e6ff-155">Human-readable short description.</span></span> <span data-ttu-id="1e6ff-156">Он будет виден в клиенте Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="1e6ff-156">This will be visible on the Microsoft Teams client.</span></span>|
|<span data-ttu-id="1e6ff-157">templateText</span><span class="sxs-lookup"><span data-stu-id="1e6ff-157">templateText</span></span>|<span data-ttu-id="1e6ff-158">Строка</span><span class="sxs-lookup"><span data-stu-id="1e6ff-158">string</span></span>|<span data-ttu-id="1e6ff-159">Текст шаблона уведомления об активности.</span><span class="sxs-lookup"><span data-stu-id="1e6ff-159">Template text for the activity notification.</span></span> <span data-ttu-id="1e6ff-160">Параметры можно объявить, инкапсулируя параметры в `{}` .</span><span class="sxs-lookup"><span data-stu-id="1e6ff-160">You can declare your parameters by encapsulating parameters in `{}`.</span></span>|

><span data-ttu-id="1e6ff-161">**Примечание.** `actor` — это специальный параметр, который всегда принимает имя вызываемого.</span><span class="sxs-lookup"><span data-stu-id="1e6ff-161">**Note:** `actor` is a special parameter that always takes the name of the caller.</span></span> <span data-ttu-id="1e6ff-162">В делегных вызовах `actor` это имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="1e6ff-162">In delegated calls, `actor` is the user's name.</span></span> <span data-ttu-id="1e6ff-163">В вызовах только для приложений он принимает имя приложения Teams.</span><span class="sxs-lookup"><span data-stu-id="1e6ff-163">In application-only calls, it takes the name of the Teams app.</span></span>

### <a name="installing-the-teams-app"></a><span data-ttu-id="1e6ff-164">Установка приложения Teams</span><span class="sxs-lookup"><span data-stu-id="1e6ff-164">Installing the Teams app</span></span>

<span data-ttu-id="1e6ff-165">Приложения Teams можно устанавливать в команде, чате или лично для пользователя, а также распространять их несколькими способами.</span><span class="sxs-lookup"><span data-stu-id="1e6ff-165">Teams apps can be installed in a team, a chat, or for a user personally, and can be distributed in multiple ways.</span></span> <span data-ttu-id="1e6ff-166">Подробные сведения см. в [методах распространения приложений Teams.](/microsoftteams/platform/concepts/deploy-and-publish/overview)</span><span class="sxs-lookup"><span data-stu-id="1e6ff-166">For details, see [Teams app distribution methods](/microsoftteams/platform/concepts/deploy-and-publish/overview).</span></span> <span data-ttu-id="1e6ff-167">Как правило, [загрузка нео](/microsoftteams/platform/concepts/deploy-and-publish/apps-upload) боков предпочтительна в целях разработки.</span><span class="sxs-lookup"><span data-stu-id="1e6ff-167">Typically, [sideloading](/microsoftteams/platform/concepts/deploy-and-publish/apps-upload) is preferred for development purposes.</span></span> <span data-ttu-id="1e6ff-168">После разработки вы можете выбрать правильный способ распространения в зависимости от того, хотите ли вы распространять их на один или все клиенты.</span><span class="sxs-lookup"><span data-stu-id="1e6ff-168">After development, you can choose the right distribution method based on whether you want to distribute to one tenant or to all tenants.</span></span>

<span data-ttu-id="1e6ff-169">Вы также можете использовать API установки приложений [Teams](/graph/api/resources/teamsappinstallation?preserve-view=true) для управления установками приложений Teams.</span><span class="sxs-lookup"><span data-stu-id="1e6ff-169">You can also use [Teams app installation](/graph/api/resources/teamsappinstallation?preserve-view=true) APIs to manage Teams app installations.</span></span>

## <a name="sending-activity-feed-notifications-to-users"></a><span data-ttu-id="1e6ff-170">Отправка уведомлений веб-канала активности пользователям</span><span class="sxs-lookup"><span data-stu-id="1e6ff-170">Sending activity feed notifications to users</span></span>

<span data-ttu-id="1e6ff-171">Так как приложение Teams можно установить для пользователя, в команде или в чате, уведомления также можно отправить в этих трех контекстах:</span><span class="sxs-lookup"><span data-stu-id="1e6ff-171">Because a Teams app can be installed for a user, in a team, or in a chat, the notifications can be sent in these three contexts as well:</span></span>

- [<span data-ttu-id="1e6ff-172">Отправка уведомления пользователю в чате</span><span class="sxs-lookup"><span data-stu-id="1e6ff-172">Send notification to user in a chat</span></span>](/graph/api/chat-sendactivitynotification)
- [<span data-ttu-id="1e6ff-173">Отправка уведомления пользователю в команде</span><span class="sxs-lookup"><span data-stu-id="1e6ff-173">Send notification to user in a team</span></span>](/graph/api/team-sendactivitynotification)
- [<span data-ttu-id="1e6ff-174">Отправка уведомления пользователю</span><span class="sxs-lookup"><span data-stu-id="1e6ff-174">Send notification to user</span></span>](/graph/api/userteamwork-sendactivitynotification)

<span data-ttu-id="1e6ff-175">Подробные сведения о том, какие темы поддерживаются для каждого сценария, см. в определенных API.</span><span class="sxs-lookup"><span data-stu-id="1e6ff-175">For details about what topics are supported for each scenario, see the specific APIs.</span></span> <span data-ttu-id="1e6ff-176">Настраиваемые текстовые разделы поддерживаются во всех сценариях.</span><span class="sxs-lookup"><span data-stu-id="1e6ff-176">Custom text-based topics are supported for all scenarios.</span></span>

### <a name="example-1-notify-a-user-about-a-task-created-in-a-chat"></a><span data-ttu-id="1e6ff-177">Пример 1. Уведомление пользователя о задаче, созданной в чате</span><span class="sxs-lookup"><span data-stu-id="1e6ff-177">Example 1: Notify a user about a task created in a chat</span></span>

<span data-ttu-id="1e6ff-178">В этом примере показано, как можно отправить уведомление веб-канала активности для новой задачи, созданной в чате.</span><span class="sxs-lookup"><span data-stu-id="1e6ff-178">This example shows how you can send an activity feed notification for a new task created in a chat.</span></span> <span data-ttu-id="1e6ff-179">В этом случае приложение Teams должно быть установлено в чате с ИД, а пользователь также должен быть частью `chatId` `569363e2-4e49-4661-87f2-16f245c5d66a` чата.</span><span class="sxs-lookup"><span data-stu-id="1e6ff-179">In this case, the Teams app must be installed in a chat with Id `chatId` and user `569363e2-4e49-4661-87f2-16f245c5d66a` must be part of the chat as well.</span></span>

#### <a name="request"></a><span data-ttu-id="1e6ff-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="1e6ff-180">Request</span></span>
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

#### <a name="response"></a><span data-ttu-id="1e6ff-181">Отклик</span><span class="sxs-lookup"><span data-stu-id="1e6ff-181">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-notify-a-user-about-a-task-created-in-a-team"></a><span data-ttu-id="1e6ff-182">Пример 2. Уведомление пользователя о задаче, созданной в команде</span><span class="sxs-lookup"><span data-stu-id="1e6ff-182">Example 2: Notify a user about a task created in a team</span></span>

<span data-ttu-id="1e6ff-183">В этом примере показано, как можно отправить уведомление веб-канала активности для команды.</span><span class="sxs-lookup"><span data-stu-id="1e6ff-183">This example shows how you can send an activity feed notification for a team.</span></span> <span data-ttu-id="1e6ff-184">В этом примере владельцу команды сообщается о новой задаче, которая требует внимания.</span><span class="sxs-lookup"><span data-stu-id="1e6ff-184">This example notifies the team owner about a new task created that requires their attention.</span></span>

#### <a name="request"></a><span data-ttu-id="1e6ff-185">Запрос</span><span class="sxs-lookup"><span data-stu-id="1e6ff-185">Request</span></span>
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

#### <a name="response"></a><span data-ttu-id="1e6ff-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="1e6ff-186">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-3-notify-a-user-about-an-event-using-a-custom-topic"></a><span data-ttu-id="1e6ff-187">Пример 3. Уведомление пользователя о событии с помощью настраиваемой темы</span><span class="sxs-lookup"><span data-stu-id="1e6ff-187">Example 3: Notify a user about an event using a custom topic</span></span>

<span data-ttu-id="1e6ff-188">Как видно из предыдущих примеров, вы можете ссылаться на различные аспекты команды или чата.</span><span class="sxs-lookup"><span data-stu-id="1e6ff-188">As seen in the previous examples, you can link to different aspects of a team or a chat.</span></span> <span data-ttu-id="1e6ff-189">Тем не менее, если вы хотите связать аспект, который не является частью команды или не представлен Microsoft Graph, или если вы хотите настроить имя, вы можете установить источник и передать для него пользовательское `topic` `text` значение.</span><span class="sxs-lookup"><span data-stu-id="1e6ff-189">However, if you want to link to an aspect that is not part of the team or is not represented by Microsoft Graph, or if you want to customize the name, you can set the source of the `topic` to `text` and pass in a custom value for it.</span></span> <span data-ttu-id="1e6ff-190">Кроме того, при использовании источника в `webUrl` качестве `topic` `text` .</span><span class="sxs-lookup"><span data-stu-id="1e6ff-190">Additionally, `webUrl` is required when you use `topic` source as `text`.</span></span>

<span data-ttu-id="1e6ff-191">В примере уведомления Yammer, показанного ранее, используется настраиваемый раздел, так как ресурсы Yammer не поддерживаются Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1e6ff-191">The Yammer notification example shown earlier uses a custom topic because Yammer's resources are not supported by Microsoft Graph.</span></span>

> <span data-ttu-id="1e6ff-192">**Примечание.** `webUrl` должен начинаться с домена Microsoft Teams (teams.microsoft.com например).</span><span class="sxs-lookup"><span data-stu-id="1e6ff-192">**Note:** `webUrl` must start with the Microsoft Teams domain (teams.microsoft.com for example).</span></span>

#### <a name="request"></a><span data-ttu-id="1e6ff-193">Запрос</span><span class="sxs-lookup"><span data-stu-id="1e6ff-193">Request</span></span>
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

#### <a name="response"></a><span data-ttu-id="1e6ff-194">Отклик</span><span class="sxs-lookup"><span data-stu-id="1e6ff-194">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

## <a name="customizing-how-the-notifications-alert-you"></a><span data-ttu-id="1e6ff-195">Настройка оповещения уведомлений</span><span class="sxs-lookup"><span data-stu-id="1e6ff-195">Customizing how the notifications alert you</span></span>

<span data-ttu-id="1e6ff-196">Пользователи Microsoft Teams могут настраивать уведомления, которые они видят в веб-канале, в качестве баннера и так далее.</span><span class="sxs-lookup"><span data-stu-id="1e6ff-196">Microsoft Teams users can customize the notifications they see in their feed, as a banner, and so on.</span></span> <span data-ttu-id="1e6ff-197">Уведомления, созданные с помощью API веб-каналов активности, также можно настроить.</span><span class="sxs-lookup"><span data-stu-id="1e6ff-197">Notifications generated through activity feed APIs can also be customized.</span></span> <span data-ttu-id="1e6ff-198">Пользователи могут выбрать, как они будут уведомлены с помощью параметров в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="1e6ff-198">Users can choose how they are notified via settings in Microsoft Teams.</span></span> <span data-ttu-id="1e6ff-199">Приложения Teams появятся в списке для выбора пользователем, как показано на следующем снимке экрана.</span><span class="sxs-lookup"><span data-stu-id="1e6ff-199">Teams apps will appear in the list for the user to choose from, as shown in the following screenshot.</span></span>

![Снимок экрана: параметры уведомлений в Teams с выделенной настройкой](images/teams-activityfeednotifications/notificationsettings.png)

<span data-ttu-id="1e6ff-201">Пользователи могут **нажать** кнопку "Изменить" рядом с приложением и настроить уведомления, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="1e6ff-201">Users can click **Edit** next to an app and customize the notifications, as shown in the following example.</span></span> <span data-ttu-id="1e6ff-202">Отображается `description` поле в манифесте приложения Teams.</span><span class="sxs-lookup"><span data-stu-id="1e6ff-202">The `description` field in the Teams app manifest is displayed.</span></span>

![Снимок экрана: уведомления, настроенные на баннер и веб-канал для приложения Teams](images/teams-activityfeednotifications/applevelnotificationsettings.png)

## <a name="faqs"></a><span data-ttu-id="1e6ff-204">Вопросы и ответы</span><span class="sxs-lookup"><span data-stu-id="1e6ff-204">FAQs</span></span>

### <a name="who-needs-to-install-the-teams-app"></a><span data-ttu-id="1e6ff-205">Кому необходимо установить приложение Teams?</span><span class="sxs-lookup"><span data-stu-id="1e6ff-205">Who needs to install the Teams app?</span></span>

<span data-ttu-id="1e6ff-206">У целевого пользователя должно быть установлено приложение Teams, которое отправляет уведомления.</span><span class="sxs-lookup"><span data-stu-id="1e6ff-206">The target user must have the Teams app that is sending notifications installed.</span></span>

### <a name="can-a-user-send-notifications-to-themselves"></a><span data-ttu-id="1e6ff-207">Может ли пользователь отправлять уведомления себе?</span><span class="sxs-lookup"><span data-stu-id="1e6ff-207">Can a user send notifications to themselves?</span></span>

<span data-ttu-id="1e6ff-208">Нет, пользователь не может отправлять уведомления себе.</span><span class="sxs-lookup"><span data-stu-id="1e6ff-208">No, a user cannot send notifications to themselves.</span></span> <span data-ttu-id="1e6ff-209">В этом сценарии используйте разрешения приложений.</span><span class="sxs-lookup"><span data-stu-id="1e6ff-209">For this scenario, use application permissions.</span></span>

### <a name="can-a-teams-app-control-how-the-notifications-are-shown-to-the-user"></a><span data-ttu-id="1e6ff-210">Может ли приложение Teams управлять тем, как уведомления показываются пользователю?</span><span class="sxs-lookup"><span data-stu-id="1e6ff-210">Can a Teams app control how the notifications are shown to the user?</span></span>

<span data-ttu-id="1e6ff-211">Нет, изменять параметры уведомлений могут только пользователи.</span><span class="sxs-lookup"><span data-stu-id="1e6ff-211">No, only users are allowed to change notification settings.</span></span>

### <a name="i-installed-my-app-why-dont-i-see-notification-settings-under-the-user-account"></a><span data-ttu-id="1e6ff-212">Я установил свое приложение, почему я не вижу параметры уведомлений под учетной записью пользователя?</span><span class="sxs-lookup"><span data-stu-id="1e6ff-212">I installed my app, why don't I see notification settings under the user account?</span></span>

<span data-ttu-id="1e6ff-213">Параметры отображаются после того, как приложение Teams отправляет первое уведомление.</span><span class="sxs-lookup"><span data-stu-id="1e6ff-213">The settings will appear after the first notification is sent by the Teams app.</span></span> <span data-ttu-id="1e6ff-214">Это уменьшает количество параметров, которые видят пользователи.</span><span class="sxs-lookup"><span data-stu-id="1e6ff-214">This reduces the number of settings that users see.</span></span>

### <a name="i-started-getting-a-409-conflict-error-how-do-i-resolve-it"></a><span data-ttu-id="1e6ff-215">Я начал получать ошибку 409 (конфликт), как ее устранить?</span><span class="sxs-lookup"><span data-stu-id="1e6ff-215">I started getting a 409 (conflict) error, how do I resolve it?</span></span>

<span data-ttu-id="1e6ff-216">`Conflict` ошибки в основном возникают, когда несколько приложений Teams, установленных в одной области (команда, чат, пользователь и так далее), имеют одинаковый appId Azure AD в разделе `webApplicationInfo` манифеста.</span><span class="sxs-lookup"><span data-stu-id="1e6ff-216">`Conflict` errors primarily occur when multiple Teams apps installed in the same scope (team, chat, user, and so on) have the same Azure AD appId in the `webApplicationInfo` section of the manifest.</span></span> <span data-ttu-id="1e6ff-217">В этом случае вы получите такую ошибку, как `Found multiple applications with the same Azure AD App ID 'Your AzureAD AppId'.` .</span><span class="sxs-lookup"><span data-stu-id="1e6ff-217">When this happens, you will get an error such as `Found multiple applications with the same Azure AD App ID 'Your AzureAD AppId'.`.</span></span> <span data-ttu-id="1e6ff-218">Убедитесь, что вы используете уникальные приложения Azure AD для уникальных приложений Teams.</span><span class="sxs-lookup"><span data-stu-id="1e6ff-218">Make sure that you use unique Azure AD apps for unique Teams apps.</span></span> <span data-ttu-id="1e6ff-219">Обратите внимание, что одно и то же приложение Teams может быть установлено в нескольких сферах (например, для команды и пользователя).</span><span class="sxs-lookup"><span data-stu-id="1e6ff-219">Note that you can have the same Teams app installed in multiple scopes (team + user for example).</span></span>


