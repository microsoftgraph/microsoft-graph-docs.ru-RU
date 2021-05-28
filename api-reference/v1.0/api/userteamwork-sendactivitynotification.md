---
title: 'userTeamwork: sendActivityNotification'
description: Отправка уведомления о канале действий пользователю.
author: eddie-lee-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 2d6d82e251fd476dbaa0f657d887bac5fd475883
ms.sourcegitcommit: a9a035e7cf7b500aebe5477c05361552e7c3a7ab
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/28/2021
ms.locfileid: "52696270"
---
# <a name="userteamwork-sendactivitynotification"></a><span data-ttu-id="22aab-103">userTeamwork: sendActivityNotification</span><span class="sxs-lookup"><span data-stu-id="22aab-103">userTeamwork: sendActivityNotification</span></span>
<span data-ttu-id="22aab-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22aab-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="22aab-105">Отправка уведомления о канале действий пользователю.</span><span class="sxs-lookup"><span data-stu-id="22aab-105">Send an activity feed notification to a user.</span></span> <span data-ttu-id="22aab-106">Дополнительные сведения об отправке уведомлений и требованиях к этому см. в Teams [действия.](/graph/teams-send-activityfeednotifications)</span><span class="sxs-lookup"><span data-stu-id="22aab-106">For more details about sending notifications and the requirements for doing so, see [sending Teams activity notifications](/graph/teams-send-activityfeednotifications).</span></span>

## <a name="permissions"></a><span data-ttu-id="22aab-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="22aab-107">Permissions</span></span>
<span data-ttu-id="22aab-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22aab-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22aab-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="22aab-110">Permission type</span></span>|<span data-ttu-id="22aab-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="22aab-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22aab-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="22aab-112">Delegated (work or school account)</span></span>|<span data-ttu-id="22aab-113">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="22aab-113">TeamsActivity.Send</span></span>|
|<span data-ttu-id="22aab-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="22aab-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22aab-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22aab-115">Not Supported.</span></span>|
|<span data-ttu-id="22aab-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="22aab-116">Application</span></span>|<span data-ttu-id="22aab-117">TeamsActivity.Send</span><span class="sxs-lookup"><span data-stu-id="22aab-117">TeamsActivity.Send</span></span>|

## <a name="http-request"></a><span data-ttu-id="22aab-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="22aab-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{userId | user-principal-name}/teamwork/sendActivityNotification
```

## <a name="request-headers"></a><span data-ttu-id="22aab-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="22aab-119">Request headers</span></span>
|<span data-ttu-id="22aab-120">Имя</span><span class="sxs-lookup"><span data-stu-id="22aab-120">Name</span></span>|<span data-ttu-id="22aab-121">Описание</span><span class="sxs-lookup"><span data-stu-id="22aab-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="22aab-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="22aab-122">Authorization</span></span>|<span data-ttu-id="22aab-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="22aab-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="22aab-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="22aab-125">Content-Type</span></span>|<span data-ttu-id="22aab-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="22aab-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="22aab-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="22aab-128">Request body</span></span>
<span data-ttu-id="22aab-129">В тело запроса добавьте параметры в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="22aab-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="22aab-130">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="22aab-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="22aab-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="22aab-131">Parameter</span></span>|<span data-ttu-id="22aab-132">Тип</span><span class="sxs-lookup"><span data-stu-id="22aab-132">Type</span></span>|<span data-ttu-id="22aab-133">Описание</span><span class="sxs-lookup"><span data-stu-id="22aab-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22aab-134">topic</span><span class="sxs-lookup"><span data-stu-id="22aab-134">topic</span></span>|[<span data-ttu-id="22aab-135">teamworkActivityTopic</span><span class="sxs-lookup"><span data-stu-id="22aab-135">teamworkActivityTopic</span></span>](../resources/teamworkactivitytopic.md)|<span data-ttu-id="22aab-136">Тема уведомления.</span><span class="sxs-lookup"><span data-stu-id="22aab-136">Topic of the notification.</span></span> <span data-ttu-id="22aab-137">Указывает обсуждаемый ресурс.</span><span class="sxs-lookup"><span data-stu-id="22aab-137">Specifies the resource being talked about.</span></span>|
|<span data-ttu-id="22aab-138">activityType</span><span class="sxs-lookup"><span data-stu-id="22aab-138">activityType</span></span>|<span data-ttu-id="22aab-139">String</span><span class="sxs-lookup"><span data-stu-id="22aab-139">String</span></span>|<span data-ttu-id="22aab-140">Тип действия.</span><span class="sxs-lookup"><span data-stu-id="22aab-140">Activity type.</span></span> <span data-ttu-id="22aab-141">Это должно быть объявлено в [манифесте Teams приложения](/microsoftteams/platform/overview).</span><span class="sxs-lookup"><span data-stu-id="22aab-141">This must be declared in the [Teams app manifest](/microsoftteams/platform/overview).</span></span>|
|<span data-ttu-id="22aab-142">chainId</span><span class="sxs-lookup"><span data-stu-id="22aab-142">chainId</span></span>|<span data-ttu-id="22aab-143">Int64</span><span class="sxs-lookup"><span data-stu-id="22aab-143">Int64</span></span>|<span data-ttu-id="22aab-144">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="22aab-144">Optional.</span></span> <span data-ttu-id="22aab-145">Используется для переопределения предыдущего уведомления.</span><span class="sxs-lookup"><span data-stu-id="22aab-145">Used to override a previous notification.</span></span> <span data-ttu-id="22aab-146">Используйте то же `chainId` самое в последующих запросах для переопределения предыдущего уведомления.</span><span class="sxs-lookup"><span data-stu-id="22aab-146">Use the same `chainId` in subsequent requests to override the previous notification.</span></span>|
|<span data-ttu-id="22aab-147">previewText</span><span class="sxs-lookup"><span data-stu-id="22aab-147">previewText</span></span>|[<span data-ttu-id="22aab-148">itemBody</span><span class="sxs-lookup"><span data-stu-id="22aab-148">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="22aab-149">Предварительный текст уведомления.</span><span class="sxs-lookup"><span data-stu-id="22aab-149">Preview text for the notification.</span></span> <span data-ttu-id="22aab-150">Microsoft Teams только первые 150 символов.</span><span class="sxs-lookup"><span data-stu-id="22aab-150">Microsoft Teams will only show first 150 characters.</span></span>|
|<span data-ttu-id="22aab-151">templateParameters</span><span class="sxs-lookup"><span data-stu-id="22aab-151">templateParameters</span></span>|<span data-ttu-id="22aab-152">Коллекция [keyValuePair](../resources/keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="22aab-152">[keyValuePair](../resources/keyvaluepair.md) collection</span></span>|<span data-ttu-id="22aab-153">Значения переменных шаблонов, определенных в записи ленты действий, соответствующие манифесту `activityType` [Teams приложения.](/microsoftteams/platform/overview)</span><span class="sxs-lookup"><span data-stu-id="22aab-153">Values for template variables defined in the activity feed entry corresponding to `activityType` in [Teams app manifest](/microsoftteams/platform/overview).</span></span>|

<span data-ttu-id="22aab-154">При настройке значения свойства темы для следующих ресурсов `source` поддерживаются следующие  `entityUrl` ресурсы:</span><span class="sxs-lookup"><span data-stu-id="22aab-154">The following resources are supported when setting the `source` value of the **topic** property to `entityUrl`:</span></span>

- [<span data-ttu-id="22aab-155">teamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="22aab-155">teamsAppInstallation</span></span>](../resources/teamsappinstallation.md)
- [<span data-ttu-id="22aab-156">teamsCatalogApp</span><span class="sxs-lookup"><span data-stu-id="22aab-156">teamsCatalogApp</span></span>](../resources/teamscatalogapp.md)

## <a name="response"></a><span data-ttu-id="22aab-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="22aab-157">Response</span></span>

<span data-ttu-id="22aab-158">В случае успешного выполнения это действие возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="22aab-158">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="22aab-159">Примеры</span><span class="sxs-lookup"><span data-stu-id="22aab-159">Examples</span></span>

### <a name="example-1-send-notification-to-a-user-for-a-task-created"></a><span data-ttu-id="22aab-160">Пример 1. Отправка уведомления пользователю для задачи, созданной</span><span class="sxs-lookup"><span data-stu-id="22aab-160">Example 1: Send notification to a user for a task created</span></span>

#### <a name="request"></a><span data-ttu-id="22aab-161">Запрос</span><span class="sxs-lookup"><span data-stu-id="22aab-161">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="22aab-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="22aab-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "userteamwork_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/users/{userId}/teamwork/sendActivityNotification
Content-Type: application/json

{
    "topic": {
        "source": "entityUrl",
        "value": "https://graph.microsoft.com/v1.0/users/{userId}/teamwork/installedApps/{installationId}"
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
# <a name="c"></a>[<span data-ttu-id="22aab-163">C#</span><span class="sxs-lookup"><span data-stu-id="22aab-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/userteamwork-sendactivitynotification-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="22aab-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="22aab-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/userteamwork-sendactivitynotification-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="22aab-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="22aab-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/userteamwork-sendactivitynotification-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="22aab-166">Java</span><span class="sxs-lookup"><span data-stu-id="22aab-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/userteamwork-sendactivitynotification-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="22aab-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="22aab-167">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```

### <a name="example-2-notify-a-user-about-an-event-using-custom-topic"></a><span data-ttu-id="22aab-168">Пример 2. Уведомление пользователя о событии с использованием настраиваемой темы</span><span class="sxs-lookup"><span data-stu-id="22aab-168">Example 2: Notify a user about an event using custom topic</span></span>

<span data-ttu-id="22aab-169">Если вы хотите связать аспект, который не представлен корпорацией Майкрософт Graph или настроить имя, вы можете установить источник для него и передать его в настраиваемом `topic` `text` значении.</span><span class="sxs-lookup"><span data-stu-id="22aab-169">If you want to link an aspect that is not represented by Microsoft Graph, or you want to customize the name, you can set the source of the `topic` to `text` and pass in a custom value for it.</span></span> <span data-ttu-id="22aab-170">`webUrl` требуется при использовании `topic` источника в качестве `text` .</span><span class="sxs-lookup"><span data-stu-id="22aab-170">`webUrl` is required when using `topic` source as `text`.</span></span>

#### <a name="request"></a><span data-ttu-id="22aab-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="22aab-171">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="22aab-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="22aab-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "team_sendactivitynotification"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/users/{userId}/teamwork/sendActivityNotification
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
# <a name="c"></a>[<span data-ttu-id="22aab-173">C#</span><span class="sxs-lookup"><span data-stu-id="22aab-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/team-sendactivitynotification-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="22aab-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="22aab-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/team-sendactivitynotification-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="22aab-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="22aab-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/team-sendactivitynotification-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="22aab-176">Java</span><span class="sxs-lookup"><span data-stu-id="22aab-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/team-sendactivitynotification-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="22aab-177">Отклик</span><span class="sxs-lookup"><span data-stu-id="22aab-177">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
}
-->
``` http
HTTP/1.1 204 No Content
```
