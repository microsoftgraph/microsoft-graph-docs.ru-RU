---
title: 'команда: Сендактивитинотификатион'
description: Отправка уведомления о канале активности в области действия команды.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ed7177f4a91fae4fb5e87f496489cdc0c9569607
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377612"
---
# <a name="team-sendactivitynotification"></a><span data-ttu-id="71f8d-103">команда: Сендактивитинотификатион</span><span class="sxs-lookup"><span data-stu-id="71f8d-103">team: sendActivityNotification</span></span>
<span data-ttu-id="71f8d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71f8d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="71f8d-105">Отправка уведомления о канале активности в области действия команды.</span><span class="sxs-lookup"><span data-stu-id="71f8d-105">Send an activity feed notification in the scope of a team.</span></span> <span data-ttu-id="71f8d-106">Дополнительные сведения об отправке уведомлений и требованиях для этого можно найти в разделе [Отправка уведомлений о действиях в группах](/graph/teams-send-activityfeednotifications).</span><span class="sxs-lookup"><span data-stu-id="71f8d-106">For more details about sending notifications and the requirements for doing so, see [sending Teams activity notifications](/graph/teams-send-activityfeednotifications).</span></span>

## <a name="permissions"></a><span data-ttu-id="71f8d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="71f8d-107">Permissions</span></span>
<span data-ttu-id="71f8d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71f8d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71f8d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71f8d-110">Permission type</span></span>|<span data-ttu-id="71f8d-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="71f8d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71f8d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71f8d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="71f8d-113">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="71f8d-113">TeamsActivity.Send</span></span>|
|<span data-ttu-id="71f8d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71f8d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71f8d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71f8d-115">Not Supported.</span></span>|
|<span data-ttu-id="71f8d-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="71f8d-116">Application</span></span>|<span data-ttu-id="71f8d-117">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="71f8d-117">TeamsActivity.Send</span></span>|

## <a name="http-request"></a><span data-ttu-id="71f8d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71f8d-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /teams/{teamId}/sendActivityNotification
```

## <a name="request-headers"></a><span data-ttu-id="71f8d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="71f8d-119">Request headers</span></span>
|<span data-ttu-id="71f8d-120">Имя</span><span class="sxs-lookup"><span data-stu-id="71f8d-120">Name</span></span>|<span data-ttu-id="71f8d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="71f8d-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="71f8d-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="71f8d-122">Authorization</span></span>|<span data-ttu-id="71f8d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="71f8d-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="71f8d-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="71f8d-125">Content-Type</span></span>|<span data-ttu-id="71f8d-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="71f8d-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="71f8d-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="71f8d-128">Request body</span></span>
<span data-ttu-id="71f8d-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="71f8d-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="71f8d-130">В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="71f8d-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="71f8d-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="71f8d-131">Parameter</span></span>|<span data-ttu-id="71f8d-132">Тип</span><span class="sxs-lookup"><span data-stu-id="71f8d-132">Type</span></span>|<span data-ttu-id="71f8d-133">Описание</span><span class="sxs-lookup"><span data-stu-id="71f8d-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71f8d-134">topic</span><span class="sxs-lookup"><span data-stu-id="71f8d-134">topic</span></span>|[<span data-ttu-id="71f8d-135">теамворкактивититопик</span><span class="sxs-lookup"><span data-stu-id="71f8d-135">teamworkActivityTopic</span></span>](../resources/teamworkactivitytopic.md)|<span data-ttu-id="71f8d-136">Тема уведомления.</span><span class="sxs-lookup"><span data-stu-id="71f8d-136">Topic of the notification.</span></span> <span data-ttu-id="71f8d-137">Указывает ресурс, о котором идет речь.</span><span class="sxs-lookup"><span data-stu-id="71f8d-137">Specifies the resource being talked about.</span></span>|
|<span data-ttu-id="71f8d-138">activityType</span><span class="sxs-lookup"><span data-stu-id="71f8d-138">activityType</span></span>|<span data-ttu-id="71f8d-139">String</span><span class="sxs-lookup"><span data-stu-id="71f8d-139">String</span></span>|<span data-ttu-id="71f8d-140">Тип действия.</span><span class="sxs-lookup"><span data-stu-id="71f8d-140">Activity type.</span></span> <span data-ttu-id="71f8d-141">Он должен быть объявлен в [манифесте приложения Teams](/microsoftteams/platform/overview).</span><span class="sxs-lookup"><span data-stu-id="71f8d-141">This must be declared in the [Teams app manifest](/microsoftteams/platform/overview).</span></span>|
|<span data-ttu-id="71f8d-142">чаинид</span><span class="sxs-lookup"><span data-stu-id="71f8d-142">chainId</span></span>|<span data-ttu-id="71f8d-143">Int64</span><span class="sxs-lookup"><span data-stu-id="71f8d-143">Int64</span></span>|<span data-ttu-id="71f8d-144">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="71f8d-144">Optional.</span></span> <span data-ttu-id="71f8d-145">Используется для переопределения предыдущего уведомления.</span><span class="sxs-lookup"><span data-stu-id="71f8d-145">Used to override a previous notification.</span></span> <span data-ttu-id="71f8d-146">Используйте одно и то же `chainId` в последующих запросах для переопределения предыдущего уведомления.</span><span class="sxs-lookup"><span data-stu-id="71f8d-146">Use the same `chainId` in subsequent requests to override the previous notification.</span></span>|
|<span data-ttu-id="71f8d-147">previewText</span><span class="sxs-lookup"><span data-stu-id="71f8d-147">previewText</span></span>|[<span data-ttu-id="71f8d-148">itemBody</span><span class="sxs-lookup"><span data-stu-id="71f8d-148">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="71f8d-149">Предварительный просмотр текста уведомления.</span><span class="sxs-lookup"><span data-stu-id="71f8d-149">Preview text for the notification.</span></span> <span data-ttu-id="71f8d-150">Microsoft Teams будет показывать только первые 150 символов.</span><span class="sxs-lookup"><span data-stu-id="71f8d-150">Microsoft Teams will only show first 150 characters.</span></span>|
|<span data-ttu-id="71f8d-151">темплатепараметерс</span><span class="sxs-lookup"><span data-stu-id="71f8d-151">templateParameters</span></span>|<span data-ttu-id="71f8d-152">Коллекция [keyValuePair](../resources/keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="71f8d-152">[keyValuePair](../resources/keyvaluepair.md) collection</span></span>|<span data-ttu-id="71f8d-153">Значения для переменных шаблона, определенных в записи веб-канала активности, соответствующей `activityType` [манифесту приложения Teams](/microsoftteams/platform/overview).</span><span class="sxs-lookup"><span data-stu-id="71f8d-153">Values for template variables defined in the activity feed entry corresponding to `activityType` in [Teams app manifest](/microsoftteams/platform/overview).</span></span>|
|<span data-ttu-id="71f8d-154">получатель;</span><span class="sxs-lookup"><span data-stu-id="71f8d-154">recipient</span></span>|[<span data-ttu-id="71f8d-155">теамворкнотификатионреЦипиент</span><span class="sxs-lookup"><span data-stu-id="71f8d-155">teamworkNotificationRecipient</span></span>](../resources/teamworknotificationrecipient.md)|<span data-ttu-id="71f8d-156">Получатель уведомления.</span><span class="sxs-lookup"><span data-stu-id="71f8d-156">Recipient of the notification.</span></span> <span data-ttu-id="71f8d-157">Поддерживаются только пользователи Azure AD.</span><span class="sxs-lookup"><span data-stu-id="71f8d-157">Only Azure AD users are supported.</span></span> <span data-ttu-id="71f8d-158">См. также [аадусернотификатионреЦипиент](../resources/aadusernotificationrecipient.md).</span><span class="sxs-lookup"><span data-stu-id="71f8d-158">See also [aadUserNotificationRecipient](../resources/aadusernotificationrecipient.md).</span></span> |

<span data-ttu-id="71f8d-159">Следующие ресурсы поддерживаются при задании `source` значения свойства **Topic** `entityUrl` следующим образом:</span><span class="sxs-lookup"><span data-stu-id="71f8d-159">The following resources are supported when setting the `source` value of the **topic** property to `entityUrl`:</span></span>

- [<span data-ttu-id="71f8d-160">team</span><span class="sxs-lookup"><span data-stu-id="71f8d-160">team</span></span>](../resources/team.md)
- [<span data-ttu-id="71f8d-161">channel</span><span class="sxs-lookup"><span data-stu-id="71f8d-161">channel</span></span>](../resources/channel.md)
- [<span data-ttu-id="71f8d-162">чатмесаже</span><span class="sxs-lookup"><span data-stu-id="71f8d-162">chatMesage</span></span>](../resources/chatmessage.md)
- [<span data-ttu-id="71f8d-163">teamsTab</span><span class="sxs-lookup"><span data-stu-id="71f8d-163">teamsTab</span></span>](../resources/teamstab.md)

> <span data-ttu-id="71f8d-164">**Примечание:** URL-адрес сущности должен быть таким же или дочерним ресурсом команды в URL-адресе.</span><span class="sxs-lookup"><span data-stu-id="71f8d-164">**Note:** The entity url must be same or child resource of the team in the url.</span></span> <span data-ttu-id="71f8d-165">Кроме того, в команде должно быть установлено [приложение](/microsoftteams/platform/overview) Teams.</span><span class="sxs-lookup"><span data-stu-id="71f8d-165">Additionally, the [Teams app](/microsoftteams/platform/overview) must be installed in the team.</span></span>

## <a name="response"></a><span data-ttu-id="71f8d-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="71f8d-166">Response</span></span>

<span data-ttu-id="71f8d-167">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="71f8d-167">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="71f8d-168">Примеры</span><span class="sxs-lookup"><span data-stu-id="71f8d-168">Examples</span></span>

### <a name="example-1-notify-a-user-about-pending-finance-approval-requests"></a><span data-ttu-id="71f8d-169">Пример 1: уведомить пользователя о предопределенном запросе на утверждение в финансах</span><span class="sxs-lookup"><span data-stu-id="71f8d-169">Example 1: Notify a user about pending finance approval requests</span></span>

<span data-ttu-id="71f8d-170">В этом примере показано, как можно отправить уведомление веб-канала активности для команды.</span><span class="sxs-lookup"><span data-stu-id="71f8d-170">This example shows how you can send an activity feed notification for a team.</span></span> <span data-ttu-id="71f8d-171">В этом примере владелец команды уведомляется о незавершенных запросах на утверждение в финансах.</span><span class="sxs-lookup"><span data-stu-id="71f8d-171">This example notifies the team owner about pending finance approval requests.</span></span>

#### <a name="request"></a><span data-ttu-id="71f8d-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="71f8d-172">Request</span></span>
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

#### <a name="response"></a><span data-ttu-id="71f8d-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="71f8d-173">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-notify-a-user-about-a-channel-tab"></a><span data-ttu-id="71f8d-174">Пример 2: уведомление пользователя о вкладке канала</span><span class="sxs-lookup"><span data-stu-id="71f8d-174">Example 2: Notify a user about a channel tab</span></span>

<span data-ttu-id="71f8d-175">Как и в предыдущем примере, в этом примере используется `entityUrl` для `topic` .</span><span class="sxs-lookup"><span data-stu-id="71f8d-175">Similar to the previous example, this example uses `entityUrl` for the `topic`.</span></span> <span data-ttu-id="71f8d-176">Однако в этом примере показано, как создать ссылку на [вкладку](../resources/teamstab.md) в [канале](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="71f8d-176">However, this example links to a [tab](../resources/teamstab.md) in a [channel](../resources/channel.md).</span></span> <span data-ttu-id="71f8d-177">На вкладке размещается страница, на которой пользователь находится в состоянии бронирования гостиницы.</span><span class="sxs-lookup"><span data-stu-id="71f8d-177">The tab hosts a page showing the user the status of their hotel reservation.</span></span> <span data-ttu-id="71f8d-178">При выборе уведомления пользователь будет переходить на вкладку, где они могут проверить резервирование.</span><span class="sxs-lookup"><span data-stu-id="71f8d-178">Selecting the notification will take the user to the tab, where they can check their reservation.</span></span>

#### <a name="request"></a><span data-ttu-id="71f8d-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="71f8d-179">Request</span></span>
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

#### <a name="response"></a><span data-ttu-id="71f8d-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="71f8d-180">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-3-notify-a-user-about-an-event-using-custom-topic"></a><span data-ttu-id="71f8d-181">Пример 3: уведомление пользователя о событии с помощью настраиваемого раздела</span><span class="sxs-lookup"><span data-stu-id="71f8d-181">Example 3: Notify a user about an event using custom topic</span></span>

<span data-ttu-id="71f8d-182">Как показано в предыдущих примерах, вы можете ссылаться на различные аспекты команды.</span><span class="sxs-lookup"><span data-stu-id="71f8d-182">As seen in the previous examples, you can link to different aspects of the team.</span></span> <span data-ttu-id="71f8d-183">Тем не менее, если вы хотите создать ссылку на аспект, не являющийся частью команды или не представленный в Microsoft Graph, или вы хотите изменить имя, вы можете задать `topic` для `text` него значение и передать его настраиваемое значение.</span><span class="sxs-lookup"><span data-stu-id="71f8d-183">However, if you want to link to an aspect that is not part of the team or is not represented by Microsoft Graph, or you want to customize the name, you can set the source of the `topic` to `text` and pass in a custom value for it.</span></span> <span data-ttu-id="71f8d-184">`webUrl` является обязательным, если задано значение `topic` source `text` .</span><span class="sxs-lookup"><span data-stu-id="71f8d-184">`webUrl` is required when setting `topic` source to `text`.</span></span>

#### <a name="request"></a><span data-ttu-id="71f8d-185">Запрос</span><span class="sxs-lookup"><span data-stu-id="71f8d-185">Request</span></span>
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

#### <a name="response"></a><span data-ttu-id="71f8d-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="71f8d-186">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```
