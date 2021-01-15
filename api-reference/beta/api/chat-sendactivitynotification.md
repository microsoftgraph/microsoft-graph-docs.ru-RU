---
title: 'chat: sendActivityNotification'
description: Отправка уведомления веб-канала активности в области чата.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7147ad0019b9c066f19f30b9829e80e1a75570ca
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872861"
---
# <a name="chat-sendactivitynotification"></a><span data-ttu-id="4155e-103">chat: sendActivityNotification</span><span class="sxs-lookup"><span data-stu-id="4155e-103">chat: sendActivityNotification</span></span>
<span data-ttu-id="4155e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4155e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4155e-105">Отправка уведомления веб-канала активности в области чата.</span><span class="sxs-lookup"><span data-stu-id="4155e-105">Send an activity feed notification in scope of a chat.</span></span> <span data-ttu-id="4155e-106">Дополнительные сведения об отправке уведомлений и требованиях для этого см. в отправке уведомлений [о действиях Teams.](/graph/teams-send-activityfeednotifications)</span><span class="sxs-lookup"><span data-stu-id="4155e-106">For more details about sending notifications and the requirements for doing so, see [sending Teams activity notifications](/graph/teams-send-activityfeednotifications).</span></span>

## <a name="permissions"></a><span data-ttu-id="4155e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4155e-107">Permissions</span></span>
<span data-ttu-id="4155e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4155e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4155e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4155e-110">Permission type</span></span>|<span data-ttu-id="4155e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4155e-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4155e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4155e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4155e-113">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="4155e-113">TeamsActivity.Send</span></span>|
|<span data-ttu-id="4155e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4155e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4155e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4155e-115">Not Supported.</span></span>|
|<span data-ttu-id="4155e-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="4155e-116">Application</span></span>|<span data-ttu-id="4155e-117">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="4155e-117">TeamsActivity.Send</span></span>|

## <a name="http-request"></a><span data-ttu-id="4155e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4155e-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /chats/{chatId}/sendActivityNotification
```

## <a name="request-headers"></a><span data-ttu-id="4155e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4155e-119">Request headers</span></span>
|<span data-ttu-id="4155e-120">Имя</span><span class="sxs-lookup"><span data-stu-id="4155e-120">Name</span></span>|<span data-ttu-id="4155e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="4155e-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4155e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4155e-122">Authorization</span></span>|<span data-ttu-id="4155e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4155e-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4155e-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4155e-125">Content-Type</span></span>|<span data-ttu-id="4155e-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4155e-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4155e-128">Основной текст запроса</span><span class="sxs-lookup"><span data-stu-id="4155e-128">Request body</span></span>
<span data-ttu-id="4155e-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4155e-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="4155e-130">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="4155e-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="4155e-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="4155e-131">Parameter</span></span>|<span data-ttu-id="4155e-132">Тип</span><span class="sxs-lookup"><span data-stu-id="4155e-132">Type</span></span>|<span data-ttu-id="4155e-133">Описание</span><span class="sxs-lookup"><span data-stu-id="4155e-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4155e-134">topic</span><span class="sxs-lookup"><span data-stu-id="4155e-134">topic</span></span>|[<span data-ttu-id="4155e-135">teamworkActivityTopic</span><span class="sxs-lookup"><span data-stu-id="4155e-135">teamworkActivityTopic</span></span>](../resources/teamworkactivitytopic.md)|<span data-ttu-id="4155e-136">Тема уведомления.</span><span class="sxs-lookup"><span data-stu-id="4155e-136">Topic of the notification.</span></span> <span data-ttu-id="4155e-137">Указывает ресурс, о который идет речь.</span><span class="sxs-lookup"><span data-stu-id="4155e-137">Specifies the resource being talked about.</span></span>|
|<span data-ttu-id="4155e-138">activityType</span><span class="sxs-lookup"><span data-stu-id="4155e-138">activityType</span></span>|<span data-ttu-id="4155e-139">String</span><span class="sxs-lookup"><span data-stu-id="4155e-139">String</span></span>|<span data-ttu-id="4155e-140">Тип действия.</span><span class="sxs-lookup"><span data-stu-id="4155e-140">Activity type.</span></span> <span data-ttu-id="4155e-141">Это должно быть объявлено в манифесте [приложения Teams.](/microsoftteams/platform/overview)</span><span class="sxs-lookup"><span data-stu-id="4155e-141">This must be declared in the [Teams app manifest](/microsoftteams/platform/overview).</span></span>|
|<span data-ttu-id="4155e-142">chainId</span><span class="sxs-lookup"><span data-stu-id="4155e-142">chainId</span></span>|<span data-ttu-id="4155e-143">Int64</span><span class="sxs-lookup"><span data-stu-id="4155e-143">Int64</span></span>|<span data-ttu-id="4155e-144">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="4155e-144">Optional.</span></span> <span data-ttu-id="4155e-145">Используется для переопределения предыдущего уведомления.</span><span class="sxs-lookup"><span data-stu-id="4155e-145">Used to override a previous notification.</span></span> <span data-ttu-id="4155e-146">Используйте то же самое `chainId` в последующих запросах для переопределения предыдущего уведомления.</span><span class="sxs-lookup"><span data-stu-id="4155e-146">Use the same `chainId` in subsequent requests to override the previous notification.</span></span>|
|<span data-ttu-id="4155e-147">previewText</span><span class="sxs-lookup"><span data-stu-id="4155e-147">previewText</span></span>|[<span data-ttu-id="4155e-148">itemBody</span><span class="sxs-lookup"><span data-stu-id="4155e-148">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="4155e-149">Предварительный просмотр текста уведомления.</span><span class="sxs-lookup"><span data-stu-id="4155e-149">Preview text for the notification.</span></span> <span data-ttu-id="4155e-150">Microsoft Teams будет показывать только первые 150 символов.</span><span class="sxs-lookup"><span data-stu-id="4155e-150">Microsoft Teams will only show first 150 characters.</span></span>|
|<span data-ttu-id="4155e-151">templateParameters</span><span class="sxs-lookup"><span data-stu-id="4155e-151">templateParameters</span></span>|<span data-ttu-id="4155e-152">Коллекция [keyValuePair](../resources/keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="4155e-152">[keyValuePair](../resources/keyvaluepair.md) collection</span></span>|<span data-ttu-id="4155e-153">Значения переменных шаблона, определенных в записи веб-канала активности, соответствующей `activityType` [манифесту приложения Teams.](/microsoftteams/platform/overview)</span><span class="sxs-lookup"><span data-stu-id="4155e-153">Values for template variables defined in the activity feed entry corresponding to `activityType` in [Teams app manifest](/microsoftteams/platform/overview).</span></span>|
|<span data-ttu-id="4155e-154">получатель;</span><span class="sxs-lookup"><span data-stu-id="4155e-154">recipient</span></span>|[<span data-ttu-id="4155e-155">teamworkNotificationRecipient</span><span class="sxs-lookup"><span data-stu-id="4155e-155">teamworkNotificationRecipient</span></span>](../resources/teamworknotificationrecipient.md)|<span data-ttu-id="4155e-156">Получатель уведомления.</span><span class="sxs-lookup"><span data-stu-id="4155e-156">Recipient of the notification.</span></span> <span data-ttu-id="4155e-157">Поддерживаются только пользователи Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4155e-157">Only Azure AD users are supported.</span></span> <span data-ttu-id="4155e-158">См. [также aadUserNotificationRecipient.](../resources/aadusernotificationrecipient.md)</span><span class="sxs-lookup"><span data-stu-id="4155e-158">See also [aadUserNotificationRecipient](../resources/aadusernotificationrecipient.md).</span></span> |

<span data-ttu-id="4155e-159">Следующие ресурсы поддерживаются при установке для свойства `source` **темы** значения `entityURL` :</span><span class="sxs-lookup"><span data-stu-id="4155e-159">The following resources are supported when setting the `source` value of the **topic** property to `entityURL`:</span></span>

- [<span data-ttu-id="4155e-160">chat</span><span class="sxs-lookup"><span data-stu-id="4155e-160">chat</span></span>](../resources/chat.md)
- [<span data-ttu-id="4155e-161">chatMessage</span><span class="sxs-lookup"><span data-stu-id="4155e-161">chatMessage</span></span>](../resources/chatmessage.md)

> <span data-ttu-id="4155e-162">**Примечание.** URL-адрес сущности должен быть таким же, как или его дитя в чате в URL-адресе.</span><span class="sxs-lookup"><span data-stu-id="4155e-162">**Note:** The entity URL must be the same as or a child resource of the chat in the URL.</span></span> <span data-ttu-id="4155e-163">Кроме того, приложение [Teams должно](/microsoftteams/platform/overview) быть установлено в чате.</span><span class="sxs-lookup"><span data-stu-id="4155e-163">Additionally, the [Teams app](/microsoftteams/platform/overview) must be installed in the chat.</span></span>

## <a name="response"></a><span data-ttu-id="4155e-164">Ответ</span><span class="sxs-lookup"><span data-stu-id="4155e-164">Response</span></span>

<span data-ttu-id="4155e-165">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4155e-165">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="4155e-166">Примеры</span><span class="sxs-lookup"><span data-stu-id="4155e-166">Examples</span></span>

### <a name="example-1-notify-a-user-about-a-task-created-in-a-chat"></a><span data-ttu-id="4155e-167">Пример 1. Уведомление пользователя о задаче, созданной в чате</span><span class="sxs-lookup"><span data-stu-id="4155e-167">Example 1: Notify a user about a task created in a chat</span></span>

<span data-ttu-id="4155e-168">В этом примере показано, как можно отправить уведомление веб-канала активности для новой задачи, созданной в чате.</span><span class="sxs-lookup"><span data-stu-id="4155e-168">This example shows how you can send an activity feed notification for a new task created in a chat.</span></span> <span data-ttu-id="4155e-169">Дополнительные сведения [см. в отправке уведомлений об активности Teams.](/graph/teams-send-activityfeednotifications)</span><span class="sxs-lookup"><span data-stu-id="4155e-169">For more details, see [sending Teams activity notifications](/graph/teams-send-activityfeednotifications).</span></span>

#### <a name="request"></a><span data-ttu-id="4155e-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="4155e-170">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="4155e-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="4155e-171">HTTP</span></span>](#tab/http)
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
            "value": "Task 12322"
        }
    ] 
}
```
# <a name="c"></a>[<span data-ttu-id="4155e-172">C#</span><span class="sxs-lookup"><span data-stu-id="4155e-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chat-sendactivitynotification-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4155e-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4155e-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chat-sendactivitynotification-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4155e-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4155e-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chat-sendactivitynotification-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4155e-175">Java</span><span class="sxs-lookup"><span data-stu-id="4155e-175">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chat-sendactivitynotification-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4155e-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="4155e-176">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-notify-a-user-about-a-approval-needed-in-a-chat-message"></a><span data-ttu-id="4155e-177">Пример 2. Уведомление пользователя об утверждении, необходимом в сообщении чата</span><span class="sxs-lookup"><span data-stu-id="4155e-177">Example 2: Notify a user about a approval needed in a chat message</span></span>

<span data-ttu-id="4155e-178">Как и в предыдущем примере, в этом примере `entityUrl` используется для `topic` .</span><span class="sxs-lookup"><span data-stu-id="4155e-178">Similar to the previous example, this example uses `entityUrl` for the `topic`.</span></span> <span data-ttu-id="4155e-179">Однако в этом случае он ссылайтесь на сообщение в чате.</span><span class="sxs-lookup"><span data-stu-id="4155e-179">However, in this case, it links to a message in the chat.</span></span> <span data-ttu-id="4155e-180">Сообщение может содержит карточку с кнопкой утверждения.</span><span class="sxs-lookup"><span data-stu-id="4155e-180">The message can contains a card with the approval button on it.</span></span>

#### <a name="request"></a><span data-ttu-id="4155e-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="4155e-181">Request</span></span>
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

#### <a name="response"></a><span data-ttu-id="4155e-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="4155e-182">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-3-notify-a-user-about-an-event-in-relation-to-a-chat"></a><span data-ttu-id="4155e-183">Пример 3. Уведомление пользователя о событии по отношению к чату</span><span class="sxs-lookup"><span data-stu-id="4155e-183">Example 3: Notify a user about an event in relation to a chat</span></span>

<span data-ttu-id="4155e-184">Как показано в предыдущих примерах, вы можете ссылаться на различные аспекты чата.</span><span class="sxs-lookup"><span data-stu-id="4155e-184">As shown in the previous examples, you can link to different aspects of the chat.</span></span> <span data-ttu-id="4155e-185">Однако если вы хотите связать аспект, который не является частью чата или не представлен Microsoft Graph, вы можете установить источник и передать для него пользовательское `topic` `text` значение.</span><span class="sxs-lookup"><span data-stu-id="4155e-185">However, if you want to link to an aspect that is not part of the chat, or is not represented by Microsoft Graph, you can set the source of the `topic` to `text` and pass in a custom value for it.</span></span> <span data-ttu-id="4155e-186">Кроме того, `webUrl` требуется при установке `topic` для источника параметра `text` ..</span><span class="sxs-lookup"><span data-stu-id="4155e-186">Also, `webUrl` is required when setting `topic` source to `text`.</span></span>

#### <a name="request"></a><span data-ttu-id="4155e-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="4155e-187">Request</span></span>
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

#### <a name="response"></a><span data-ttu-id="4155e-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="4155e-188">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```
