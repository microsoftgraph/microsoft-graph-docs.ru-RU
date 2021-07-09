---
title: 'чат: sendActivityNotification'
description: Отправьте уведомление о канале действий в области чата.
author: eddie-lee-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1e3cd2d0ad69924ee5ca1b672a5cac12b3b63c69
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2021
ms.locfileid: "53333956"
---
# <a name="chat-sendactivitynotification"></a><span data-ttu-id="206b1-103">чат: sendActivityNotification</span><span class="sxs-lookup"><span data-stu-id="206b1-103">chat: sendActivityNotification</span></span>
<span data-ttu-id="206b1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="206b1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="206b1-105">Отправьте уведомление о канале действий в области чата.</span><span class="sxs-lookup"><span data-stu-id="206b1-105">Send an activity feed notification in scope of a chat.</span></span> <span data-ttu-id="206b1-106">Дополнительные сведения об отправке уведомлений и требованиях к этому см. в Teams [действия.](/graph/teams-send-activityfeednotifications)</span><span class="sxs-lookup"><span data-stu-id="206b1-106">For more details about sending notifications and the requirements for doing so, see [sending Teams activity notifications](/graph/teams-send-activityfeednotifications).</span></span>

## <a name="permissions"></a><span data-ttu-id="206b1-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="206b1-107">Permissions</span></span>
<span data-ttu-id="206b1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="206b1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="206b1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="206b1-110">Permission type</span></span>|<span data-ttu-id="206b1-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="206b1-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="206b1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="206b1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="206b1-113">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="206b1-113">TeamsActivity.Send</span></span>|
|<span data-ttu-id="206b1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="206b1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="206b1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="206b1-115">Not Supported.</span></span>|
|<span data-ttu-id="206b1-116">Application</span><span class="sxs-lookup"><span data-stu-id="206b1-116">Application</span></span>|<span data-ttu-id="206b1-117">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="206b1-117">TeamsActivity.Send</span></span>|

## <a name="http-request"></a><span data-ttu-id="206b1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="206b1-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /chats/{chatId}/sendActivityNotification
```

## <a name="request-headers"></a><span data-ttu-id="206b1-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="206b1-119">Request headers</span></span>
|<span data-ttu-id="206b1-120">Имя</span><span class="sxs-lookup"><span data-stu-id="206b1-120">Name</span></span>|<span data-ttu-id="206b1-121">Описание</span><span class="sxs-lookup"><span data-stu-id="206b1-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="206b1-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="206b1-122">Authorization</span></span>|<span data-ttu-id="206b1-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="206b1-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="206b1-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="206b1-125">Content-Type</span></span>|<span data-ttu-id="206b1-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="206b1-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="206b1-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="206b1-128">Request body</span></span>
<span data-ttu-id="206b1-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="206b1-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="206b1-130">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="206b1-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="206b1-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="206b1-131">Parameter</span></span>|<span data-ttu-id="206b1-132">Тип</span><span class="sxs-lookup"><span data-stu-id="206b1-132">Type</span></span>|<span data-ttu-id="206b1-133">Описание</span><span class="sxs-lookup"><span data-stu-id="206b1-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="206b1-134">topic</span><span class="sxs-lookup"><span data-stu-id="206b1-134">topic</span></span>|[<span data-ttu-id="206b1-135">teamworkActivityTopic</span><span class="sxs-lookup"><span data-stu-id="206b1-135">teamworkActivityTopic</span></span>](../resources/teamworkactivitytopic.md)|<span data-ttu-id="206b1-136">Тема уведомления.</span><span class="sxs-lookup"><span data-stu-id="206b1-136">Topic of the notification.</span></span> <span data-ttu-id="206b1-137">Указывает обсуждаемый ресурс.</span><span class="sxs-lookup"><span data-stu-id="206b1-137">Specifies the resource being talked about.</span></span>|
|<span data-ttu-id="206b1-138">activityType</span><span class="sxs-lookup"><span data-stu-id="206b1-138">activityType</span></span>|<span data-ttu-id="206b1-139">String</span><span class="sxs-lookup"><span data-stu-id="206b1-139">String</span></span>|<span data-ttu-id="206b1-140">Тип действия.</span><span class="sxs-lookup"><span data-stu-id="206b1-140">Activity type.</span></span> <span data-ttu-id="206b1-141">Это должно быть объявлено в [манифесте Teams приложения](/microsoftteams/platform/overview).</span><span class="sxs-lookup"><span data-stu-id="206b1-141">This must be declared in the [Teams app manifest](/microsoftteams/platform/overview).</span></span>|
|<span data-ttu-id="206b1-142">chainId</span><span class="sxs-lookup"><span data-stu-id="206b1-142">chainId</span></span>|<span data-ttu-id="206b1-143">Int64</span><span class="sxs-lookup"><span data-stu-id="206b1-143">Int64</span></span>|<span data-ttu-id="206b1-144">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="206b1-144">Optional.</span></span> <span data-ttu-id="206b1-145">Используется для переопределения предыдущего уведомления.</span><span class="sxs-lookup"><span data-stu-id="206b1-145">Used to override a previous notification.</span></span> <span data-ttu-id="206b1-146">Используйте то же `chainId` самое в последующих запросах для переопределения предыдущего уведомления.</span><span class="sxs-lookup"><span data-stu-id="206b1-146">Use the same `chainId` in subsequent requests to override the previous notification.</span></span>|
|<span data-ttu-id="206b1-147">previewText</span><span class="sxs-lookup"><span data-stu-id="206b1-147">previewText</span></span>|[<span data-ttu-id="206b1-148">itemBody</span><span class="sxs-lookup"><span data-stu-id="206b1-148">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="206b1-149">Предварительный текст уведомления.</span><span class="sxs-lookup"><span data-stu-id="206b1-149">Preview text for the notification.</span></span> <span data-ttu-id="206b1-150">Microsoft Teams только первые 150 символов.</span><span class="sxs-lookup"><span data-stu-id="206b1-150">Microsoft Teams will only show first 150 characters.</span></span>|
|<span data-ttu-id="206b1-151">templateParameters</span><span class="sxs-lookup"><span data-stu-id="206b1-151">templateParameters</span></span>|<span data-ttu-id="206b1-152">Коллекция [keyValuePair](../resources/keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="206b1-152">[keyValuePair](../resources/keyvaluepair.md) collection</span></span>|<span data-ttu-id="206b1-153">Значения переменных шаблонов, определенных в записи ленты действий, соответствующие манифесту `activityType` [Teams приложения.](/microsoftteams/platform/overview)</span><span class="sxs-lookup"><span data-stu-id="206b1-153">Values for template variables defined in the activity feed entry corresponding to `activityType` in [Teams app manifest](/microsoftteams/platform/overview).</span></span>|
|<span data-ttu-id="206b1-154">получатель;</span><span class="sxs-lookup"><span data-stu-id="206b1-154">recipient</span></span>|[<span data-ttu-id="206b1-155">teamworkNotificationRecipient</span><span class="sxs-lookup"><span data-stu-id="206b1-155">teamworkNotificationRecipient</span></span>](../resources/teamworknotificationrecipient.md)|<span data-ttu-id="206b1-156">Получатель уведомления.</span><span class="sxs-lookup"><span data-stu-id="206b1-156">Recipient of the notification.</span></span> <span data-ttu-id="206b1-157">Поддерживаются только пользователи Azure AD.</span><span class="sxs-lookup"><span data-stu-id="206b1-157">Only Azure AD users are supported.</span></span> <span data-ttu-id="206b1-158">См. [также aadUserNotificationRecipient](../resources/aadusernotificationrecipient.md).</span><span class="sxs-lookup"><span data-stu-id="206b1-158">See also [aadUserNotificationRecipient](../resources/aadusernotificationrecipient.md).</span></span> |

<span data-ttu-id="206b1-159">При настройке значения свойства темы для следующих ресурсов `source` поддерживаются следующие  `entityURL` ресурсы:</span><span class="sxs-lookup"><span data-stu-id="206b1-159">The following resources are supported when setting the `source` value of the **topic** property to `entityURL`:</span></span>

- [<span data-ttu-id="206b1-160">chat</span><span class="sxs-lookup"><span data-stu-id="206b1-160">chat</span></span>](../resources/chat.md)
- [<span data-ttu-id="206b1-161">chatMessage</span><span class="sxs-lookup"><span data-stu-id="206b1-161">chatMessage</span></span>](../resources/chatmessage.md)

> <span data-ttu-id="206b1-162">**Примечание:** URL-адрес объекта должен быть таким же, как или детский ресурс чата в URL-адресе.</span><span class="sxs-lookup"><span data-stu-id="206b1-162">**Note:** The entity URL must be the same as or a child resource of the chat in the URL.</span></span> <span data-ttu-id="206b1-163">Кроме того, [Teams приложение должно](/microsoftteams/platform/overview) быть установлено в чате.</span><span class="sxs-lookup"><span data-stu-id="206b1-163">Additionally, the [Teams app](/microsoftteams/platform/overview) must be installed in the chat.</span></span>

## <a name="response"></a><span data-ttu-id="206b1-164">Ответ</span><span class="sxs-lookup"><span data-stu-id="206b1-164">Response</span></span>

<span data-ttu-id="206b1-165">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="206b1-165">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="206b1-166">Примеры</span><span class="sxs-lookup"><span data-stu-id="206b1-166">Examples</span></span>

### <a name="example-1-notify-a-user-about-a-task-created-in-a-chat"></a><span data-ttu-id="206b1-167">Пример 1. Уведомление пользователя о задаче, созданной в чате</span><span class="sxs-lookup"><span data-stu-id="206b1-167">Example 1: Notify a user about a task created in a chat</span></span>

<span data-ttu-id="206b1-168">В этом примере показано, как можно отправить уведомление о ленте действий для новой задачи, созданной в чате.</span><span class="sxs-lookup"><span data-stu-id="206b1-168">This example shows how you can send an activity feed notification for a new task created in a chat.</span></span> <span data-ttu-id="206b1-169">Дополнительные сведения см. [в Teams уведомлений об активности.](/graph/teams-send-activityfeednotifications)</span><span class="sxs-lookup"><span data-stu-id="206b1-169">For more details, see [sending Teams activity notifications](/graph/teams-send-activityfeednotifications).</span></span>

#### <a name="request"></a><span data-ttu-id="206b1-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="206b1-170">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="206b1-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="206b1-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chat_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/chats/{chatId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/v1.0/chats/{chatId}"
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
# <a name="c"></a>[<span data-ttu-id="206b1-172">C#</span><span class="sxs-lookup"><span data-stu-id="206b1-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chat-sendactivitynotification-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="206b1-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="206b1-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chat-sendactivitynotification-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="206b1-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="206b1-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chat-sendactivitynotification-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="206b1-175">Java</span><span class="sxs-lookup"><span data-stu-id="206b1-175">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chat-sendactivitynotification-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="206b1-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="206b1-176">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-notify-a-user-about-an-approval-needed-in-a-chat-message"></a><span data-ttu-id="206b1-177">Пример 2. Уведомление пользователя об утверждении, необходимом в сообщении чата</span><span class="sxs-lookup"><span data-stu-id="206b1-177">Example 2: Notify a user about an approval needed in a chat message</span></span>

<span data-ttu-id="206b1-178">Как и в предыдущем примере, в этом примере `entityUrl` используется `topic` для .</span><span class="sxs-lookup"><span data-stu-id="206b1-178">Similar to the previous example, this example uses `entityUrl` for the `topic`.</span></span> <span data-ttu-id="206b1-179">Однако в этом случае он связывается с сообщением в чате.</span><span class="sxs-lookup"><span data-stu-id="206b1-179">However, in this case, it links to a message in the chat.</span></span> <span data-ttu-id="206b1-180">В сообщении может содержаться карточка с кнопкой утверждения.</span><span class="sxs-lookup"><span data-stu-id="206b1-180">The message can contain a card with the approval button on it.</span></span>

#### <a name="request"></a><span data-ttu-id="206b1-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="206b1-181">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "chat_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/chats/{chatId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/v1.0/chats/{chatId}/messages/{messageId}"
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

#### <a name="response"></a><span data-ttu-id="206b1-182">Ответ</span><span class="sxs-lookup"><span data-stu-id="206b1-182">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-3-notify-a-user-about-an-event-in-relation-to-a-chat"></a><span data-ttu-id="206b1-183">Пример 3. Уведомление пользователя о событии по отношению к чату</span><span class="sxs-lookup"><span data-stu-id="206b1-183">Example 3: Notify a user about an event in relation to a chat</span></span>

<span data-ttu-id="206b1-184">Как показано в предыдущих примерах, вы можете связаться с различными аспектами чата.</span><span class="sxs-lookup"><span data-stu-id="206b1-184">As shown in the previous examples, you can link to different aspects of the chat.</span></span> <span data-ttu-id="206b1-185">Однако, если вы хотите связаться с аспектом, который не является частью чата или не представлен Microsoft Graph, вы можете установить источник и передать в настраиваемом значении для `topic` `text` него.</span><span class="sxs-lookup"><span data-stu-id="206b1-185">However, if you want to link to an aspect that is not part of the chat, or is not represented by Microsoft Graph, you can set the source of the `topic` to `text` and pass in a custom value for it.</span></span> <span data-ttu-id="206b1-186">Кроме того, `webUrl` требуется при настройке `topic` источника для `text` .</span><span class="sxs-lookup"><span data-stu-id="206b1-186">Also, `webUrl` is required when setting `topic` source to `text`.</span></span>

#### <a name="request"></a><span data-ttu-id="206b1-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="206b1-187">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "chat_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/chats/{chatId}/sendActivityNotification
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

#### <a name="response"></a><span data-ttu-id="206b1-188">Ответ</span><span class="sxs-lookup"><span data-stu-id="206b1-188">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```
## <a name="see-also"></a><span data-ttu-id="206b1-189">См. также</span><span class="sxs-lookup"><span data-stu-id="206b1-189">See also</span></span>

[<span data-ttu-id="206b1-190">Извещать образец приложения C# каналов</span><span class="sxs-lookup"><span data-stu-id="206b1-190">Notify Feed App C# sample</span></span>](https://github.com/OfficeDev/Microsoft-Teams-Samples/tree/main/samples/graph-activity-feed/csharp)
