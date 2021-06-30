---
title: 'команда: sendActivityNotification'
description: Отправьте уведомление о канале действий в области группы.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e16d6aade57dfb10f4cd387d9d6719c85c2c3b79
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209340"
---
# <a name="team-sendactivitynotification"></a><span data-ttu-id="c76f9-103">команда: sendActivityNotification</span><span class="sxs-lookup"><span data-stu-id="c76f9-103">team: sendActivityNotification</span></span>
<span data-ttu-id="c76f9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c76f9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c76f9-105">Отправьте уведомление о канале действий в области группы.</span><span class="sxs-lookup"><span data-stu-id="c76f9-105">Send an activity feed notification in the scope of a team.</span></span> <span data-ttu-id="c76f9-106">Дополнительные сведения об отправке уведомлений и требованиях к этому см. в Teams [действия.](/graph/teams-send-activityfeednotifications)</span><span class="sxs-lookup"><span data-stu-id="c76f9-106">For more details about sending notifications and the requirements for doing so, see [sending Teams activity notifications](/graph/teams-send-activityfeednotifications).</span></span>

## <a name="permissions"></a><span data-ttu-id="c76f9-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c76f9-107">Permissions</span></span>
<span data-ttu-id="c76f9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c76f9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c76f9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c76f9-110">Permission type</span></span>|<span data-ttu-id="c76f9-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c76f9-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c76f9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c76f9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c76f9-113">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="c76f9-113">TeamsActivity.Send</span></span>|
|<span data-ttu-id="c76f9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c76f9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c76f9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c76f9-115">Not Supported.</span></span>|
|<span data-ttu-id="c76f9-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="c76f9-116">Application</span></span>|<span data-ttu-id="c76f9-117">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="c76f9-117">TeamsActivity.Send</span></span>|

## <a name="http-request"></a><span data-ttu-id="c76f9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c76f9-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /teams/{teamId}/sendActivityNotification
```

## <a name="request-headers"></a><span data-ttu-id="c76f9-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c76f9-119">Request headers</span></span>
|<span data-ttu-id="c76f9-120">Имя</span><span class="sxs-lookup"><span data-stu-id="c76f9-120">Name</span></span>|<span data-ttu-id="c76f9-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c76f9-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c76f9-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c76f9-122">Authorization</span></span>|<span data-ttu-id="c76f9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c76f9-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c76f9-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c76f9-125">Content-Type</span></span>|<span data-ttu-id="c76f9-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c76f9-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c76f9-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c76f9-128">Request body</span></span>
<span data-ttu-id="c76f9-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c76f9-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c76f9-130">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="c76f9-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c76f9-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="c76f9-131">Parameter</span></span>|<span data-ttu-id="c76f9-132">Тип</span><span class="sxs-lookup"><span data-stu-id="c76f9-132">Type</span></span>|<span data-ttu-id="c76f9-133">Описание</span><span class="sxs-lookup"><span data-stu-id="c76f9-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c76f9-134">topic</span><span class="sxs-lookup"><span data-stu-id="c76f9-134">topic</span></span>|[<span data-ttu-id="c76f9-135">teamworkActivityTopic</span><span class="sxs-lookup"><span data-stu-id="c76f9-135">teamworkActivityTopic</span></span>](../resources/teamworkactivitytopic.md)|<span data-ttu-id="c76f9-136">Тема уведомления.</span><span class="sxs-lookup"><span data-stu-id="c76f9-136">Topic of the notification.</span></span> <span data-ttu-id="c76f9-137">Указывает обсуждаемый ресурс.</span><span class="sxs-lookup"><span data-stu-id="c76f9-137">Specifies the resource being talked about.</span></span>|
|<span data-ttu-id="c76f9-138">activityType</span><span class="sxs-lookup"><span data-stu-id="c76f9-138">activityType</span></span>|<span data-ttu-id="c76f9-139">String</span><span class="sxs-lookup"><span data-stu-id="c76f9-139">String</span></span>|<span data-ttu-id="c76f9-140">Тип действия.</span><span class="sxs-lookup"><span data-stu-id="c76f9-140">Activity type.</span></span> <span data-ttu-id="c76f9-141">Это должно быть объявлено в [манифесте Teams приложения](/microsoftteams/platform/overview).</span><span class="sxs-lookup"><span data-stu-id="c76f9-141">This must be declared in the [Teams app manifest](/microsoftteams/platform/overview).</span></span>|
|<span data-ttu-id="c76f9-142">chainId</span><span class="sxs-lookup"><span data-stu-id="c76f9-142">chainId</span></span>|<span data-ttu-id="c76f9-143">Int64</span><span class="sxs-lookup"><span data-stu-id="c76f9-143">Int64</span></span>|<span data-ttu-id="c76f9-144">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="c76f9-144">Optional.</span></span> <span data-ttu-id="c76f9-145">Используется для переопределения предыдущего уведомления.</span><span class="sxs-lookup"><span data-stu-id="c76f9-145">Used to override a previous notification.</span></span> <span data-ttu-id="c76f9-146">Используйте то же `chainId` самое в последующих запросах для переопределения предыдущего уведомления.</span><span class="sxs-lookup"><span data-stu-id="c76f9-146">Use the same `chainId` in subsequent requests to override the previous notification.</span></span>|
|<span data-ttu-id="c76f9-147">previewText</span><span class="sxs-lookup"><span data-stu-id="c76f9-147">previewText</span></span>|[<span data-ttu-id="c76f9-148">itemBody</span><span class="sxs-lookup"><span data-stu-id="c76f9-148">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="c76f9-149">Предварительный текст уведомления.</span><span class="sxs-lookup"><span data-stu-id="c76f9-149">Preview text for the notification.</span></span> <span data-ttu-id="c76f9-150">Microsoft Teams только первые 150 символов.</span><span class="sxs-lookup"><span data-stu-id="c76f9-150">Microsoft Teams will only show first 150 characters.</span></span>|
|<span data-ttu-id="c76f9-151">templateParameters</span><span class="sxs-lookup"><span data-stu-id="c76f9-151">templateParameters</span></span>|<span data-ttu-id="c76f9-152">Коллекция [keyValuePair](../resources/keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="c76f9-152">[keyValuePair](../resources/keyvaluepair.md) collection</span></span>|<span data-ttu-id="c76f9-153">Значения переменных шаблонов, определенных в записи ленты действий, соответствующие манифесту `activityType` [Teams приложения.](/microsoftteams/platform/overview)</span><span class="sxs-lookup"><span data-stu-id="c76f9-153">Values for template variables defined in the activity feed entry corresponding to `activityType` in [Teams app manifest](/microsoftteams/platform/overview).</span></span>|
|<span data-ttu-id="c76f9-154">получатель;</span><span class="sxs-lookup"><span data-stu-id="c76f9-154">recipient</span></span>|[<span data-ttu-id="c76f9-155">teamworkNotificationRecipient</span><span class="sxs-lookup"><span data-stu-id="c76f9-155">teamworkNotificationRecipient</span></span>](../resources/teamworknotificationrecipient.md)|<span data-ttu-id="c76f9-156">Получатель уведомления.</span><span class="sxs-lookup"><span data-stu-id="c76f9-156">Recipient of the notification.</span></span> <span data-ttu-id="c76f9-157">См. [также aadUserNotificationRecipient,](../resources/aadusernotificationrecipient.md) [teamMembersNotificationRecipient](../resources/teammembersnotificationrecipient.md)и [channelMembersNotificationRecipient](../resources/channelmembersnotificationrecipient.md).</span><span class="sxs-lookup"><span data-stu-id="c76f9-157">See also [aadUserNotificationRecipient](../resources/aadusernotificationrecipient.md), [teamMembersNotificationRecipient](../resources/teammembersnotificationrecipient.md), and [channelMembersNotificationRecipient](../resources/channelmembersnotificationrecipient.md).</span></span> |

<span data-ttu-id="c76f9-158">При настройке значения свойства темы для следующих ресурсов `source` поддерживаются следующие  `entityUrl` ресурсы:</span><span class="sxs-lookup"><span data-stu-id="c76f9-158">The following resources are supported when setting the `source` value of the **topic** property to `entityUrl`:</span></span>

- [<span data-ttu-id="c76f9-159">team</span><span class="sxs-lookup"><span data-stu-id="c76f9-159">team</span></span>](../resources/team.md)
- [<span data-ttu-id="c76f9-160">channel</span><span class="sxs-lookup"><span data-stu-id="c76f9-160">channel</span></span>](../resources/channel.md)
- [<span data-ttu-id="c76f9-161">chatMesage</span><span class="sxs-lookup"><span data-stu-id="c76f9-161">chatMesage</span></span>](../resources/chatmessage.md)
- [<span data-ttu-id="c76f9-162">teamsTab</span><span class="sxs-lookup"><span data-stu-id="c76f9-162">teamsTab</span></span>](../resources/teamstab.md)

> <span data-ttu-id="c76f9-163">**Примечание:** URL-адрес объекта должен быть одним и тем же или детским ресурсом группы в URL-адресе.</span><span class="sxs-lookup"><span data-stu-id="c76f9-163">**Note:** The entity URL must be same or child resource of the team in the URL.</span></span> <span data-ttu-id="c76f9-164">Кроме того, [Teams приложение должно](/microsoftteams/platform/overview) быть установлено в команде.</span><span class="sxs-lookup"><span data-stu-id="c76f9-164">Additionally, the [Teams app](/microsoftteams/platform/overview) must be installed in the team.</span></span>

## <a name="response"></a><span data-ttu-id="c76f9-165">Ответ</span><span class="sxs-lookup"><span data-stu-id="c76f9-165">Response</span></span>

<span data-ttu-id="c76f9-166">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c76f9-166">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="c76f9-167">Примеры</span><span class="sxs-lookup"><span data-stu-id="c76f9-167">Examples</span></span>

### <a name="example-1-notify-a-user-about-pending-finance-approval-requests"></a><span data-ttu-id="c76f9-168">Пример 1. Уведомление пользователя о ожидающих запросах на утверждение финансирования</span><span class="sxs-lookup"><span data-stu-id="c76f9-168">Example 1: Notify a user about pending finance approval requests</span></span>

<span data-ttu-id="c76f9-169">В этом примере показано, как можно отправить уведомление о канале действий для группы.</span><span class="sxs-lookup"><span data-stu-id="c76f9-169">This example shows how you can send an activity feed notification for a team.</span></span> <span data-ttu-id="c76f9-170">В этом примере владелец группы сообщает о ожидающих запросах на утверждение финансирования.</span><span class="sxs-lookup"><span data-stu-id="c76f9-170">This example notifies the team owner about pending finance approval requests.</span></span>

#### <a name="request"></a><span data-ttu-id="c76f9-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="c76f9-171">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c76f9-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="c76f9-172">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="c76f9-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c76f9-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/team-sendactivitynotification-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="c76f9-174">C#</span><span class="sxs-lookup"><span data-stu-id="c76f9-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/team-sendactivitynotification-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c76f9-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c76f9-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/team-sendactivitynotification-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c76f9-176">Java</span><span class="sxs-lookup"><span data-stu-id="c76f9-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/team-sendactivitynotification-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c76f9-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="c76f9-177">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-notify-a-user-about-a-channel-tab"></a><span data-ttu-id="c76f9-178">Пример 2. Уведомление пользователя о вкладке канала</span><span class="sxs-lookup"><span data-stu-id="c76f9-178">Example 2: Notify a user about a channel tab</span></span>

<span data-ttu-id="c76f9-179">Как и в предыдущем примере, в этом примере `entityUrl` используется `topic` для .</span><span class="sxs-lookup"><span data-stu-id="c76f9-179">Similar to the previous example, this example uses `entityUrl` for the `topic`.</span></span> <span data-ttu-id="c76f9-180">Однако в этом примере ссылки на [вкладку](../resources/teamstab.md) в [канале](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="c76f9-180">However, this example links to a [tab](../resources/teamstab.md) in a [channel](../resources/channel.md).</span></span> <span data-ttu-id="c76f9-181">На вкладке размещена страница, показывающая пользователю состояние бронирования в отеле.</span><span class="sxs-lookup"><span data-stu-id="c76f9-181">The tab hosts a page showing the user the status of their hotel reservation.</span></span> <span data-ttu-id="c76f9-182">Выбор уведомления будет принимать пользователя на вкладке, где он может проверить свое бронирование.</span><span class="sxs-lookup"><span data-stu-id="c76f9-182">Selecting the notification will take the user to the tab, where they can check their reservation.</span></span>

#### <a name="request"></a><span data-ttu-id="c76f9-183">Запрос</span><span class="sxs-lookup"><span data-stu-id="c76f9-183">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c76f9-184">HTTP</span><span class="sxs-lookup"><span data-stu-id="c76f9-184">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c76f9-185">C#</span><span class="sxs-lookup"><span data-stu-id="c76f9-185">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/team-sendactivitynotification-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c76f9-186">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c76f9-186">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/team-sendactivitynotification-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c76f9-187">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c76f9-187">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/team-sendactivitynotification-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c76f9-188">Java</span><span class="sxs-lookup"><span data-stu-id="c76f9-188">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/team-sendactivitynotification-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c76f9-189">Отклик</span><span class="sxs-lookup"><span data-stu-id="c76f9-189">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-3-notify-a-user-about-an-event-using-custom-topic"></a><span data-ttu-id="c76f9-190">Пример 3. Уведомление пользователя о событии с использованием настраиваемой темы</span><span class="sxs-lookup"><span data-stu-id="c76f9-190">Example 3: Notify a user about an event using custom topic</span></span>

<span data-ttu-id="c76f9-191">Как повествуют в предыдущих примерах, вы можете ссылаться на различные аспекты команды.</span><span class="sxs-lookup"><span data-stu-id="c76f9-191">As seen in the previous examples, you can link to different aspects of the team.</span></span> <span data-ttu-id="c76f9-192">Однако если вы хотите связаться с аспектом, который не является частью команды или не представлен Корпорацией Майкрософт Graph, или вы хотите настроить имя, вы можете установить источник и передать в настраиваемом значении для `topic` `text` него.</span><span class="sxs-lookup"><span data-stu-id="c76f9-192">However, if you want to link to an aspect that is not part of the team or is not represented by Microsoft Graph, or you want to customize the name, you can set the source of the `topic` to `text` and pass in a custom value for it.</span></span> <span data-ttu-id="c76f9-193">`webUrl` требуется при настройке `topic` источника `text` для .</span><span class="sxs-lookup"><span data-stu-id="c76f9-193">`webUrl` is required when setting `topic` source to `text`.</span></span>

#### <a name="request"></a><span data-ttu-id="c76f9-194">Запрос</span><span class="sxs-lookup"><span data-stu-id="c76f9-194">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c76f9-195">HTTP</span><span class="sxs-lookup"><span data-stu-id="c76f9-195">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c76f9-196">C#</span><span class="sxs-lookup"><span data-stu-id="c76f9-196">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/team-sendactivitynotification-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c76f9-197">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c76f9-197">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/team-sendactivitynotification-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c76f9-198">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c76f9-198">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/team-sendactivitynotification-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c76f9-199">Java</span><span class="sxs-lookup"><span data-stu-id="c76f9-199">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/team-sendactivitynotification-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c76f9-200">Отклик</span><span class="sxs-lookup"><span data-stu-id="c76f9-200">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-4-notify-the-team-members-about-pending-finance-approval-requests"></a><span data-ttu-id="c76f9-201">Пример 4. Уведомление членов группы о ожидающих запросах на утверждение финансирования</span><span class="sxs-lookup"><span data-stu-id="c76f9-201">Example 4: Notify the team members about pending finance approval requests</span></span>

<span data-ttu-id="c76f9-202">В этом примере показано, как можно отправить уведомление о канале действий всем участникам группы.</span><span class="sxs-lookup"><span data-stu-id="c76f9-202">This example shows how you can send an activity feed notification to all team members.</span></span> <span data-ttu-id="c76f9-203">Этот пример похож на предыдущие примеры.</span><span class="sxs-lookup"><span data-stu-id="c76f9-203">This example is similar to previous examples.</span></span> <span data-ttu-id="c76f9-204">Однако в этом случае это `recipient` [teamMembersNotificationRecipient](../resources/teammembersnotificationrecipient.md).</span><span class="sxs-lookup"><span data-stu-id="c76f9-204">However, in this case, the `recipient` is a [teamMembersNotificationRecipient](../resources/teammembersnotificationrecipient.md).</span></span> <span data-ttu-id="c76f9-205">Обратите `teamId` внимание, что указанный в `recipient` должен соответствовать указанному `teamId` в URL-адресе запроса.</span><span class="sxs-lookup"><span data-stu-id="c76f9-205">Note that the `teamId` specified in the `recipient` must match the `teamId` specified in the request URL.</span></span>

> <span data-ttu-id="c76f9-206">**Примечание:** Возможность отправлять уведомления всем членам группы ограничена группами с 10 000 членов или менее.</span><span class="sxs-lookup"><span data-stu-id="c76f9-206">**Note:** The ability to send notifications to all team members is limited to teams with 10,000 members or less.</span></span> <span data-ttu-id="c76f9-207">Если количество членов группы превышает 10 000, никто из членов группы не получит уведомления.</span><span class="sxs-lookup"><span data-stu-id="c76f9-207">If the team exceeds 10,000 members, none of the team members will receive a notification.</span></span>

#### <a name="request"></a><span data-ttu-id="c76f9-208">Запрос</span><span class="sxs-lookup"><span data-stu-id="c76f9-208">Request</span></span>
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

#### <a name="response"></a><span data-ttu-id="c76f9-209">Отклик</span><span class="sxs-lookup"><span data-stu-id="c76f9-209">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-5-notify-the-channel-members-about-pending-finance-approval-requests"></a><span data-ttu-id="c76f9-210">Пример 5. Уведомление участников канала о ожидающих запросах на утверждение финансирования</span><span class="sxs-lookup"><span data-stu-id="c76f9-210">Example 5: Notify the channel members about pending finance approval requests</span></span>

<span data-ttu-id="c76f9-211">В этом примере показано, как можно отправить уведомление о канале действий всем участникам канала.</span><span class="sxs-lookup"><span data-stu-id="c76f9-211">This example shows how you can send an activity feed notification to all channel members.</span></span> <span data-ttu-id="c76f9-212">Этот пример похож на предыдущий пример.</span><span class="sxs-lookup"><span data-stu-id="c76f9-212">This example is similar to the previous example.</span></span> <span data-ttu-id="c76f9-213">Однако в этом случае это `recipient` [каналMembersNotificationRecipient](../resources/channelmembersnotificationrecipient.md).</span><span class="sxs-lookup"><span data-stu-id="c76f9-213">However, in this case, the `recipient` is a [channelMembersNotificationRecipient](../resources/channelmembersnotificationrecipient.md).</span></span> <span data-ttu-id="c76f9-214">Обратите `teamId` внимание, что указанный в `recipient` должен соответствовать указанному `teamId` в URL-адресе запроса.</span><span class="sxs-lookup"><span data-stu-id="c76f9-214">Note that the `teamId` specified in the `recipient` must match the `teamId` specified in the request URL.</span></span>

#### <a name="request"></a><span data-ttu-id="c76f9-215">Запрос</span><span class="sxs-lookup"><span data-stu-id="c76f9-215">Request</span></span>
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

#### <a name="response"></a><span data-ttu-id="c76f9-216">Отклик</span><span class="sxs-lookup"><span data-stu-id="c76f9-216">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```
