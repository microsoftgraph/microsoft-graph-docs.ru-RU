---
title: 'userTeamwork: sendActivityNotification'
description: Отправьте пользователю уведомление веб-канала активности.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1c28aa329299597e40d856b81e569a734f1b068c
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/19/2020
ms.locfileid: "49719771"
---
# <a name="userteamwork-sendactivitynotification"></a><span data-ttu-id="c1073-103">userTeamwork: sendActivityNotification</span><span class="sxs-lookup"><span data-stu-id="c1073-103">userTeamwork: sendActivityNotification</span></span>
<span data-ttu-id="c1073-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1073-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c1073-105">Отправьте пользователю уведомление веб-канала активности.</span><span class="sxs-lookup"><span data-stu-id="c1073-105">Send an activity feed notification to a user.</span></span> <span data-ttu-id="c1073-106">Дополнительные сведения об отправке уведомлений и требованиях для этого см. в отправке уведомлений [о действиях Teams.](/graph/teams-send-activityfeednotifications)</span><span class="sxs-lookup"><span data-stu-id="c1073-106">For more details about sending notifications and the requirements for doing so, see [sending Teams activity notifications](/graph/teams-send-activityfeednotifications).</span></span>

## <a name="permissions"></a><span data-ttu-id="c1073-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c1073-107">Permissions</span></span>
<span data-ttu-id="c1073-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1073-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1073-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c1073-110">Permission type</span></span>|<span data-ttu-id="c1073-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c1073-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1073-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c1073-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c1073-113">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="c1073-113">TeamsActivity.Send</span></span>|
|<span data-ttu-id="c1073-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c1073-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1073-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1073-115">Not Supported.</span></span>|
|<span data-ttu-id="c1073-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="c1073-116">Application</span></span>|<span data-ttu-id="c1073-117">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="c1073-117">TeamsActivity.Send</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1073-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c1073-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{userId}/teamwork/sendActivityNotification
```

## <a name="request-headers"></a><span data-ttu-id="c1073-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c1073-119">Request headers</span></span>
|<span data-ttu-id="c1073-120">Имя</span><span class="sxs-lookup"><span data-stu-id="c1073-120">Name</span></span>|<span data-ttu-id="c1073-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c1073-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c1073-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c1073-122">Authorization</span></span>|<span data-ttu-id="c1073-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c1073-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c1073-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c1073-125">Content-Type</span></span>|<span data-ttu-id="c1073-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c1073-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1073-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c1073-128">Request body</span></span>
<span data-ttu-id="c1073-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c1073-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c1073-130">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="c1073-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c1073-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="c1073-131">Parameter</span></span>|<span data-ttu-id="c1073-132">Тип</span><span class="sxs-lookup"><span data-stu-id="c1073-132">Type</span></span>|<span data-ttu-id="c1073-133">Описание</span><span class="sxs-lookup"><span data-stu-id="c1073-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1073-134">topic</span><span class="sxs-lookup"><span data-stu-id="c1073-134">topic</span></span>|[<span data-ttu-id="c1073-135">teamworkActivityTopic</span><span class="sxs-lookup"><span data-stu-id="c1073-135">teamworkActivityTopic</span></span>](../resources/teamworkactivitytopic.md)|<span data-ttu-id="c1073-136">Тема уведомления.</span><span class="sxs-lookup"><span data-stu-id="c1073-136">Topic of the notification.</span></span> <span data-ttu-id="c1073-137">Указывает ресурс, о который идет речь.</span><span class="sxs-lookup"><span data-stu-id="c1073-137">Specifies the resource being talked about.</span></span>|
|<span data-ttu-id="c1073-138">activityType</span><span class="sxs-lookup"><span data-stu-id="c1073-138">activityType</span></span>|<span data-ttu-id="c1073-139">String</span><span class="sxs-lookup"><span data-stu-id="c1073-139">String</span></span>|<span data-ttu-id="c1073-140">Тип действия.</span><span class="sxs-lookup"><span data-stu-id="c1073-140">Activity type.</span></span> <span data-ttu-id="c1073-141">Это должно быть объявлено в [манифесте приложения Teams.](/microsoftteams/platform/overview)</span><span class="sxs-lookup"><span data-stu-id="c1073-141">This must be declared in the [Teams app manifest](/microsoftteams/platform/overview).</span></span>|
|<span data-ttu-id="c1073-142">chainId</span><span class="sxs-lookup"><span data-stu-id="c1073-142">chainId</span></span>|<span data-ttu-id="c1073-143">Int64</span><span class="sxs-lookup"><span data-stu-id="c1073-143">Int64</span></span>|<span data-ttu-id="c1073-144">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="c1073-144">Optional.</span></span> <span data-ttu-id="c1073-145">Используется для переопределения предыдущего уведомления.</span><span class="sxs-lookup"><span data-stu-id="c1073-145">Used to override a previous notification.</span></span> <span data-ttu-id="c1073-146">Используйте то же самое `chainId` в последующих запросах для переопределения предыдущего уведомления.</span><span class="sxs-lookup"><span data-stu-id="c1073-146">Use the same `chainId` in subsequent requests to override the previous notification.</span></span>|
|<span data-ttu-id="c1073-147">previewText</span><span class="sxs-lookup"><span data-stu-id="c1073-147">previewText</span></span>|[<span data-ttu-id="c1073-148">itemBody</span><span class="sxs-lookup"><span data-stu-id="c1073-148">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="c1073-149">Предварительный просмотр текста уведомления.</span><span class="sxs-lookup"><span data-stu-id="c1073-149">Preview text for the notification.</span></span> <span data-ttu-id="c1073-150">Microsoft Teams будет показывать только первые 150 символов.</span><span class="sxs-lookup"><span data-stu-id="c1073-150">Microsoft Teams will only show first 150 characters.</span></span>|
|<span data-ttu-id="c1073-151">templateParameters</span><span class="sxs-lookup"><span data-stu-id="c1073-151">templateParameters</span></span>|<span data-ttu-id="c1073-152">Коллекция [keyValuePair](../resources/keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="c1073-152">[keyValuePair](../resources/keyvaluepair.md) collection</span></span>|<span data-ttu-id="c1073-153">Значения переменных шаблона, определенных в записи веб-канала активности, соответствующей `activityType` [манифесту приложения Teams.](/microsoftteams/platform/overview)</span><span class="sxs-lookup"><span data-stu-id="c1073-153">Values for template variables defined in the activity feed entry corresponding to `activityType` in [Teams app manifest](/microsoftteams/platform/overview).</span></span>|

<span data-ttu-id="c1073-154">Следующие ресурсы поддерживаются при установке для свойства `source` **темы** значения `entityUrl` :</span><span class="sxs-lookup"><span data-stu-id="c1073-154">The following resources are supported when setting the `source` value of the **topic** property to `entityUrl`:</span></span>

- [<span data-ttu-id="c1073-155">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="c1073-155">teamsAppInstallation</span></span>](../resources/teamsappinstallation.md)
- [<span data-ttu-id="c1073-156">teamsCatalogApp</span><span class="sxs-lookup"><span data-stu-id="c1073-156">teamsCatalogApp</span></span>](../resources/teamscatalogapp.md)

## <a name="response"></a><span data-ttu-id="c1073-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="c1073-157">Response</span></span>

<span data-ttu-id="c1073-158">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c1073-158">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="c1073-159">Примеры</span><span class="sxs-lookup"><span data-stu-id="c1073-159">Examples</span></span>

### <a name="example-1-send-notification-to-a-user-for-a-task-created"></a><span data-ttu-id="c1073-160">Пример 1. Отправка уведомления пользователю о созданной задаче</span><span class="sxs-lookup"><span data-stu-id="c1073-160">Example 1: Send notification to a user for a task created</span></span>

#### <a name="request"></a><span data-ttu-id="c1073-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1073-161">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c1073-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="c1073-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "userteamwork_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/beta/users/{userId}/teamwork/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/beta/users/{userId}/teamwork/installedApps/{installationId}"
    },
    "activityType": "taskCreated",
    "previewText": {
        "content": "New Task Created"
    },
    "templateParameters": [
        {
            "name": "taskId",
            "value": "Task 12322"
        }
    ]
}

```
# <a name="c"></a>[<span data-ttu-id="c1073-163">C#</span><span class="sxs-lookup"><span data-stu-id="c1073-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/userteamwork-sendactivitynotification-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c1073-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1073-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/userteamwork-sendactivitynotification-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c1073-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c1073-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/userteamwork-sendactivitynotification-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c1073-166">Java</span><span class="sxs-lookup"><span data-stu-id="c1073-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/userteamwork-sendactivitynotification-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c1073-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1073-167">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-notify-a-user-about-an-event-using-custom-topic"></a><span data-ttu-id="c1073-168">Пример 2. Уведомление пользователя о событии с помощью настраиваемой темы</span><span class="sxs-lookup"><span data-stu-id="c1073-168">Example 2: Notify a user about an event using custom topic</span></span>

<span data-ttu-id="c1073-169">Если вы хотите связать аспект, который не представлен Microsoft Graph, или настроить имя, можно установить источник и передать для него пользовательское `topic` `text` значение.</span><span class="sxs-lookup"><span data-stu-id="c1073-169">If you want to link an aspect that is not represented by Microsoft Graph, or you want to customize the name, you can set the source of the `topic` to `text` and pass in a custom value for it.</span></span> <span data-ttu-id="c1073-170">`webUrl` требуется при использовании источника `topic` в качестве `text` .</span><span class="sxs-lookup"><span data-stu-id="c1073-170">`webUrl` is required when using `topic` source as `text`.</span></span>

#### <a name="request"></a><span data-ttu-id="c1073-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1073-171">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c1073-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="c1073-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/beta/users/{userId}/teamwork/sendActivityNotification
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
    "templateParameters": [
        {
            "name": "deploymentId",
            "value": "6788662"
        }
    ]
}
```
# <a name="javascript"></a>[<span data-ttu-id="c1073-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1073-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/team-sendactivitynotification-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c1073-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="c1073-174">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```
