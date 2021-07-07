---
title: 'команда: sendActivityNotification'
description: Отправьте уведомление о канале действий в области группы.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 81b081ddf045cc1406903bd7d9b88edffc05480d
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2021
ms.locfileid: "53317157"
---
# <a name="team-sendactivitynotification"></a><span data-ttu-id="038ca-103">команда: sendActivityNotification</span><span class="sxs-lookup"><span data-stu-id="038ca-103">team: sendActivityNotification</span></span>
<span data-ttu-id="038ca-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="038ca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="038ca-105">Отправьте уведомление о канале действий в области группы.</span><span class="sxs-lookup"><span data-stu-id="038ca-105">Send an activity feed notification in the scope of a team.</span></span> <span data-ttu-id="038ca-106">Дополнительные сведения об отправке уведомлений и требованиях к этому см. в Teams [действия.](/graph/teams-send-activityfeednotifications)</span><span class="sxs-lookup"><span data-stu-id="038ca-106">For more details about sending notifications and the requirements for doing so, see [sending Teams activity notifications](/graph/teams-send-activityfeednotifications).</span></span>

## <a name="permissions"></a><span data-ttu-id="038ca-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="038ca-107">Permissions</span></span>
<span data-ttu-id="038ca-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="038ca-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="038ca-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="038ca-110">Permission type</span></span>|<span data-ttu-id="038ca-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="038ca-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="038ca-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="038ca-112">Delegated (work or school account)</span></span>|<span data-ttu-id="038ca-113">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="038ca-113">TeamsActivity.Send</span></span>|
|<span data-ttu-id="038ca-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="038ca-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="038ca-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="038ca-115">Not Supported.</span></span>|
|<span data-ttu-id="038ca-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="038ca-116">Application</span></span>|<span data-ttu-id="038ca-117">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="038ca-117">TeamsActivity.Send</span></span>|

## <a name="http-request"></a><span data-ttu-id="038ca-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="038ca-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /teams/{teamId}/sendActivityNotification
```

## <a name="request-headers"></a><span data-ttu-id="038ca-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="038ca-119">Request headers</span></span>
|<span data-ttu-id="038ca-120">Имя</span><span class="sxs-lookup"><span data-stu-id="038ca-120">Name</span></span>|<span data-ttu-id="038ca-121">Описание</span><span class="sxs-lookup"><span data-stu-id="038ca-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="038ca-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="038ca-122">Authorization</span></span>|<span data-ttu-id="038ca-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="038ca-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="038ca-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="038ca-125">Content-Type</span></span>|<span data-ttu-id="038ca-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="038ca-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="038ca-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="038ca-128">Request body</span></span>
<span data-ttu-id="038ca-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="038ca-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="038ca-130">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="038ca-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="038ca-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="038ca-131">Parameter</span></span>|<span data-ttu-id="038ca-132">Тип</span><span class="sxs-lookup"><span data-stu-id="038ca-132">Type</span></span>|<span data-ttu-id="038ca-133">Описание</span><span class="sxs-lookup"><span data-stu-id="038ca-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="038ca-134">topic</span><span class="sxs-lookup"><span data-stu-id="038ca-134">topic</span></span>|[<span data-ttu-id="038ca-135">teamworkActivityTopic</span><span class="sxs-lookup"><span data-stu-id="038ca-135">teamworkActivityTopic</span></span>](../resources/teamworkactivitytopic.md)|<span data-ttu-id="038ca-136">Тема уведомления.</span><span class="sxs-lookup"><span data-stu-id="038ca-136">Topic of the notification.</span></span> <span data-ttu-id="038ca-137">Указывает обсуждаемый ресурс.</span><span class="sxs-lookup"><span data-stu-id="038ca-137">Specifies the resource being talked about.</span></span>|
|<span data-ttu-id="038ca-138">activityType</span><span class="sxs-lookup"><span data-stu-id="038ca-138">activityType</span></span>|<span data-ttu-id="038ca-139">String</span><span class="sxs-lookup"><span data-stu-id="038ca-139">String</span></span>|<span data-ttu-id="038ca-140">Тип действия.</span><span class="sxs-lookup"><span data-stu-id="038ca-140">Activity type.</span></span> <span data-ttu-id="038ca-141">Это должно быть объявлено в [манифесте Teams приложения](/microsoftteams/platform/overview).</span><span class="sxs-lookup"><span data-stu-id="038ca-141">This must be declared in the [Teams app manifest](/microsoftteams/platform/overview).</span></span>|
|<span data-ttu-id="038ca-142">chainId</span><span class="sxs-lookup"><span data-stu-id="038ca-142">chainId</span></span>|<span data-ttu-id="038ca-143">Int64</span><span class="sxs-lookup"><span data-stu-id="038ca-143">Int64</span></span>|<span data-ttu-id="038ca-144">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="038ca-144">Optional.</span></span> <span data-ttu-id="038ca-145">Используется для переопределения предыдущего уведомления.</span><span class="sxs-lookup"><span data-stu-id="038ca-145">Used to override a previous notification.</span></span> <span data-ttu-id="038ca-146">Используйте то же `chainId` самое в последующих запросах для переопределения предыдущего уведомления.</span><span class="sxs-lookup"><span data-stu-id="038ca-146">Use the same `chainId` in subsequent requests to override the previous notification.</span></span>|
|<span data-ttu-id="038ca-147">previewText</span><span class="sxs-lookup"><span data-stu-id="038ca-147">previewText</span></span>|[<span data-ttu-id="038ca-148">itemBody</span><span class="sxs-lookup"><span data-stu-id="038ca-148">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="038ca-149">Предварительный текст уведомления.</span><span class="sxs-lookup"><span data-stu-id="038ca-149">Preview text for the notification.</span></span> <span data-ttu-id="038ca-150">Microsoft Teams только первые 150 символов.</span><span class="sxs-lookup"><span data-stu-id="038ca-150">Microsoft Teams will only show first 150 characters.</span></span>|
|<span data-ttu-id="038ca-151">templateParameters</span><span class="sxs-lookup"><span data-stu-id="038ca-151">templateParameters</span></span>|<span data-ttu-id="038ca-152">Коллекция [keyValuePair](../resources/keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="038ca-152">[keyValuePair](../resources/keyvaluepair.md) collection</span></span>|<span data-ttu-id="038ca-153">Значения переменных шаблонов, определенных в записи ленты действий, соответствующие манифесту `activityType` [Teams приложения.](/microsoftteams/platform/overview)</span><span class="sxs-lookup"><span data-stu-id="038ca-153">Values for template variables defined in the activity feed entry corresponding to `activityType` in [Teams app manifest](/microsoftteams/platform/overview).</span></span>|
|<span data-ttu-id="038ca-154">получатель;</span><span class="sxs-lookup"><span data-stu-id="038ca-154">recipient</span></span>|[<span data-ttu-id="038ca-155">teamworkNotificationRecipient</span><span class="sxs-lookup"><span data-stu-id="038ca-155">teamworkNotificationRecipient</span></span>](../resources/teamworknotificationrecipient.md)|<span data-ttu-id="038ca-156">Получатель уведомления.</span><span class="sxs-lookup"><span data-stu-id="038ca-156">Recipient of the notification.</span></span> <span data-ttu-id="038ca-157">См. [также aadUserNotificationRecipient,](../resources/aadusernotificationrecipient.md) [teamMembersNotificationRecipient](../resources/teammembersnotificationrecipient.md)и [channelMembersNotificationRecipient](../resources/channelmembersnotificationrecipient.md).</span><span class="sxs-lookup"><span data-stu-id="038ca-157">See also [aadUserNotificationRecipient](../resources/aadusernotificationrecipient.md), [teamMembersNotificationRecipient](../resources/teammembersnotificationrecipient.md), and [channelMembersNotificationRecipient](../resources/channelmembersnotificationrecipient.md).</span></span> |

<span data-ttu-id="038ca-158">При настройке значения свойства темы для следующих ресурсов `source` поддерживаются следующие  `entityUrl` ресурсы:</span><span class="sxs-lookup"><span data-stu-id="038ca-158">The following resources are supported when setting the `source` value of the **topic** property to `entityUrl`:</span></span>

- [<span data-ttu-id="038ca-159">team</span><span class="sxs-lookup"><span data-stu-id="038ca-159">team</span></span>](../resources/team.md)
- [<span data-ttu-id="038ca-160">channel</span><span class="sxs-lookup"><span data-stu-id="038ca-160">channel</span></span>](../resources/channel.md)
- [<span data-ttu-id="038ca-161">chatMesage</span><span class="sxs-lookup"><span data-stu-id="038ca-161">chatMesage</span></span>](../resources/chatmessage.md)
- [<span data-ttu-id="038ca-162">teamsTab</span><span class="sxs-lookup"><span data-stu-id="038ca-162">teamsTab</span></span>](../resources/teamstab.md)

> <span data-ttu-id="038ca-163">**Примечание:** URL-адрес объекта должен быть одним и тем же или детским ресурсом группы в URL-адресе.</span><span class="sxs-lookup"><span data-stu-id="038ca-163">**Note:** The entity URL must be same or child resource of the team in the URL.</span></span> <span data-ttu-id="038ca-164">Кроме того, [Teams приложение должно](/microsoftteams/platform/overview) быть установлено в команде.</span><span class="sxs-lookup"><span data-stu-id="038ca-164">Additionally, the [Teams app](/microsoftteams/platform/overview) must be installed in the team.</span></span>

## <a name="response"></a><span data-ttu-id="038ca-165">Ответ</span><span class="sxs-lookup"><span data-stu-id="038ca-165">Response</span></span>

<span data-ttu-id="038ca-166">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="038ca-166">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="038ca-167">Примеры</span><span class="sxs-lookup"><span data-stu-id="038ca-167">Examples</span></span>

### <a name="example-1-notify-a-user-about-pending-finance-approval-requests"></a><span data-ttu-id="038ca-168">Пример 1. Уведомление пользователя о ожидающих запросах на утверждение финансирования</span><span class="sxs-lookup"><span data-stu-id="038ca-168">Example 1: Notify a user about pending finance approval requests</span></span>

<span data-ttu-id="038ca-169">В этом примере показано, как можно отправить уведомление о канале действий для группы.</span><span class="sxs-lookup"><span data-stu-id="038ca-169">This example shows how you can send an activity feed notification for a team.</span></span> <span data-ttu-id="038ca-170">В этом примере владелец группы сообщает о ожидающих запросах на утверждение финансирования.</span><span class="sxs-lookup"><span data-stu-id="038ca-170">This example notifies the team owner about pending finance approval requests.</span></span>

#### <a name="request"></a><span data-ttu-id="038ca-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="038ca-171">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="038ca-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="038ca-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification_1"
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
# <a name="javascript"></a>[<span data-ttu-id="038ca-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="038ca-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/team-sendactivitynotification-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="038ca-174">C#</span><span class="sxs-lookup"><span data-stu-id="038ca-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/team-sendactivitynotification-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="038ca-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="038ca-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/team-sendactivitynotification-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="038ca-176">Java</span><span class="sxs-lookup"><span data-stu-id="038ca-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/team-sendactivitynotification-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="038ca-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="038ca-177">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-notify-a-user-about-a-channel-tab"></a><span data-ttu-id="038ca-178">Пример 2. Уведомление пользователя о вкладке канала</span><span class="sxs-lookup"><span data-stu-id="038ca-178">Example 2: Notify a user about a channel tab</span></span>

<span data-ttu-id="038ca-179">Как и в предыдущем примере, в этом примере `entityUrl` используется `topic` для .</span><span class="sxs-lookup"><span data-stu-id="038ca-179">Similar to the previous example, this example uses `entityUrl` for the `topic`.</span></span> <span data-ttu-id="038ca-180">Однако в этом примере ссылки на [вкладку](../resources/teamstab.md) в [канале](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="038ca-180">However, this example links to a [tab](../resources/teamstab.md) in a [channel](../resources/channel.md).</span></span> <span data-ttu-id="038ca-181">На вкладке размещена страница, показывающая пользователю состояние бронирования в отеле.</span><span class="sxs-lookup"><span data-stu-id="038ca-181">The tab hosts a page showing the user the status of their hotel reservation.</span></span> <span data-ttu-id="038ca-182">Выбор уведомления будет принимать пользователя на вкладке, где он может проверить свое бронирование.</span><span class="sxs-lookup"><span data-stu-id="038ca-182">Selecting the notification will take the user to the tab, where they can check their reservation.</span></span>

#### <a name="request"></a><span data-ttu-id="038ca-183">Запрос</span><span class="sxs-lookup"><span data-stu-id="038ca-183">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="038ca-184">HTTP</span><span class="sxs-lookup"><span data-stu-id="038ca-184">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification_2"
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
# <a name="c"></a>[<span data-ttu-id="038ca-185">C#</span><span class="sxs-lookup"><span data-stu-id="038ca-185">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/team-sendactivitynotification-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="038ca-186">JavaScript</span><span class="sxs-lookup"><span data-stu-id="038ca-186">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/team-sendactivitynotification-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="038ca-187">Objective-C</span><span class="sxs-lookup"><span data-stu-id="038ca-187">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/team-sendactivitynotification-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="038ca-188">Java</span><span class="sxs-lookup"><span data-stu-id="038ca-188">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/team-sendactivitynotification-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="038ca-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="038ca-189">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-3-notify-a-user-about-an-event-using-custom-topic"></a><span data-ttu-id="038ca-190">Пример 3. Уведомление пользователя о событии с использованием настраиваемой темы</span><span class="sxs-lookup"><span data-stu-id="038ca-190">Example 3: Notify a user about an event using custom topic</span></span>

<span data-ttu-id="038ca-191">Как повествуют в предыдущих примерах, вы можете ссылаться на различные аспекты команды.</span><span class="sxs-lookup"><span data-stu-id="038ca-191">As seen in the previous examples, you can link to different aspects of the team.</span></span> <span data-ttu-id="038ca-192">Однако если вы хотите связаться с аспектом, который не является частью команды или не представлен Корпорацией Майкрософт Graph, или вы хотите настроить имя, вы можете установить источник и передать в настраиваемом значении для `topic` `text` него.</span><span class="sxs-lookup"><span data-stu-id="038ca-192">However, if you want to link to an aspect that is not part of the team or is not represented by Microsoft Graph, or you want to customize the name, you can set the source of the `topic` to `text` and pass in a custom value for it.</span></span> <span data-ttu-id="038ca-193">`webUrl` требуется при настройке `topic` источника `text` для .</span><span class="sxs-lookup"><span data-stu-id="038ca-193">`webUrl` is required when setting `topic` source to `text`.</span></span>

#### <a name="request"></a><span data-ttu-id="038ca-194">Запрос</span><span class="sxs-lookup"><span data-stu-id="038ca-194">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="038ca-195">HTTP</span><span class="sxs-lookup"><span data-stu-id="038ca-195">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification_3"
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
# <a name="c"></a>[<span data-ttu-id="038ca-196">C#</span><span class="sxs-lookup"><span data-stu-id="038ca-196">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/team-sendactivitynotification-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="038ca-197">JavaScript</span><span class="sxs-lookup"><span data-stu-id="038ca-197">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/team-sendactivitynotification-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="038ca-198">Objective-C</span><span class="sxs-lookup"><span data-stu-id="038ca-198">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/team-sendactivitynotification-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="038ca-199">Java</span><span class="sxs-lookup"><span data-stu-id="038ca-199">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/team-sendactivitynotification-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="038ca-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="038ca-200">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-4-notify-the-team-members-about-pending-finance-approval-requests"></a><span data-ttu-id="038ca-201">Пример 4. Уведомление членов группы о ожидающих запросах на утверждение финансирования</span><span class="sxs-lookup"><span data-stu-id="038ca-201">Example 4: Notify the team members about pending finance approval requests</span></span>

<span data-ttu-id="038ca-202">В этом примере показано, как можно отправить уведомление о канале действий всем участникам группы.</span><span class="sxs-lookup"><span data-stu-id="038ca-202">This example shows how you can send an activity feed notification to all team members.</span></span> <span data-ttu-id="038ca-203">Этот пример похож на предыдущие примеры.</span><span class="sxs-lookup"><span data-stu-id="038ca-203">This example is similar to previous examples.</span></span> <span data-ttu-id="038ca-204">Однако в этом случае это `recipient` [teamMembersNotificationRecipient](../resources/teammembersnotificationrecipient.md).</span><span class="sxs-lookup"><span data-stu-id="038ca-204">However, in this case, the `recipient` is a [teamMembersNotificationRecipient](../resources/teammembersnotificationrecipient.md).</span></span> <span data-ttu-id="038ca-205">Обратите `teamId` внимание, что указанный в `recipient` должен соответствовать указанному `teamId` в URL-адресе запроса.</span><span class="sxs-lookup"><span data-stu-id="038ca-205">Note that the `teamId` specified in the `recipient` must match the `teamId` specified in the request URL.</span></span>

> <span data-ttu-id="038ca-206">**Примечание:** Возможность отправлять уведомления всем членам группы ограничена группами с 10 000 членов или менее.</span><span class="sxs-lookup"><span data-stu-id="038ca-206">**Note:** The ability to send notifications to all team members is limited to teams with 10,000 members or less.</span></span> <span data-ttu-id="038ca-207">Если количество членов группы превышает 10 000, никто из членов группы не получит уведомления.</span><span class="sxs-lookup"><span data-stu-id="038ca-207">If the team exceeds 10,000 members, none of the team members will receive a notification.</span></span>

#### <a name="request"></a><span data-ttu-id="038ca-208">Запрос</span><span class="sxs-lookup"><span data-stu-id="038ca-208">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="038ca-209">HTTP</span><span class="sxs-lookup"><span data-stu-id="038ca-209">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification_4"
}
-->

``` http
POST https://graph.microsoft.com/beta/teams/e8bece96-d393-4b9b-b8da-69cedef1a7e7/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/beta/teams/e8bece96-d393-4b9b-b8da-69cedef1a7e7"
    },
    "activityType": "pendingFinanceApprovalRequests",
    "previewText": {
        "content": "Internal spending team has a pending finance approval requests"
    },
    "recipient": {
        "@odata.type": "microsoft.graph.teamMembersNotificationRecipient",
        "teamId": "e8bece96-d393-4b9b-b8da-69cedef1a7e7"
    },
    "templateParameters": [
        {
            "name": "pendingRequestCount",
            "value": "5"
        }
    ] 
}
```
# <a name="c"></a>[<span data-ttu-id="038ca-210">C#</span><span class="sxs-lookup"><span data-stu-id="038ca-210">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/team-sendactivitynotification-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="038ca-211">JavaScript</span><span class="sxs-lookup"><span data-stu-id="038ca-211">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/team-sendactivitynotification-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="038ca-212">Objective-C</span><span class="sxs-lookup"><span data-stu-id="038ca-212">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/team-sendactivitynotification-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="038ca-213">Java</span><span class="sxs-lookup"><span data-stu-id="038ca-213">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/team-sendactivitynotification-4-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="038ca-214">Отклик</span><span class="sxs-lookup"><span data-stu-id="038ca-214">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-5-notify-the-channel-members-about-pending-finance-approval-requests"></a><span data-ttu-id="038ca-215">Пример 5. Уведомление участников канала о ожидающих запросах на утверждение финансирования</span><span class="sxs-lookup"><span data-stu-id="038ca-215">Example 5: Notify the channel members about pending finance approval requests</span></span>

<span data-ttu-id="038ca-216">В этом примере показано, как можно отправить уведомление о канале действий всем участникам канала.</span><span class="sxs-lookup"><span data-stu-id="038ca-216">This example shows how you can send an activity feed notification to all channel members.</span></span> <span data-ttu-id="038ca-217">Этот пример похож на предыдущий пример.</span><span class="sxs-lookup"><span data-stu-id="038ca-217">This example is similar to the previous example.</span></span> <span data-ttu-id="038ca-218">Однако в этом случае это `recipient` [каналMembersNotificationRecipient](../resources/channelmembersnotificationrecipient.md).</span><span class="sxs-lookup"><span data-stu-id="038ca-218">However, in this case, the `recipient` is a [channelMembersNotificationRecipient](../resources/channelmembersnotificationrecipient.md).</span></span> <span data-ttu-id="038ca-219">Обратите `teamId` внимание, что указанный в `recipient` должен соответствовать указанному `teamId` в URL-адресе запроса.</span><span class="sxs-lookup"><span data-stu-id="038ca-219">Note that the `teamId` specified in the `recipient` must match the `teamId` specified in the request URL.</span></span>

#### <a name="request"></a><span data-ttu-id="038ca-220">Запрос</span><span class="sxs-lookup"><span data-stu-id="038ca-220">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="038ca-221">HTTP</span><span class="sxs-lookup"><span data-stu-id="038ca-221">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification_5"
}
-->

``` http
POST https://graph.microsoft.com/beta/teams/e8bece96-d393-4b9b-b8da-69cedef1a7e7/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/beta/teams/e8bece96-d393-4b9b-b8da-69cedef1a7e7"
    },
    "activityType": "pendingFinanceApprovalRequests",
    "previewText": {
        "content": "Internal spending team has a pending finance approval requests"
    },
    "recipient": {
        "@odata.type": "microsoft.graph.channelMembersNotificationRecipient",
        "teamId": "e8bece96-d393-4b9b-b8da-69cedef1a7e7",
        "channelId": "19:3d61a2309f094f4a9310b20f1db37520@thread.tacv2"
    },
    "templateParameters": [
        {
            "name": "pendingRequestCount",
            "value": "5"
        }
    ] 
}
```
# <a name="c"></a>[<span data-ttu-id="038ca-222">C#</span><span class="sxs-lookup"><span data-stu-id="038ca-222">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/team-sendactivitynotification-5-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="038ca-223">JavaScript</span><span class="sxs-lookup"><span data-stu-id="038ca-223">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/team-sendactivitynotification-5-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="038ca-224">Objective-C</span><span class="sxs-lookup"><span data-stu-id="038ca-224">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/team-sendactivitynotification-5-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="038ca-225">Java</span><span class="sxs-lookup"><span data-stu-id="038ca-225">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/team-sendactivitynotification-5-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="038ca-226">Отклик</span><span class="sxs-lookup"><span data-stu-id="038ca-226">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```
