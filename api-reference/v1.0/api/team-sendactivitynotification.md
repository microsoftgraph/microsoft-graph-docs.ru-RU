---
title: 'команда: sendActivityNotification'
description: Отправьте уведомление о канале действий в области группы.
author: eddie-lee-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: add05d086580d5ed76b4195de98d28187e3ad30d
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507573"
---
# <a name="team-sendactivitynotification"></a><span data-ttu-id="4ce93-103">команда: sendActivityNotification</span><span class="sxs-lookup"><span data-stu-id="4ce93-103">team: sendActivityNotification</span></span>
<span data-ttu-id="4ce93-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ce93-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4ce93-105">Отправьте уведомление о канале действий в области группы.</span><span class="sxs-lookup"><span data-stu-id="4ce93-105">Send an activity feed notification in the scope of a team.</span></span> <span data-ttu-id="4ce93-106">Дополнительные сведения об отправке уведомлений и требованиях к этому см. в материале Отправка уведомлений о [действиях Teams.](/graph/teams-send-activityfeednotifications)</span><span class="sxs-lookup"><span data-stu-id="4ce93-106">For more details about sending notifications and the requirements for doing so, see [sending Teams activity notifications](/graph/teams-send-activityfeednotifications).</span></span>

## <a name="permissions"></a><span data-ttu-id="4ce93-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4ce93-107">Permissions</span></span>
<span data-ttu-id="4ce93-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ce93-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ce93-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4ce93-110">Permission type</span></span>|<span data-ttu-id="4ce93-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4ce93-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ce93-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4ce93-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4ce93-113">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="4ce93-113">TeamsActivity.Send</span></span>|
|<span data-ttu-id="4ce93-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4ce93-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ce93-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4ce93-115">Not Supported.</span></span>|
|<span data-ttu-id="4ce93-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4ce93-116">Application</span></span>|<span data-ttu-id="4ce93-117">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="4ce93-117">TeamsActivity.Send</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ce93-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4ce93-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /teams/{teamId}/sendActivityNotification
```

## <a name="request-headers"></a><span data-ttu-id="4ce93-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4ce93-119">Request headers</span></span>
|<span data-ttu-id="4ce93-120">Имя</span><span class="sxs-lookup"><span data-stu-id="4ce93-120">Name</span></span>|<span data-ttu-id="4ce93-121">Описание</span><span class="sxs-lookup"><span data-stu-id="4ce93-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4ce93-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4ce93-122">Authorization</span></span>|<span data-ttu-id="4ce93-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4ce93-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4ce93-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4ce93-125">Content-Type</span></span>|<span data-ttu-id="4ce93-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4ce93-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ce93-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4ce93-128">Request body</span></span>
<span data-ttu-id="4ce93-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4ce93-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="4ce93-130">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="4ce93-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="4ce93-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="4ce93-131">Parameter</span></span>|<span data-ttu-id="4ce93-132">Тип</span><span class="sxs-lookup"><span data-stu-id="4ce93-132">Type</span></span>|<span data-ttu-id="4ce93-133">Описание</span><span class="sxs-lookup"><span data-stu-id="4ce93-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ce93-134">topic</span><span class="sxs-lookup"><span data-stu-id="4ce93-134">topic</span></span>|[<span data-ttu-id="4ce93-135">teamworkActivityTopic</span><span class="sxs-lookup"><span data-stu-id="4ce93-135">teamworkActivityTopic</span></span>](../resources/teamworkactivitytopic.md)|<span data-ttu-id="4ce93-136">Тема уведомления.</span><span class="sxs-lookup"><span data-stu-id="4ce93-136">Topic of the notification.</span></span> <span data-ttu-id="4ce93-137">Указывает обсуждаемый ресурс.</span><span class="sxs-lookup"><span data-stu-id="4ce93-137">Specifies the resource being talked about.</span></span>|
|<span data-ttu-id="4ce93-138">activityType</span><span class="sxs-lookup"><span data-stu-id="4ce93-138">activityType</span></span>|<span data-ttu-id="4ce93-139">String</span><span class="sxs-lookup"><span data-stu-id="4ce93-139">String</span></span>|<span data-ttu-id="4ce93-140">Тип действия.</span><span class="sxs-lookup"><span data-stu-id="4ce93-140">Activity type.</span></span> <span data-ttu-id="4ce93-141">Это должно быть объявлено в [манифесте приложения Teams.](/microsoftteams/platform/overview)</span><span class="sxs-lookup"><span data-stu-id="4ce93-141">This must be declared in the [Teams app manifest](/microsoftteams/platform/overview).</span></span>|
|<span data-ttu-id="4ce93-142">chainId</span><span class="sxs-lookup"><span data-stu-id="4ce93-142">chainId</span></span>|<span data-ttu-id="4ce93-143">Int64</span><span class="sxs-lookup"><span data-stu-id="4ce93-143">Int64</span></span>|<span data-ttu-id="4ce93-144">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="4ce93-144">Optional.</span></span> <span data-ttu-id="4ce93-145">Используется для переопределения предыдущего уведомления.</span><span class="sxs-lookup"><span data-stu-id="4ce93-145">Used to override a previous notification.</span></span> <span data-ttu-id="4ce93-146">Используйте то же `chainId` самое в последующих запросах для переопределения предыдущего уведомления.</span><span class="sxs-lookup"><span data-stu-id="4ce93-146">Use the same `chainId` in subsequent requests to override the previous notification.</span></span>|
|<span data-ttu-id="4ce93-147">previewText</span><span class="sxs-lookup"><span data-stu-id="4ce93-147">previewText</span></span>|[<span data-ttu-id="4ce93-148">itemBody</span><span class="sxs-lookup"><span data-stu-id="4ce93-148">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="4ce93-149">Предварительный текст уведомления.</span><span class="sxs-lookup"><span data-stu-id="4ce93-149">Preview text for the notification.</span></span> <span data-ttu-id="4ce93-150">Microsoft Teams покажет только первые 150 символов.</span><span class="sxs-lookup"><span data-stu-id="4ce93-150">Microsoft Teams will only show first 150 characters.</span></span>|
|<span data-ttu-id="4ce93-151">templateParameters</span><span class="sxs-lookup"><span data-stu-id="4ce93-151">templateParameters</span></span>|<span data-ttu-id="4ce93-152">Коллекция [keyValuePair](../resources/keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="4ce93-152">[keyValuePair](../resources/keyvaluepair.md) collection</span></span>|<span data-ttu-id="4ce93-153">Значения для переменных шаблонов, определенных в записи ленты действий, соответствующие `activityType` [манифесту приложения Teams.](/microsoftteams/platform/overview)</span><span class="sxs-lookup"><span data-stu-id="4ce93-153">Values for template variables defined in the activity feed entry corresponding to `activityType` in [Teams app manifest](/microsoftteams/platform/overview).</span></span>|
|<span data-ttu-id="4ce93-154">получатель;</span><span class="sxs-lookup"><span data-stu-id="4ce93-154">recipient</span></span>|[<span data-ttu-id="4ce93-155">teamworkNotificationRecipient</span><span class="sxs-lookup"><span data-stu-id="4ce93-155">teamworkNotificationRecipient</span></span>](../resources/teamworknotificationrecipient.md)|<span data-ttu-id="4ce93-156">Получатель уведомления.</span><span class="sxs-lookup"><span data-stu-id="4ce93-156">Recipient of the notification.</span></span> <span data-ttu-id="4ce93-157">Поддерживаются только пользователи Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4ce93-157">Only Azure AD users are supported.</span></span> <span data-ttu-id="4ce93-158">См. [также aadUserNotificationRecipient](../resources/aadusernotificationrecipient.md).</span><span class="sxs-lookup"><span data-stu-id="4ce93-158">See also [aadUserNotificationRecipient](../resources/aadusernotificationrecipient.md).</span></span> |

<span data-ttu-id="4ce93-159">При настройке значения свойства темы для следующих ресурсов `source` поддерживаются следующие  `entityUrl` ресурсы:</span><span class="sxs-lookup"><span data-stu-id="4ce93-159">The following resources are supported when setting the `source` value of the **topic** property to `entityUrl`:</span></span>

- [<span data-ttu-id="4ce93-160">team</span><span class="sxs-lookup"><span data-stu-id="4ce93-160">team</span></span>](../resources/team.md)
- [<span data-ttu-id="4ce93-161">channel</span><span class="sxs-lookup"><span data-stu-id="4ce93-161">channel</span></span>](../resources/channel.md)
- [<span data-ttu-id="4ce93-162">chatMesage</span><span class="sxs-lookup"><span data-stu-id="4ce93-162">chatMesage</span></span>](../resources/chatmessage.md)
- [<span data-ttu-id="4ce93-163">teamsTab</span><span class="sxs-lookup"><span data-stu-id="4ce93-163">teamsTab</span></span>](../resources/teamstab.md)

> <span data-ttu-id="4ce93-164">**Примечание:** URL-адрес объекта должен быть одним и тем же или детским ресурсом группы в URL-адресе.</span><span class="sxs-lookup"><span data-stu-id="4ce93-164">**Note:** The entity URL must be same or child resource of the team in the URL.</span></span> <span data-ttu-id="4ce93-165">Кроме того, приложение [Teams должно](/microsoftteams/platform/overview) быть установлено в команде.</span><span class="sxs-lookup"><span data-stu-id="4ce93-165">Additionally, the [Teams app](/microsoftteams/platform/overview) must be installed in the team.</span></span>

## <a name="response"></a><span data-ttu-id="4ce93-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="4ce93-166">Response</span></span>

<span data-ttu-id="4ce93-167">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="4ce93-167">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="4ce93-168">Примеры</span><span class="sxs-lookup"><span data-stu-id="4ce93-168">Examples</span></span>

### <a name="example-1-notify-a-user-about-pending-finance-approval-requests"></a><span data-ttu-id="4ce93-169">Пример 1. Уведомление пользователя о ожидающих запросах на утверждение финансирования</span><span class="sxs-lookup"><span data-stu-id="4ce93-169">Example 1: Notify a user about pending finance approval requests</span></span>

<span data-ttu-id="4ce93-170">В этом примере показано, как можно отправить уведомление о канале действий для группы.</span><span class="sxs-lookup"><span data-stu-id="4ce93-170">This example shows how you can send an activity feed notification for a team.</span></span> <span data-ttu-id="4ce93-171">В этом примере владелец группы сообщает о ожидающих запросах на утверждение финансирования.</span><span class="sxs-lookup"><span data-stu-id="4ce93-171">This example notifies the team owner about pending finance approval requests.</span></span>

#### <a name="request"></a><span data-ttu-id="4ce93-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ce93-172">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="4ce93-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="4ce93-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/v1.0/teams/{teamId}"
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
# <a name="c"></a>[<span data-ttu-id="4ce93-174">C#</span><span class="sxs-lookup"><span data-stu-id="4ce93-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/team-sendactivitynotification-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4ce93-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4ce93-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/team-sendactivitynotification-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4ce93-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4ce93-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/team-sendactivitynotification-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4ce93-177">Java</span><span class="sxs-lookup"><span data-stu-id="4ce93-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/team-sendactivitynotification-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



---


#### <a name="response"></a><span data-ttu-id="4ce93-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ce93-178">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-notify-a-user-about-a-channel-tab"></a><span data-ttu-id="4ce93-179">Пример 2. Уведомление пользователя о вкладке канала</span><span class="sxs-lookup"><span data-stu-id="4ce93-179">Example 2: Notify a user about a channel tab</span></span>

<span data-ttu-id="4ce93-180">Как и в предыдущем примере, в этом примере `entityUrl` используется `topic` для .</span><span class="sxs-lookup"><span data-stu-id="4ce93-180">Similar to the previous example, this example uses `entityUrl` for the `topic`.</span></span> <span data-ttu-id="4ce93-181">Однако в этом примере ссылки на [вкладку](../resources/teamstab.md) в [канале](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="4ce93-181">However, this example links to a [tab](../resources/teamstab.md) in a [channel](../resources/channel.md).</span></span> <span data-ttu-id="4ce93-182">На вкладке размещена страница, показывающая пользователю состояние бронирования в отеле.</span><span class="sxs-lookup"><span data-stu-id="4ce93-182">The tab hosts a page showing the user the status of their hotel reservation.</span></span> <span data-ttu-id="4ce93-183">Выбор уведомления будет принимать пользователя на вкладке, где он может проверить свое бронирование.</span><span class="sxs-lookup"><span data-stu-id="4ce93-183">Selecting the notification will take the user to the tab, where they can check their reservation.</span></span>

#### <a name="request"></a><span data-ttu-id="4ce93-184">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ce93-184">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/v1.0/teams/{teamId}/channels/{channelId}/tabs/{tabId}"
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

#### <a name="response"></a><span data-ttu-id="4ce93-185">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ce93-185">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-3-notify-a-user-about-an-event-using-custom-topic"></a><span data-ttu-id="4ce93-186">Пример 3. Уведомление пользователя о событии с использованием настраиваемой темы</span><span class="sxs-lookup"><span data-stu-id="4ce93-186">Example 3: Notify a user about an event using custom topic</span></span>

<span data-ttu-id="4ce93-187">Как повествуют в предыдущих примерах, вы можете ссылаться на различные аспекты команды.</span><span class="sxs-lookup"><span data-stu-id="4ce93-187">As seen in the previous examples, you can link to different aspects of the team.</span></span> <span data-ttu-id="4ce93-188">Однако, если вы хотите связаться с аспектом, который не является частью команды или не представлен Microsoft Graph, или вы хотите настроить имя, вы можете установить источник и передать в настраиваемом значении для `topic` `text` него.</span><span class="sxs-lookup"><span data-stu-id="4ce93-188">However, if you want to link to an aspect that is not part of the team or is not represented by Microsoft Graph, or you want to customize the name, you can set the source of the `topic` to `text` and pass in a custom value for it.</span></span> <span data-ttu-id="4ce93-189">`webUrl` требуется при настройке `topic` источника `text` для .</span><span class="sxs-lookup"><span data-stu-id="4ce93-189">`webUrl` is required when setting `topic` source to `text`.</span></span>

#### <a name="request"></a><span data-ttu-id="4ce93-190">Запрос</span><span class="sxs-lookup"><span data-stu-id="4ce93-190">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/sendActivityNotification
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

#### <a name="response"></a><span data-ttu-id="4ce93-191">Отклик</span><span class="sxs-lookup"><span data-stu-id="4ce93-191">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```
