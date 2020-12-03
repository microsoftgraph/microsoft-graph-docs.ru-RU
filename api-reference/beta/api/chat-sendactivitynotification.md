---
title: 'чат: Сендактивитинотификатион'
description: Отправка уведомления о канале активности в области разговора.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 76598572ebca1421770de5a298f46fdedc30a0c9
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522001"
---
# <a name="chat-sendactivitynotification"></a><span data-ttu-id="03d14-103">чат: Сендактивитинотификатион</span><span class="sxs-lookup"><span data-stu-id="03d14-103">chat: sendActivityNotification</span></span>
<span data-ttu-id="03d14-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03d14-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="03d14-105">Отправка уведомления о канале активности в области разговора.</span><span class="sxs-lookup"><span data-stu-id="03d14-105">Send an activity feed notification in scope of a chat.</span></span> <span data-ttu-id="03d14-106">Дополнительные сведения об отправке уведомлений и требованиях для этого можно найти в разделе [Отправка уведомлений о действиях в группах](/graph/teams-send-activityfeednotifications).</span><span class="sxs-lookup"><span data-stu-id="03d14-106">For more details about sending notifications and the requirements for doing so, see [sending Teams activity notifications](/graph/teams-send-activityfeednotifications).</span></span>

## <a name="permissions"></a><span data-ttu-id="03d14-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="03d14-107">Permissions</span></span>
<span data-ttu-id="03d14-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03d14-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03d14-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03d14-110">Permission type</span></span>|<span data-ttu-id="03d14-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="03d14-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03d14-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03d14-112">Delegated (work or school account)</span></span>|<span data-ttu-id="03d14-113">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="03d14-113">TeamsActivity.Send</span></span>|
|<span data-ttu-id="03d14-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03d14-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03d14-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03d14-115">Not Supported.</span></span>|
|<span data-ttu-id="03d14-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="03d14-116">Application</span></span>|<span data-ttu-id="03d14-117">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="03d14-117">TeamsActivity.Send</span></span>|

## <a name="http-request"></a><span data-ttu-id="03d14-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03d14-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /chats/{chatId}/sendActivityNotification
```

## <a name="request-headers"></a><span data-ttu-id="03d14-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="03d14-119">Request headers</span></span>
|<span data-ttu-id="03d14-120">Имя</span><span class="sxs-lookup"><span data-stu-id="03d14-120">Name</span></span>|<span data-ttu-id="03d14-121">Описание</span><span class="sxs-lookup"><span data-stu-id="03d14-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="03d14-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="03d14-122">Authorization</span></span>|<span data-ttu-id="03d14-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03d14-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="03d14-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="03d14-125">Content-Type</span></span>|<span data-ttu-id="03d14-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03d14-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="03d14-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="03d14-128">Request body</span></span>
<span data-ttu-id="03d14-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="03d14-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="03d14-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="03d14-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="03d14-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="03d14-131">Parameter</span></span>|<span data-ttu-id="03d14-132">Тип</span><span class="sxs-lookup"><span data-stu-id="03d14-132">Type</span></span>|<span data-ttu-id="03d14-133">Описание</span><span class="sxs-lookup"><span data-stu-id="03d14-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03d14-134">topic</span><span class="sxs-lookup"><span data-stu-id="03d14-134">topic</span></span>|[<span data-ttu-id="03d14-135">теамворкактивититопик</span><span class="sxs-lookup"><span data-stu-id="03d14-135">teamworkActivityTopic</span></span>](../resources/teamworkactivitytopic.md)|<span data-ttu-id="03d14-136">Тема уведомления.</span><span class="sxs-lookup"><span data-stu-id="03d14-136">Topic of the notification.</span></span> <span data-ttu-id="03d14-137">Указывает ресурс, о котором идет речь.</span><span class="sxs-lookup"><span data-stu-id="03d14-137">Specifies the resource being talked about.</span></span>|
|<span data-ttu-id="03d14-138">activityType</span><span class="sxs-lookup"><span data-stu-id="03d14-138">activityType</span></span>|<span data-ttu-id="03d14-139">String</span><span class="sxs-lookup"><span data-stu-id="03d14-139">String</span></span>|<span data-ttu-id="03d14-140">Тип действия.</span><span class="sxs-lookup"><span data-stu-id="03d14-140">Activity type.</span></span> <span data-ttu-id="03d14-141">Он должен быть объявлен в [манифесте приложения Teams](/microsoftteams/platform/overview).</span><span class="sxs-lookup"><span data-stu-id="03d14-141">This must be declared in the [Teams app manifest](/microsoftteams/platform/overview).</span></span>|
|<span data-ttu-id="03d14-142">чаинид</span><span class="sxs-lookup"><span data-stu-id="03d14-142">chainId</span></span>|<span data-ttu-id="03d14-143">Int64</span><span class="sxs-lookup"><span data-stu-id="03d14-143">Int64</span></span>|<span data-ttu-id="03d14-144">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="03d14-144">Optional.</span></span> <span data-ttu-id="03d14-145">Используется для переопределения предыдущего уведомления.</span><span class="sxs-lookup"><span data-stu-id="03d14-145">Used to override a previous notification.</span></span> <span data-ttu-id="03d14-146">Используйте одно и то же `chainId` в последующих запросах для переопределения предыдущего уведомления.</span><span class="sxs-lookup"><span data-stu-id="03d14-146">Use the same `chainId` in subsequent requests to override the previous notification.</span></span>|
|<span data-ttu-id="03d14-147">previewText</span><span class="sxs-lookup"><span data-stu-id="03d14-147">previewText</span></span>|[<span data-ttu-id="03d14-148">itemBody</span><span class="sxs-lookup"><span data-stu-id="03d14-148">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="03d14-149">Предварительный просмотр текста уведомления.</span><span class="sxs-lookup"><span data-stu-id="03d14-149">Preview text for the notification.</span></span> <span data-ttu-id="03d14-150">Microsoft Teams будет показывать только первые 150 символов.</span><span class="sxs-lookup"><span data-stu-id="03d14-150">Microsoft Teams will only show first 150 characters.</span></span>|
|<span data-ttu-id="03d14-151">темплатепараметерс</span><span class="sxs-lookup"><span data-stu-id="03d14-151">templateParameters</span></span>|<span data-ttu-id="03d14-152">Коллекция [keyValuePair](../resources/keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="03d14-152">[keyValuePair](../resources/keyvaluepair.md) collection</span></span>|<span data-ttu-id="03d14-153">Значения для переменных шаблона, определенных в записи веб-канала активности, соответствующей `activityType` [манифесту приложения Teams](/microsoftteams/platform/overview).</span><span class="sxs-lookup"><span data-stu-id="03d14-153">Values for template variables defined in the activity feed entry corresponding to `activityType` in [Teams app manifest](/microsoftteams/platform/overview).</span></span>|
|<span data-ttu-id="03d14-154">получатель;</span><span class="sxs-lookup"><span data-stu-id="03d14-154">recipient</span></span>|[<span data-ttu-id="03d14-155">теамворкнотификатионреЦипиент</span><span class="sxs-lookup"><span data-stu-id="03d14-155">teamworkNotificationRecipient</span></span>](../resources/teamworknotificationrecipient.md)|<span data-ttu-id="03d14-156">Получатель уведомления.</span><span class="sxs-lookup"><span data-stu-id="03d14-156">Recipient of the notification.</span></span> <span data-ttu-id="03d14-157">Поддерживаются только пользователи Azure AD.</span><span class="sxs-lookup"><span data-stu-id="03d14-157">Only Azure AD users are supported.</span></span> <span data-ttu-id="03d14-158">См. также [аадусернотификатионреЦипиент](../resources/aadusernotificationrecipient.md).</span><span class="sxs-lookup"><span data-stu-id="03d14-158">See also [aadUserNotificationRecipient](../resources/aadusernotificationrecipient.md).</span></span> |

<span data-ttu-id="03d14-159">Следующие ресурсы поддерживаются при задании `source` значения свойства **Topic** `entityURL` следующим образом:</span><span class="sxs-lookup"><span data-stu-id="03d14-159">The following resources are supported when setting the `source` value of the **topic** property to `entityURL`:</span></span>

- [<span data-ttu-id="03d14-160">chat</span><span class="sxs-lookup"><span data-stu-id="03d14-160">chat</span></span>](../resources/chat.md)
- [<span data-ttu-id="03d14-161">chatMessage</span><span class="sxs-lookup"><span data-stu-id="03d14-161">chatMessage</span></span>](../resources/chatmessage.md)

> <span data-ttu-id="03d14-162">**Примечание:** URL-адрес сущности должен быть таким же, как или дочерний ресурс чата в URL-адресе.</span><span class="sxs-lookup"><span data-stu-id="03d14-162">**Note:** The entity URL must be the same as or a child resource of the chat in the URL.</span></span> <span data-ttu-id="03d14-163">Кроме того, [приложение Teams](/microsoftteams/platform/overview) должно быть установлено в чате.</span><span class="sxs-lookup"><span data-stu-id="03d14-163">Additionally, the [Teams app](/microsoftteams/platform/overview) must be installed in the chat.</span></span>

## <a name="response"></a><span data-ttu-id="03d14-164">Ответ</span><span class="sxs-lookup"><span data-stu-id="03d14-164">Response</span></span>

<span data-ttu-id="03d14-165">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="03d14-165">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="03d14-166">Примеры</span><span class="sxs-lookup"><span data-stu-id="03d14-166">Examples</span></span>

### <a name="example-1-notify-a-user-about-a-task-created-in-a-chat"></a><span data-ttu-id="03d14-167">Пример 1: уведомление пользователя о задаче, созданной в чате</span><span class="sxs-lookup"><span data-stu-id="03d14-167">Example 1: Notify a user about a task created in a chat</span></span>

<span data-ttu-id="03d14-168">В этом примере показано, как можно отправить уведомление веб-канала активности для новой задачи, созданной в чате.</span><span class="sxs-lookup"><span data-stu-id="03d14-168">This example shows how you can send an activity feed notification for a new task created in a chat.</span></span> <span data-ttu-id="03d14-169">Более подробную информацию можно узнать в статье [Отправка уведомлений о действиях в группах](/graph/teams-send-activityfeednotifications).</span><span class="sxs-lookup"><span data-stu-id="03d14-169">For more details, see [sending Teams activity notifications](/graph/teams-send-activityfeednotifications).</span></span>

#### <a name="request"></a><span data-ttu-id="03d14-170">Запрос</span><span class="sxs-lookup"><span data-stu-id="03d14-170">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="03d14-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="03d14-171">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="03d14-172">C#</span><span class="sxs-lookup"><span data-stu-id="03d14-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chat-sendactivitynotification-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="03d14-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="03d14-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chat-sendactivitynotification-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="03d14-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="03d14-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chat-sendactivitynotification-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="03d14-175">Java</span><span class="sxs-lookup"><span data-stu-id="03d14-175">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chat-sendactivitynotification-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="03d14-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="03d14-176">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-notify-a-user-about-a-approval-needed-in-a-chat-message"></a><span data-ttu-id="03d14-177">Пример 2: уведомление пользователя о необходимости утверждения в сообщении чата</span><span class="sxs-lookup"><span data-stu-id="03d14-177">Example 2: Notify a user about a approval needed in a chat message</span></span>

<span data-ttu-id="03d14-178">Как и в предыдущем примере, в этом примере используется `entityUrl` для `topic` .</span><span class="sxs-lookup"><span data-stu-id="03d14-178">Similar to the previous example, this example uses `entityUrl` for the `topic`.</span></span> <span data-ttu-id="03d14-179">Однако в этом случае он связывается с сообщением в чате.</span><span class="sxs-lookup"><span data-stu-id="03d14-179">However, in this case, it links to a message in the chat.</span></span> <span data-ttu-id="03d14-180">Сообщение может содержать карточку с кнопкой утверждения на ней.</span><span class="sxs-lookup"><span data-stu-id="03d14-180">The message can contains a card with the approval button on it.</span></span>

#### <a name="request"></a><span data-ttu-id="03d14-181">Запрос</span><span class="sxs-lookup"><span data-stu-id="03d14-181">Request</span></span>
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

#### <a name="response"></a><span data-ttu-id="03d14-182">Отклик</span><span class="sxs-lookup"><span data-stu-id="03d14-182">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-3-notify-a-user-about-an-event-in-relation-to-a-chat"></a><span data-ttu-id="03d14-183">Пример 3: уведомление пользователя о событии относительно чата</span><span class="sxs-lookup"><span data-stu-id="03d14-183">Example 3: Notify a user about an event in relation to a chat</span></span>

<span data-ttu-id="03d14-184">Как показано в предыдущих примерах, вы можете ссылаться на различные аспекты разговора.</span><span class="sxs-lookup"><span data-stu-id="03d14-184">As shown in the previous examples, you can link to different aspects of the chat.</span></span> <span data-ttu-id="03d14-185">Тем не менее, если вы хотите создать ссылку на аспект, не входящий в чат или не представленный в Microsoft Graph, можно установить для него в качестве источника `topic` `text` значение и передать его настраиваемое значение.</span><span class="sxs-lookup"><span data-stu-id="03d14-185">However, if you want to link to an aspect that is not part of the chat, or is not represented by Microsoft Graph, you can set the source of the `topic` to `text` and pass in a custom value for it.</span></span> <span data-ttu-id="03d14-186">Кроме того, `webUrl` требуется, если для параметра Source задано значение `topic` `text` .</span><span class="sxs-lookup"><span data-stu-id="03d14-186">Also, `webUrl` is required when setting `topic` source to `text`.</span></span>

#### <a name="request"></a><span data-ttu-id="03d14-187">Запрос</span><span class="sxs-lookup"><span data-stu-id="03d14-187">Request</span></span>
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

#### <a name="response"></a><span data-ttu-id="03d14-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="03d14-188">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```
