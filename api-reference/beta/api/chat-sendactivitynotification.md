---
title: 'чат: sendActivityNotification'
description: Отправьте уведомление о канале действий в области чата.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3da2bff0c6ea8997a880c93044cc09f962825562
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207506"
---
# <a name="chat-sendactivitynotification"></a><span data-ttu-id="02cb9-103">чат: sendActivityNotification</span><span class="sxs-lookup"><span data-stu-id="02cb9-103">chat: sendActivityNotification</span></span>
<span data-ttu-id="02cb9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02cb9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02cb9-105">Отправьте уведомление о канале действий в области чата.</span><span class="sxs-lookup"><span data-stu-id="02cb9-105">Send an activity feed notification in scope of a chat.</span></span> <span data-ttu-id="02cb9-106">Дополнительные сведения об отправке уведомлений и требованиях к этому см. в Teams [действия.](/graph/teams-send-activityfeednotifications)</span><span class="sxs-lookup"><span data-stu-id="02cb9-106">For more details about sending notifications and the requirements for doing so, see [sending Teams activity notifications](/graph/teams-send-activityfeednotifications).</span></span>

## <a name="permissions"></a><span data-ttu-id="02cb9-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="02cb9-107">Permissions</span></span>
<span data-ttu-id="02cb9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02cb9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02cb9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="02cb9-110">Permission type</span></span>|<span data-ttu-id="02cb9-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="02cb9-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02cb9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="02cb9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="02cb9-113">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="02cb9-113">TeamsActivity.Send</span></span>|
|<span data-ttu-id="02cb9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="02cb9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02cb9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02cb9-115">Not Supported.</span></span>|
|<span data-ttu-id="02cb9-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="02cb9-116">Application</span></span>|<span data-ttu-id="02cb9-117">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="02cb9-117">TeamsActivity.Send</span></span>|

## <a name="http-request"></a><span data-ttu-id="02cb9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="02cb9-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /chats/{chatId}/sendActivityNotification
```

## <a name="request-headers"></a><span data-ttu-id="02cb9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="02cb9-119">Request headers</span></span>
|<span data-ttu-id="02cb9-120">Имя</span><span class="sxs-lookup"><span data-stu-id="02cb9-120">Name</span></span>|<span data-ttu-id="02cb9-121">Описание</span><span class="sxs-lookup"><span data-stu-id="02cb9-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="02cb9-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="02cb9-122">Authorization</span></span>|<span data-ttu-id="02cb9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="02cb9-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="02cb9-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="02cb9-125">Content-Type</span></span>|<span data-ttu-id="02cb9-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="02cb9-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="02cb9-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="02cb9-128">Request body</span></span>
<span data-ttu-id="02cb9-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="02cb9-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="02cb9-130">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="02cb9-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="02cb9-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="02cb9-131">Parameter</span></span>|<span data-ttu-id="02cb9-132">Тип</span><span class="sxs-lookup"><span data-stu-id="02cb9-132">Type</span></span>|<span data-ttu-id="02cb9-133">Описание</span><span class="sxs-lookup"><span data-stu-id="02cb9-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02cb9-134">topic</span><span class="sxs-lookup"><span data-stu-id="02cb9-134">topic</span></span>|[<span data-ttu-id="02cb9-135">teamworkActivityTopic</span><span class="sxs-lookup"><span data-stu-id="02cb9-135">teamworkActivityTopic</span></span>](../resources/teamworkactivitytopic.md)|<span data-ttu-id="02cb9-136">Тема уведомления.</span><span class="sxs-lookup"><span data-stu-id="02cb9-136">Topic of the notification.</span></span> <span data-ttu-id="02cb9-137">Указывает обсуждаемый ресурс.</span><span class="sxs-lookup"><span data-stu-id="02cb9-137">Specifies the resource being talked about.</span></span>|
|<span data-ttu-id="02cb9-138">activityType</span><span class="sxs-lookup"><span data-stu-id="02cb9-138">activityType</span></span>|<span data-ttu-id="02cb9-139">String</span><span class="sxs-lookup"><span data-stu-id="02cb9-139">String</span></span>|<span data-ttu-id="02cb9-140">Тип действия.</span><span class="sxs-lookup"><span data-stu-id="02cb9-140">Activity type.</span></span> <span data-ttu-id="02cb9-141">Это должно быть объявлено в [манифесте Teams приложения](/microsoftteams/platform/overview).</span><span class="sxs-lookup"><span data-stu-id="02cb9-141">This must be declared in the [Teams app manifest](/microsoftteams/platform/overview).</span></span>|
|<span data-ttu-id="02cb9-142">chainId</span><span class="sxs-lookup"><span data-stu-id="02cb9-142">chainId</span></span>|<span data-ttu-id="02cb9-143">Int64</span><span class="sxs-lookup"><span data-stu-id="02cb9-143">Int64</span></span>|<span data-ttu-id="02cb9-144">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="02cb9-144">Optional.</span></span> <span data-ttu-id="02cb9-145">Используется для переопределения предыдущего уведомления.</span><span class="sxs-lookup"><span data-stu-id="02cb9-145">Used to override a previous notification.</span></span> <span data-ttu-id="02cb9-146">Используйте то же `chainId` самое в последующих запросах для переопределения предыдущего уведомления.</span><span class="sxs-lookup"><span data-stu-id="02cb9-146">Use the same `chainId` in subsequent requests to override the previous notification.</span></span>|
|<span data-ttu-id="02cb9-147">previewText</span><span class="sxs-lookup"><span data-stu-id="02cb9-147">previewText</span></span>|[<span data-ttu-id="02cb9-148">itemBody</span><span class="sxs-lookup"><span data-stu-id="02cb9-148">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="02cb9-149">Предварительный текст уведомления.</span><span class="sxs-lookup"><span data-stu-id="02cb9-149">Preview text for the notification.</span></span> <span data-ttu-id="02cb9-150">Microsoft Teams только первые 150 символов.</span><span class="sxs-lookup"><span data-stu-id="02cb9-150">Microsoft Teams will only show first 150 characters.</span></span>|
|<span data-ttu-id="02cb9-151">templateParameters</span><span class="sxs-lookup"><span data-stu-id="02cb9-151">templateParameters</span></span>|<span data-ttu-id="02cb9-152">Коллекция [keyValuePair](../resources/keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="02cb9-152">[keyValuePair](../resources/keyvaluepair.md) collection</span></span>|<span data-ttu-id="02cb9-153">Значения переменных шаблонов, определенных в записи ленты действий, соответствующие манифесту `activityType` [Teams приложения.](/microsoftteams/platform/overview)</span><span class="sxs-lookup"><span data-stu-id="02cb9-153">Values for template variables defined in the activity feed entry corresponding to `activityType` in [Teams app manifest](/microsoftteams/platform/overview).</span></span>|
|<span data-ttu-id="02cb9-154">получатель;</span><span class="sxs-lookup"><span data-stu-id="02cb9-154">recipient</span></span>|[<span data-ttu-id="02cb9-155">teamworkNotificationRecipient</span><span class="sxs-lookup"><span data-stu-id="02cb9-155">teamworkNotificationRecipient</span></span>](../resources/teamworknotificationrecipient.md)|<span data-ttu-id="02cb9-156">Получатель уведомления.</span><span class="sxs-lookup"><span data-stu-id="02cb9-156">Recipient of the notification.</span></span> <span data-ttu-id="02cb9-157">См. [также aadUserNotificationRecipient](../resources/aadusernotificationrecipient.md) и [chatMembersNotificationRecipient](../resources/chatmembersnotificationrecipient.md).</span><span class="sxs-lookup"><span data-stu-id="02cb9-157">See also [aadUserNotificationRecipient](../resources/aadusernotificationrecipient.md) and [chatMembersNotificationRecipient](../resources/chatmembersnotificationrecipient.md).</span></span> |

<span data-ttu-id="02cb9-158">При настройке значения свойства темы для следующих ресурсов `source` поддерживаются следующие  `entityURL` ресурсы:</span><span class="sxs-lookup"><span data-stu-id="02cb9-158">The following resources are supported when setting the `source` value of the **topic** property to `entityURL`:</span></span>

- [<span data-ttu-id="02cb9-159">chat</span><span class="sxs-lookup"><span data-stu-id="02cb9-159">chat</span></span>](../resources/chat.md)
- [<span data-ttu-id="02cb9-160">chatMessage</span><span class="sxs-lookup"><span data-stu-id="02cb9-160">chatMessage</span></span>](../resources/chatmessage.md)

> <span data-ttu-id="02cb9-161">**Примечание:** URL-адрес объекта должен быть таким же, как или детский ресурс чата в URL-адресе.</span><span class="sxs-lookup"><span data-stu-id="02cb9-161">**Note:** The entity URL must be the same as or a child resource of the chat in the URL.</span></span> <span data-ttu-id="02cb9-162">Кроме того, [Teams приложение должно](/microsoftteams/platform/overview) быть установлено в чате.</span><span class="sxs-lookup"><span data-stu-id="02cb9-162">Additionally, the [Teams app](/microsoftteams/platform/overview) must be installed in the chat.</span></span>

## <a name="response"></a><span data-ttu-id="02cb9-163">Ответ</span><span class="sxs-lookup"><span data-stu-id="02cb9-163">Response</span></span>

<span data-ttu-id="02cb9-164">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="02cb9-164">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="02cb9-165">Примеры</span><span class="sxs-lookup"><span data-stu-id="02cb9-165">Examples</span></span>

### <a name="example-1-notify-a-user-about-a-task-created-in-a-chat"></a><span data-ttu-id="02cb9-166">Пример 1. Уведомление пользователя о задаче, созданной в чате</span><span class="sxs-lookup"><span data-stu-id="02cb9-166">Example 1: Notify a user about a task created in a chat</span></span>

<span data-ttu-id="02cb9-167">В этом примере показано, как можно отправить уведомление о ленте действий для новой задачи, созданной в чате.</span><span class="sxs-lookup"><span data-stu-id="02cb9-167">This example shows how you can send an activity feed notification for a new task created in a chat.</span></span> <span data-ttu-id="02cb9-168">Дополнительные сведения см. [в Teams уведомлений об активности.](/graph/teams-send-activityfeednotifications)</span><span class="sxs-lookup"><span data-stu-id="02cb9-168">For more details, see [sending Teams activity notifications](/graph/teams-send-activityfeednotifications).</span></span>

#### <a name="request"></a><span data-ttu-id="02cb9-169">Запрос</span><span class="sxs-lookup"><span data-stu-id="02cb9-169">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="02cb9-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="02cb9-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chat_sendactivitynotification_1"
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
            "value": "Task 12322"
        }
    ] 
}
```
# <a name="c"></a>[<span data-ttu-id="02cb9-171">C#</span><span class="sxs-lookup"><span data-stu-id="02cb9-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chat-sendactivitynotification-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="02cb9-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="02cb9-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chat-sendactivitynotification-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="02cb9-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="02cb9-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chat-sendactivitynotification-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="02cb9-174">Java</span><span class="sxs-lookup"><span data-stu-id="02cb9-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chat-sendactivitynotification-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="02cb9-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="02cb9-175">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-notify-a-user-about-an-approval-needed-in-a-chat-message"></a><span data-ttu-id="02cb9-176">Пример 2. Уведомление пользователя об утверждении, необходимом в сообщении чата</span><span class="sxs-lookup"><span data-stu-id="02cb9-176">Example 2: Notify a user about an approval needed in a chat message</span></span>

<span data-ttu-id="02cb9-177">Как и в предыдущем примере, в этом примере `entityUrl` используется `topic` для .</span><span class="sxs-lookup"><span data-stu-id="02cb9-177">Similar to the previous example, this example uses `entityUrl` for the `topic`.</span></span> <span data-ttu-id="02cb9-178">Однако в этом случае он связывается с сообщением в чате.</span><span class="sxs-lookup"><span data-stu-id="02cb9-178">However, in this case, it links to a message in the chat.</span></span> <span data-ttu-id="02cb9-179">В сообщении может быть карточка с кнопкой утверждения.</span><span class="sxs-lookup"><span data-stu-id="02cb9-179">The message can contains a card with the approval button on it.</span></span>

#### <a name="request"></a><span data-ttu-id="02cb9-180">Запрос</span><span class="sxs-lookup"><span data-stu-id="02cb9-180">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="02cb9-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="02cb9-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chat_sendactivitynotification_2"
}
-->
``` http
POST https://graph.microsoft.com/beta/chats/{chatId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/beta/chats/{chatId}/messages/{messageId}"
    },
    "activityType": "approvalRequired",
    "previewText": {
        "content": "Deployment requires your approval"
    },
    "recipient": {
        "@odata.type": "Microsoft.Teams.GraphSvc.aadUserNotificationRecipient",
        "userId": "569363e2-4e49-4661-87f2-16f245c5d66a"
    },
    "templateParameters": [
        {
            "name": "approvalTaskId",
            "value": "2020AAGGTAPP"
        }
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="02cb9-182">C#</span><span class="sxs-lookup"><span data-stu-id="02cb9-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chat-sendactivitynotification-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="02cb9-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="02cb9-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chat-sendactivitynotification-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="02cb9-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="02cb9-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chat-sendactivitynotification-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="02cb9-185">Java</span><span class="sxs-lookup"><span data-stu-id="02cb9-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chat-sendactivitynotification-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="02cb9-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="02cb9-186">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-3-notify-a-user-about-an-event-in-relation-to-a-chat"></a><span data-ttu-id="02cb9-187">Пример 3. Уведомление пользователя о событии по отношению к чату</span><span class="sxs-lookup"><span data-stu-id="02cb9-187">Example 3: Notify a user about an event in relation to a chat</span></span>

<span data-ttu-id="02cb9-188">Как показано в предыдущих примерах, вы можете связаться с различными аспектами чата.</span><span class="sxs-lookup"><span data-stu-id="02cb9-188">As shown in the previous examples, you can link to different aspects of the chat.</span></span> <span data-ttu-id="02cb9-189">Однако, если вы хотите связаться с аспектом, который не является частью чата или не представлен Microsoft Graph, вы можете установить источник и передать в настраиваемом значении для `topic` `text` него.</span><span class="sxs-lookup"><span data-stu-id="02cb9-189">However, if you want to link to an aspect that is not part of the chat, or is not represented by Microsoft Graph, you can set the source of the `topic` to `text` and pass in a custom value for it.</span></span> <span data-ttu-id="02cb9-190">Кроме того, `webUrl` требуется при настройке `topic` источника для `text` .</span><span class="sxs-lookup"><span data-stu-id="02cb9-190">Also, `webUrl` is required when setting `topic` source to `text`.</span></span>

#### <a name="request"></a><span data-ttu-id="02cb9-191">Запрос</span><span class="sxs-lookup"><span data-stu-id="02cb9-191">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="02cb9-192">HTTP</span><span class="sxs-lookup"><span data-stu-id="02cb9-192">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chat_sendactivitynotification_3"
}
-->
``` http
POST https://graph.microsoft.com/beta/chats/{chatId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "text",
        "value": "Deployment Approvals Channel",
        "webUrl": "https://teams.microsoft.com/l/message/19:448cfd2ac2a7490a9084a9ed14cttr78c@thread.skype/1605223780000?tenantId=c8b1bf45-3834-4ecf-971a-b4c755ee677d&groupId=d4c2a937-f097-435a-bc91-5c1683ca7245&parentMessageId=1605223771864&teamName=Approvals&channelName=Azure%20DevOps&createdTime=1605223780000"
    },
    "activityType": "deploymentApprovalRequired",
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
# <a name="c"></a>[<span data-ttu-id="02cb9-193">C#</span><span class="sxs-lookup"><span data-stu-id="02cb9-193">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chat-sendactivitynotification-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="02cb9-194">JavaScript</span><span class="sxs-lookup"><span data-stu-id="02cb9-194">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chat-sendactivitynotification-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="02cb9-195">Objective-C</span><span class="sxs-lookup"><span data-stu-id="02cb9-195">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chat-sendactivitynotification-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="02cb9-196">Java</span><span class="sxs-lookup"><span data-stu-id="02cb9-196">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chat-sendactivitynotification-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="02cb9-197">Отклик</span><span class="sxs-lookup"><span data-stu-id="02cb9-197">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-4-notify-the-chat-members-about-a-task-created-in-a-chat"></a><span data-ttu-id="02cb9-198">Пример 4. Уведомление участников чата о задаче, созданной в чате.</span><span class="sxs-lookup"><span data-stu-id="02cb9-198">Example 4: Notify the chat members about a task created in a chat</span></span>

<span data-ttu-id="02cb9-199">В этом примере показано, как можно отправить уведомление о канале действий всем участникам чата.</span><span class="sxs-lookup"><span data-stu-id="02cb9-199">This example shows how you can send an activity feed notification to all chat members.</span></span> <span data-ttu-id="02cb9-200">Этот пример похож на предыдущие примеры.</span><span class="sxs-lookup"><span data-stu-id="02cb9-200">This example is similar to previous examples.</span></span> <span data-ttu-id="02cb9-201">Однако в этом случае это `recipient` [chatMembersNotificationRecipient](../resources/chatmembersnotificationrecipient.md).</span><span class="sxs-lookup"><span data-stu-id="02cb9-201">However, in this case, the `recipient` is a [chatMembersNotificationRecipient](../resources/chatmembersnotificationrecipient.md).</span></span> <span data-ttu-id="02cb9-202">Обратите `chatId` внимание, что указанный в `recipient` должен соответствовать указанному `chatId` в URL-адресе запроса.</span><span class="sxs-lookup"><span data-stu-id="02cb9-202">Note that the `chatId` specified in the `recipient` must match the `chatId` specified in the request URL.</span></span>

#### <a name="request"></a><span data-ttu-id="02cb9-203">Запрос</span><span class="sxs-lookup"><span data-stu-id="02cb9-203">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "chat_sendactivitynotification_4"
}
-->

``` http
POST https://graph.microsoft.com/beta/chats/19:1c3af46e9e0f4a5293343c8813c47619@thread.v2/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/beta/chats/19:1c3af46e9e0f4a5293343c8813c47619@thread.v2"
    },
    "activityType": "taskCreated",
    "previewText": {
        "content": "New Task Created"
    },
    "recipient": {
        "@odata.type": "microsoft.graph.chatMembersNotificationRecipient",
        "chatId": "19:1c3af46e9e0f4a5293343c8813c47619@thread.v2"
    },
    "templateParameters": [
        {
            "name": "taskId",
            "value": "Task 12322"
        }
    ] 
}
```

#### <a name="response"></a><span data-ttu-id="02cb9-204">Отклик</span><span class="sxs-lookup"><span data-stu-id="02cb9-204">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```
