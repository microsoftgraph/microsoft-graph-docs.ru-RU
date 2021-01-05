---
title: 'team: sendActivityNotification'
description: Отправка уведомления веб-канала активности в области команды.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f4ad396d25ee20bd4adc5bf579925bbd4e8de1fd
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/05/2021
ms.locfileid: "49754063"
---
# <a name="team-sendactivitynotification"></a><span data-ttu-id="47032-103">team: sendActivityNotification</span><span class="sxs-lookup"><span data-stu-id="47032-103">team: sendActivityNotification</span></span>
<span data-ttu-id="47032-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47032-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="47032-105">Отправка уведомления веб-канала активности в области команды.</span><span class="sxs-lookup"><span data-stu-id="47032-105">Send an activity feed notification in the scope of a team.</span></span> <span data-ttu-id="47032-106">Дополнительные сведения об отправке уведомлений и требованиях для этого см. в отправке уведомлений [о действиях Teams.](/graph/teams-send-activityfeednotifications)</span><span class="sxs-lookup"><span data-stu-id="47032-106">For more details about sending notifications and the requirements for doing so, see [sending Teams activity notifications](/graph/teams-send-activityfeednotifications).</span></span>

## <a name="permissions"></a><span data-ttu-id="47032-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="47032-107">Permissions</span></span>
<span data-ttu-id="47032-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47032-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47032-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47032-110">Permission type</span></span>|<span data-ttu-id="47032-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="47032-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47032-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47032-112">Delegated (work or school account)</span></span>|<span data-ttu-id="47032-113">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="47032-113">TeamsActivity.Send</span></span>|
|<span data-ttu-id="47032-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47032-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47032-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47032-115">Not Supported.</span></span>|
|<span data-ttu-id="47032-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="47032-116">Application</span></span>|<span data-ttu-id="47032-117">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="47032-117">TeamsActivity.Send</span></span>|

## <a name="http-request"></a><span data-ttu-id="47032-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47032-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /teams/{teamId}/sendActivityNotification
```

## <a name="request-headers"></a><span data-ttu-id="47032-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="47032-119">Request headers</span></span>
|<span data-ttu-id="47032-120">Имя</span><span class="sxs-lookup"><span data-stu-id="47032-120">Name</span></span>|<span data-ttu-id="47032-121">Описание</span><span class="sxs-lookup"><span data-stu-id="47032-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="47032-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="47032-122">Authorization</span></span>|<span data-ttu-id="47032-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="47032-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="47032-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="47032-125">Content-Type</span></span>|<span data-ttu-id="47032-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="47032-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="47032-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="47032-128">Request body</span></span>
<span data-ttu-id="47032-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="47032-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="47032-130">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="47032-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="47032-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="47032-131">Parameter</span></span>|<span data-ttu-id="47032-132">Тип</span><span class="sxs-lookup"><span data-stu-id="47032-132">Type</span></span>|<span data-ttu-id="47032-133">Описание</span><span class="sxs-lookup"><span data-stu-id="47032-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47032-134">topic</span><span class="sxs-lookup"><span data-stu-id="47032-134">topic</span></span>|[<span data-ttu-id="47032-135">teamworkActivityTopic</span><span class="sxs-lookup"><span data-stu-id="47032-135">teamworkActivityTopic</span></span>](../resources/teamworkactivitytopic.md)|<span data-ttu-id="47032-136">Тема уведомления.</span><span class="sxs-lookup"><span data-stu-id="47032-136">Topic of the notification.</span></span> <span data-ttu-id="47032-137">Указывает ресурс, о который идет речь.</span><span class="sxs-lookup"><span data-stu-id="47032-137">Specifies the resource being talked about.</span></span>|
|<span data-ttu-id="47032-138">activityType</span><span class="sxs-lookup"><span data-stu-id="47032-138">activityType</span></span>|<span data-ttu-id="47032-139">String</span><span class="sxs-lookup"><span data-stu-id="47032-139">String</span></span>|<span data-ttu-id="47032-140">Тип действия.</span><span class="sxs-lookup"><span data-stu-id="47032-140">Activity type.</span></span> <span data-ttu-id="47032-141">Это должно быть объявлено в манифесте [приложения Teams.](/microsoftteams/platform/overview)</span><span class="sxs-lookup"><span data-stu-id="47032-141">This must be declared in the [Teams app manifest](/microsoftteams/platform/overview).</span></span>|
|<span data-ttu-id="47032-142">chainId</span><span class="sxs-lookup"><span data-stu-id="47032-142">chainId</span></span>|<span data-ttu-id="47032-143">Int64</span><span class="sxs-lookup"><span data-stu-id="47032-143">Int64</span></span>|<span data-ttu-id="47032-144">Необязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="47032-144">Optional.</span></span> <span data-ttu-id="47032-145">Используется для переопределения предыдущего уведомления.</span><span class="sxs-lookup"><span data-stu-id="47032-145">Used to override a previous notification.</span></span> <span data-ttu-id="47032-146">Используйте то же самое `chainId` в последующих запросах для переопределения предыдущего уведомления.</span><span class="sxs-lookup"><span data-stu-id="47032-146">Use the same `chainId` in subsequent requests to override the previous notification.</span></span>|
|<span data-ttu-id="47032-147">previewText</span><span class="sxs-lookup"><span data-stu-id="47032-147">previewText</span></span>|[<span data-ttu-id="47032-148">itemBody</span><span class="sxs-lookup"><span data-stu-id="47032-148">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="47032-149">Предварительный просмотр текста уведомления.</span><span class="sxs-lookup"><span data-stu-id="47032-149">Preview text for the notification.</span></span> <span data-ttu-id="47032-150">Microsoft Teams будет показывать только первые 150 символов.</span><span class="sxs-lookup"><span data-stu-id="47032-150">Microsoft Teams will only show first 150 characters.</span></span>|
|<span data-ttu-id="47032-151">templateParameters</span><span class="sxs-lookup"><span data-stu-id="47032-151">templateParameters</span></span>|<span data-ttu-id="47032-152">Коллекция [keyValuePair](../resources/keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="47032-152">[keyValuePair](../resources/keyvaluepair.md) collection</span></span>|<span data-ttu-id="47032-153">Значения переменных шаблона, определенных в записи веб-канала активности, соответствующей `activityType` [манифесту приложения Teams.](/microsoftteams/platform/overview)</span><span class="sxs-lookup"><span data-stu-id="47032-153">Values for template variables defined in the activity feed entry corresponding to `activityType` in [Teams app manifest](/microsoftteams/platform/overview).</span></span>|
|<span data-ttu-id="47032-154">получатель;</span><span class="sxs-lookup"><span data-stu-id="47032-154">recipient</span></span>|[<span data-ttu-id="47032-155">teamworkNotificationRecipient</span><span class="sxs-lookup"><span data-stu-id="47032-155">teamworkNotificationRecipient</span></span>](../resources/teamworknotificationrecipient.md)|<span data-ttu-id="47032-156">Получатель уведомления.</span><span class="sxs-lookup"><span data-stu-id="47032-156">Recipient of the notification.</span></span> <span data-ttu-id="47032-157">Поддерживаются только пользователи Azure AD.</span><span class="sxs-lookup"><span data-stu-id="47032-157">Only Azure AD users are supported.</span></span> <span data-ttu-id="47032-158">См. [также aadUserNotificationRecipient.](../resources/aadusernotificationrecipient.md)</span><span class="sxs-lookup"><span data-stu-id="47032-158">See also [aadUserNotificationRecipient](../resources/aadusernotificationrecipient.md).</span></span> |

<span data-ttu-id="47032-159">Следующие ресурсы поддерживаются при установке для свойства `source` **темы** значения `entityUrl` :</span><span class="sxs-lookup"><span data-stu-id="47032-159">The following resources are supported when setting the `source` value of the **topic** property to `entityUrl`:</span></span>

- [<span data-ttu-id="47032-160">team</span><span class="sxs-lookup"><span data-stu-id="47032-160">team</span></span>](../resources/team.md)
- [<span data-ttu-id="47032-161">channel</span><span class="sxs-lookup"><span data-stu-id="47032-161">channel</span></span>](../resources/channel.md)
- [<span data-ttu-id="47032-162">chatMesage</span><span class="sxs-lookup"><span data-stu-id="47032-162">chatMesage</span></span>](../resources/chatmessage.md)
- [<span data-ttu-id="47032-163">teamsTab</span><span class="sxs-lookup"><span data-stu-id="47032-163">teamsTab</span></span>](../resources/teamstab.md)

> <span data-ttu-id="47032-164">**Примечание.** URL-адрес сущности должен быть тем же или иным ресурсом команды в URL-адресе.</span><span class="sxs-lookup"><span data-stu-id="47032-164">**Note:** The entity url must be same or child resource of the team in the url.</span></span> <span data-ttu-id="47032-165">Кроме того, приложение [Teams](/microsoftteams/platform/overview) должно быть установлено в команде.</span><span class="sxs-lookup"><span data-stu-id="47032-165">Additionally, the [Teams app](/microsoftteams/platform/overview) must be installed in the team.</span></span>

## <a name="response"></a><span data-ttu-id="47032-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="47032-166">Response</span></span>

<span data-ttu-id="47032-167">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="47032-167">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="47032-168">Примеры</span><span class="sxs-lookup"><span data-stu-id="47032-168">Examples</span></span>

### <a name="example-1-notify-a-user-about-pending-finance-approval-requests"></a><span data-ttu-id="47032-169">Пример 1. Уведомление пользователя об ожидающих запросах на финансовое утверждение</span><span class="sxs-lookup"><span data-stu-id="47032-169">Example 1: Notify a user about pending finance approval requests</span></span>

<span data-ttu-id="47032-170">В этом примере показано, как можно отправить уведомление веб-канала активности для команды.</span><span class="sxs-lookup"><span data-stu-id="47032-170">This example shows how you can send an activity feed notification for a team.</span></span> <span data-ttu-id="47032-171">В этом примере владельцу команды сообщается об ожидающих запросах на финансовое утверждение.</span><span class="sxs-lookup"><span data-stu-id="47032-171">This example notifies the team owner about pending finance approval requests.</span></span>

#### <a name="request"></a><span data-ttu-id="47032-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="47032-172">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="47032-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="47032-173">HTTP</span></span>](#tab/http)
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
    "activityType": "pendingFinanceApprovalRequests",
    "previewText": {
        "content": "Internal spending team has a pending finance approval requests"
    },
    "recipient": {
        "@odata.type": "microsoft.graph.aadUserNotificationRecipient",
        "userId": "569363e2-4e49-4661-87f2-16f245c5d66a"
    },
    "templateParameters": [
        {
            "name": "pendingRequestCount",
            "value": "5"
        }
    ] 
}
```
# <a name="javascript"></a>[<span data-ttu-id="47032-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="47032-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/team-sendactivitynotification-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="47032-175">C#</span><span class="sxs-lookup"><span data-stu-id="47032-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/team-sendactivitynotification-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="47032-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="47032-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/team-sendactivitynotification-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="47032-177">Java</span><span class="sxs-lookup"><span data-stu-id="47032-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/team-sendactivitynotification-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="47032-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="47032-178">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-notify-a-user-about-a-channel-tab"></a><span data-ttu-id="47032-179">Пример 2. Уведомление пользователя о вкладке канала</span><span class="sxs-lookup"><span data-stu-id="47032-179">Example 2: Notify a user about a channel tab</span></span>

<span data-ttu-id="47032-180">Как и в предыдущем примере, в этом примере `entityUrl` используется для `topic` .</span><span class="sxs-lookup"><span data-stu-id="47032-180">Similar to the previous example, this example uses `entityUrl` for the `topic`.</span></span> <span data-ttu-id="47032-181">Однако в этом примере ссылки на [вкладку](../resources/teamstab.md) в [канале.](../resources/channel.md)</span><span class="sxs-lookup"><span data-stu-id="47032-181">However, this example links to a [tab](../resources/teamstab.md) in a [channel](../resources/channel.md).</span></span> <span data-ttu-id="47032-182">На вкладке размещена страница с состоянием резервирования в гостинице.</span><span class="sxs-lookup"><span data-stu-id="47032-182">The tab hosts a page showing the user the status of their hotel reservation.</span></span> <span data-ttu-id="47032-183">При выборе уведомления пользователь перенаберется на вкладку, где он сможет проверить свое резервирование.</span><span class="sxs-lookup"><span data-stu-id="47032-183">Selecting the notification will take the user to the tab, where they can check their reservation.</span></span>

#### <a name="request"></a><span data-ttu-id="47032-184">Запрос</span><span class="sxs-lookup"><span data-stu-id="47032-184">Request</span></span>
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
        "value": "https://graph.microsoft.com/beta/teams/{teamId}/channels/{channelId}/tabs/{tabId}"
    },
    "activityType": "reservationUpdated",
    "previewText": {
        "content": "You have moved up the queue"
    },
    "recipient": {
        "@odata.type": "Microsoft.Teams.GraphSvc.aadUserNotificationRecipient",
        "userId": "569363e2-4e49-4661-87f2-16f245c5d66a"
    },
    "templateParameters": [
        {
            "name": "reservationId",
            "value": "TREEE433"
        },
        {
            "name": "currentSlot",
            "value": "23"
        }
    ]
}
```

#### <a name="response"></a><span data-ttu-id="47032-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="47032-185">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-3-notify-a-user-about-an-event-using-custom-topic"></a><span data-ttu-id="47032-186">Пример 3. Уведомление пользователя о событии с помощью настраиваемой темы</span><span class="sxs-lookup"><span data-stu-id="47032-186">Example 3: Notify a user about an event using custom topic</span></span>

<span data-ttu-id="47032-187">Как видно из предыдущих примеров, вы можете ссылаться на различные аспекты команды.</span><span class="sxs-lookup"><span data-stu-id="47032-187">As seen in the previous examples, you can link to different aspects of the team.</span></span> <span data-ttu-id="47032-188">Однако если вы хотите связать аспект, который не является частью команды или не представлен Microsoft Graph, или вы хотите настроить имя, вы можете настроить источник и передать для него настраиваемые `topic` `text` значения.</span><span class="sxs-lookup"><span data-stu-id="47032-188">However, if you want to link to an aspect that is not part of the team or is not represented by Microsoft Graph, or you want to customize the name, you can set the source of the `topic` to `text` and pass in a custom value for it.</span></span> <span data-ttu-id="47032-189">`webUrl` требуется при установке `topic` для источника параметра `text` ..</span><span class="sxs-lookup"><span data-stu-id="47032-189">`webUrl` is required when setting `topic` source to `text`.</span></span>

#### <a name="request"></a><span data-ttu-id="47032-190">Запрос</span><span class="sxs-lookup"><span data-stu-id="47032-190">Request</span></span>
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

#### <a name="response"></a><span data-ttu-id="47032-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="47032-191">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```
