---
title: 'команда: sendActivityNotification'
description: Отправьте уведомление о канале действий в области группы.
author: eddie-lee-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0473e199d7a8cf5bb6dc10a3199240450021c8b6
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51474036"
---
# <a name="team-sendactivitynotification"></a><span data-ttu-id="f9e1e-103">команда: sendActivityNotification</span><span class="sxs-lookup"><span data-stu-id="f9e1e-103">team: sendActivityNotification</span></span>
<span data-ttu-id="f9e1e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9e1e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f9e1e-105">Отправьте уведомление о канале действий в области группы.</span><span class="sxs-lookup"><span data-stu-id="f9e1e-105">Send an activity feed notification in the scope of a team.</span></span> <span data-ttu-id="f9e1e-106">Дополнительные сведения об отправке уведомлений и требованиях к этому см. в материале Отправка уведомлений о [действиях Teams.](/graph/teams-send-activityfeednotifications)</span><span class="sxs-lookup"><span data-stu-id="f9e1e-106">For more details about sending notifications and the requirements for doing so, see [sending Teams activity notifications](/graph/teams-send-activityfeednotifications).</span></span>

## <a name="permissions"></a><span data-ttu-id="f9e1e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f9e1e-107">Permissions</span></span>
<span data-ttu-id="f9e1e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f9e1e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9e1e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f9e1e-110">Permission type</span></span>|<span data-ttu-id="f9e1e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f9e1e-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9e1e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f9e1e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f9e1e-113">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="f9e1e-113">TeamsActivity.Send</span></span>|
|<span data-ttu-id="f9e1e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f9e1e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9e1e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9e1e-115">Not Supported.</span></span>|
|<span data-ttu-id="f9e1e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f9e1e-116">Application</span></span>|<span data-ttu-id="f9e1e-117">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="f9e1e-117">TeamsActivity.Send</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9e1e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f9e1e-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /teams/{teamId}/sendActivityNotification
```

## <a name="request-headers"></a><span data-ttu-id="f9e1e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f9e1e-119">Request headers</span></span>
|<span data-ttu-id="f9e1e-120">Имя</span><span class="sxs-lookup"><span data-stu-id="f9e1e-120">Name</span></span>|<span data-ttu-id="f9e1e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="f9e1e-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f9e1e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f9e1e-122">Authorization</span></span>|<span data-ttu-id="f9e1e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f9e1e-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f9e1e-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f9e1e-125">Content-Type</span></span>|<span data-ttu-id="f9e1e-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f9e1e-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9e1e-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f9e1e-128">Request body</span></span>
<span data-ttu-id="f9e1e-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f9e1e-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="f9e1e-130">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="f9e1e-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="f9e1e-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="f9e1e-131">Parameter</span></span>|<span data-ttu-id="f9e1e-132">Тип</span><span class="sxs-lookup"><span data-stu-id="f9e1e-132">Type</span></span>|<span data-ttu-id="f9e1e-133">Описание</span><span class="sxs-lookup"><span data-stu-id="f9e1e-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9e1e-134">topic</span><span class="sxs-lookup"><span data-stu-id="f9e1e-134">topic</span></span>|[<span data-ttu-id="f9e1e-135">teamworkActivityTopic</span><span class="sxs-lookup"><span data-stu-id="f9e1e-135">teamworkActivityTopic</span></span>](../resources/teamworkactivitytopic.md)|<span data-ttu-id="f9e1e-136">Тема уведомления.</span><span class="sxs-lookup"><span data-stu-id="f9e1e-136">Topic of the notification.</span></span> <span data-ttu-id="f9e1e-137">Указывает обсуждаемый ресурс.</span><span class="sxs-lookup"><span data-stu-id="f9e1e-137">Specifies the resource being talked about.</span></span>|
|<span data-ttu-id="f9e1e-138">activityType</span><span class="sxs-lookup"><span data-stu-id="f9e1e-138">activityType</span></span>|<span data-ttu-id="f9e1e-139">String</span><span class="sxs-lookup"><span data-stu-id="f9e1e-139">String</span></span>|<span data-ttu-id="f9e1e-140">Тип действия.</span><span class="sxs-lookup"><span data-stu-id="f9e1e-140">Activity type.</span></span> <span data-ttu-id="f9e1e-141">Это должно быть объявлено в [манифесте приложения Teams.](/microsoftteams/platform/overview)</span><span class="sxs-lookup"><span data-stu-id="f9e1e-141">This must be declared in the [Teams app manifest](/microsoftteams/platform/overview).</span></span>|
|<span data-ttu-id="f9e1e-142">chainId</span><span class="sxs-lookup"><span data-stu-id="f9e1e-142">chainId</span></span>|<span data-ttu-id="f9e1e-143">Int64</span><span class="sxs-lookup"><span data-stu-id="f9e1e-143">Int64</span></span>|<span data-ttu-id="f9e1e-144">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="f9e1e-144">Optional.</span></span> <span data-ttu-id="f9e1e-145">Используется для переопределения предыдущего уведомления.</span><span class="sxs-lookup"><span data-stu-id="f9e1e-145">Used to override a previous notification.</span></span> <span data-ttu-id="f9e1e-146">Используйте то же `chainId` самое в последующих запросах для переопределения предыдущего уведомления.</span><span class="sxs-lookup"><span data-stu-id="f9e1e-146">Use the same `chainId` in subsequent requests to override the previous notification.</span></span>|
|<span data-ttu-id="f9e1e-147">previewText</span><span class="sxs-lookup"><span data-stu-id="f9e1e-147">previewText</span></span>|[<span data-ttu-id="f9e1e-148">itemBody</span><span class="sxs-lookup"><span data-stu-id="f9e1e-148">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="f9e1e-149">Предварительный текст уведомления.</span><span class="sxs-lookup"><span data-stu-id="f9e1e-149">Preview text for the notification.</span></span> <span data-ttu-id="f9e1e-150">Microsoft Teams покажет только первые 150 символов.</span><span class="sxs-lookup"><span data-stu-id="f9e1e-150">Microsoft Teams will only show first 150 characters.</span></span>|
|<span data-ttu-id="f9e1e-151">templateParameters</span><span class="sxs-lookup"><span data-stu-id="f9e1e-151">templateParameters</span></span>|<span data-ttu-id="f9e1e-152">Коллекция [keyValuePair](../resources/keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="f9e1e-152">[keyValuePair](../resources/keyvaluepair.md) collection</span></span>|<span data-ttu-id="f9e1e-153">Значения для переменных шаблонов, определенных в записи ленты действий, соответствующие `activityType` [манифесту приложения Teams.](/microsoftteams/platform/overview)</span><span class="sxs-lookup"><span data-stu-id="f9e1e-153">Values for template variables defined in the activity feed entry corresponding to `activityType` in [Teams app manifest](/microsoftteams/platform/overview).</span></span>|
|<span data-ttu-id="f9e1e-154">получатель;</span><span class="sxs-lookup"><span data-stu-id="f9e1e-154">recipient</span></span>|[<span data-ttu-id="f9e1e-155">teamworkNotificationRecipient</span><span class="sxs-lookup"><span data-stu-id="f9e1e-155">teamworkNotificationRecipient</span></span>](../resources/teamworknotificationrecipient.md)|<span data-ttu-id="f9e1e-156">Получатель уведомления.</span><span class="sxs-lookup"><span data-stu-id="f9e1e-156">Recipient of the notification.</span></span> <span data-ttu-id="f9e1e-157">Поддерживаются только пользователи Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f9e1e-157">Only Azure AD users are supported.</span></span> <span data-ttu-id="f9e1e-158">См. [также aadUserNotificationRecipient](../resources/aadusernotificationrecipient.md).</span><span class="sxs-lookup"><span data-stu-id="f9e1e-158">See also [aadUserNotificationRecipient](../resources/aadusernotificationrecipient.md).</span></span> |

<span data-ttu-id="f9e1e-159">При настройке значения свойства темы для следующих ресурсов `source` поддерживаются следующие  `entityUrl` ресурсы:</span><span class="sxs-lookup"><span data-stu-id="f9e1e-159">The following resources are supported when setting the `source` value of the **topic** property to `entityUrl`:</span></span>

- [<span data-ttu-id="f9e1e-160">team</span><span class="sxs-lookup"><span data-stu-id="f9e1e-160">team</span></span>](../resources/team.md)
- [<span data-ttu-id="f9e1e-161">channel</span><span class="sxs-lookup"><span data-stu-id="f9e1e-161">channel</span></span>](../resources/channel.md)
- [<span data-ttu-id="f9e1e-162">chatMesage</span><span class="sxs-lookup"><span data-stu-id="f9e1e-162">chatMesage</span></span>](../resources/chatmessage.md)
- [<span data-ttu-id="f9e1e-163">teamsTab</span><span class="sxs-lookup"><span data-stu-id="f9e1e-163">teamsTab</span></span>](../resources/teamstab.md)

> <span data-ttu-id="f9e1e-164">**Примечание:** URL-адрес объекта должен быть одним и тем же или детским ресурсом группы в URL-адресе.</span><span class="sxs-lookup"><span data-stu-id="f9e1e-164">**Note:** The entity URL must be same or child resource of the team in the URL.</span></span> <span data-ttu-id="f9e1e-165">Кроме того, приложение [Teams должно](/microsoftteams/platform/overview) быть установлено в команде.</span><span class="sxs-lookup"><span data-stu-id="f9e1e-165">Additionally, the [Teams app](/microsoftteams/platform/overview) must be installed in the team.</span></span>

## <a name="response"></a><span data-ttu-id="f9e1e-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="f9e1e-166">Response</span></span>

<span data-ttu-id="f9e1e-167">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f9e1e-167">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="f9e1e-168">Примеры</span><span class="sxs-lookup"><span data-stu-id="f9e1e-168">Examples</span></span>

### <a name="example-1-notify-a-user-about-pending-finance-approval-requests"></a><span data-ttu-id="f9e1e-169">Пример 1. Уведомление пользователя о ожидающих запросах на утверждение финансирования</span><span class="sxs-lookup"><span data-stu-id="f9e1e-169">Example 1: Notify a user about pending finance approval requests</span></span>

<span data-ttu-id="f9e1e-170">В этом примере показано, как можно отправить уведомление о канале действий для группы.</span><span class="sxs-lookup"><span data-stu-id="f9e1e-170">This example shows how you can send an activity feed notification for a team.</span></span> <span data-ttu-id="f9e1e-171">В этом примере владелец группы сообщает о ожидающих запросах на утверждение финансирования.</span><span class="sxs-lookup"><span data-stu-id="f9e1e-171">This example notifies the team owner about pending finance approval requests.</span></span>

#### <a name="request"></a><span data-ttu-id="f9e1e-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="f9e1e-172">Request</span></span>

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


---


#### <a name="response"></a><span data-ttu-id="f9e1e-173">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9e1e-173">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-notify-a-user-about-a-channel-tab"></a><span data-ttu-id="f9e1e-174">Пример 2. Уведомление пользователя о вкладке канала</span><span class="sxs-lookup"><span data-stu-id="f9e1e-174">Example 2: Notify a user about a channel tab</span></span>

<span data-ttu-id="f9e1e-175">Как и в предыдущем примере, в этом примере `entityUrl` используется `topic` для .</span><span class="sxs-lookup"><span data-stu-id="f9e1e-175">Similar to the previous example, this example uses `entityUrl` for the `topic`.</span></span> <span data-ttu-id="f9e1e-176">Однако в этом примере ссылки на [вкладку](../resources/teamstab.md) в [канале](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="f9e1e-176">However, this example links to a [tab](../resources/teamstab.md) in a [channel](../resources/channel.md).</span></span> <span data-ttu-id="f9e1e-177">На вкладке размещена страница, показывающая пользователю состояние бронирования в отеле.</span><span class="sxs-lookup"><span data-stu-id="f9e1e-177">The tab hosts a page showing the user the status of their hotel reservation.</span></span> <span data-ttu-id="f9e1e-178">Выбор уведомления будет принимать пользователя на вкладке, где он может проверить свое бронирование.</span><span class="sxs-lookup"><span data-stu-id="f9e1e-178">Selecting the notification will take the user to the tab, where they can check their reservation.</span></span>

#### <a name="request"></a><span data-ttu-id="f9e1e-179">Запрос</span><span class="sxs-lookup"><span data-stu-id="f9e1e-179">Request</span></span>
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

#### <a name="response"></a><span data-ttu-id="f9e1e-180">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9e1e-180">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-3-notify-a-user-about-an-event-using-custom-topic"></a><span data-ttu-id="f9e1e-181">Пример 3. Уведомление пользователя о событии с использованием настраиваемой темы</span><span class="sxs-lookup"><span data-stu-id="f9e1e-181">Example 3: Notify a user about an event using custom topic</span></span>

<span data-ttu-id="f9e1e-182">Как повествуют в предыдущих примерах, вы можете ссылаться на различные аспекты команды.</span><span class="sxs-lookup"><span data-stu-id="f9e1e-182">As seen in the previous examples, you can link to different aspects of the team.</span></span> <span data-ttu-id="f9e1e-183">Однако, если вы хотите связаться с аспектом, который не является частью команды или не представлен Microsoft Graph, или вы хотите настроить имя, вы можете установить источник и передать в настраиваемом значении для `topic` `text` него.</span><span class="sxs-lookup"><span data-stu-id="f9e1e-183">However, if you want to link to an aspect that is not part of the team or is not represented by Microsoft Graph, or you want to customize the name, you can set the source of the `topic` to `text` and pass in a custom value for it.</span></span> <span data-ttu-id="f9e1e-184">`webUrl` требуется при настройке `topic` источника `text` для .</span><span class="sxs-lookup"><span data-stu-id="f9e1e-184">`webUrl` is required when setting `topic` source to `text`.</span></span>

#### <a name="request"></a><span data-ttu-id="f9e1e-185">Запрос</span><span class="sxs-lookup"><span data-stu-id="f9e1e-185">Request</span></span>
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

#### <a name="response"></a><span data-ttu-id="f9e1e-186">Отклик</span><span class="sxs-lookup"><span data-stu-id="f9e1e-186">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```
