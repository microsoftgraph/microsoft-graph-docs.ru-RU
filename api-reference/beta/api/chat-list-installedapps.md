---
title: Список приложений в каталоге
description: Список приложений, установленных в чате.
author: subray
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5e53e1218edd2fc994fb489461f7b782bb7a10a2
ms.sourcegitcommit: 99fdbd9a1806d64626423e1f39342dcde8a1eaf4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/16/2021
ms.locfileid: "52971316"
---
# <a name="list-apps-in-chat"></a><span data-ttu-id="abe25-103">Список приложений в каталоге</span><span class="sxs-lookup"><span data-stu-id="abe25-103">List apps in chat</span></span>

<span data-ttu-id="abe25-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="abe25-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="abe25-105">Список всех [установок приложений](../resources/teamsappinstallation.md) в [чате](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="abe25-105">List all [app installations](../resources/teamsappinstallation.md) within a [chat](../resources/chat.md).</span></span>

> <span data-ttu-id="abe25-106">**Примечание.** Если чат связан с экземпляром [onlineMeeting](../resources/onlinemeeting.md), объект **teamsApp**, установленный для собрания, будет отражаться в списке.</span><span class="sxs-lookup"><span data-stu-id="abe25-106">**Note**: If the chat is associated with an [onlineMeeting](../resources/onlinemeeting.md) instance, then, effectively, the **teamsApp** s installed in the meeting will be listed.</span></span>

> [!NOTE]
> <span data-ttu-id="abe25-107">`id`Ресурс **teamsAppInstallation** имеет не то же значение, что и `id` связанный ресурс **teamsApp**.</span><span class="sxs-lookup"><span data-stu-id="abe25-107">The `id` of a **teamsAppInstallation** resource is not the same value as the `id` of the associated **teamsApp** resource.</span></span>


## <a name="permissions"></a><span data-ttu-id="abe25-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="abe25-108">Permissions</span></span>

<span data-ttu-id="abe25-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="abe25-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abe25-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="abe25-111">Permission type</span></span>      | <span data-ttu-id="abe25-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="abe25-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="abe25-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="abe25-113">Delegated (work or school account)</span></span> | <span data-ttu-id="abe25-114">TeamsAppInstallation.ReadForChat, TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span><span class="sxs-lookup"><span data-stu-id="abe25-114">TeamsAppInstallation.ReadForChat, TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span></span> |
|<span data-ttu-id="abe25-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="abe25-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="abe25-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="abe25-116">Not supported.</span></span>    |
|<span data-ttu-id="abe25-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="abe25-117">Application</span></span> | <span data-ttu-id="abe25-118">TeamsAppInstallation.Read.Chat *, Chat.Manage.Chat*, TeamsAppInstallation.ReadForChat.All, TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span><span class="sxs-lookup"><span data-stu-id="abe25-118">TeamsAppInstallation.Read.Chat *, Chat.Manage.Chat*, TeamsAppInstallation.ReadForChat.All, TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span></span> |

> <span data-ttu-id="abe25-119">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов](https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="abe25-119">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

## <a name="http-request"></a><span data-ttu-id="abe25-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="abe25-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{chat-id}/installedApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="abe25-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="abe25-121">Optional query parameters</span></span>

<span data-ttu-id="abe25-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$filter`, `$select` и `$expand` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="abe25-122">This method supports the `$filter`, `$select`, and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="abe25-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="abe25-123">Request headers</span></span>

| <span data-ttu-id="abe25-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="abe25-124">Header</span></span>       | <span data-ttu-id="abe25-125">Значение</span><span class="sxs-lookup"><span data-stu-id="abe25-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="abe25-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="abe25-126">Authorization</span></span>  | <span data-ttu-id="abe25-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="abe25-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="abe25-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="abe25-129">Request body</span></span>

<span data-ttu-id="abe25-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="abe25-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="abe25-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="abe25-131">Response</span></span>

<span data-ttu-id="abe25-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [teamsAppInstallation](../resources/teamsappinstallation.md) в тексте сообщения.</span><span class="sxs-lookup"><span data-stu-id="abe25-132">If successful, this method returns a `200 OK` response code and a collection of [teamsAppInstallation](../resources/teamsappinstallation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="abe25-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="abe25-133">Examples</span></span>

### <a name="example-1-get-all-the-apps-installed-in-the-specified-chat"></a><span data-ttu-id="abe25-134">Пример 1: Получение всех приложений, установленных в указанном чате</span><span class="sxs-lookup"><span data-stu-id="abe25-134">Example 1: Get all the apps installed in the specified chat</span></span>

#### <a name="request"></a><span data-ttu-id="abe25-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="abe25-135">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="abe25-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="abe25-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_installed_apps_in_chat"
}
-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/19%3Ad65713bc498c4a428c71ef9353e6ce20%40thread.v2/installedApps
```
# <a name="c"></a>[<span data-ttu-id="abe25-137">C#</span><span class="sxs-lookup"><span data-stu-id="abe25-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-installed-apps-in-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="abe25-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="abe25-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-installed-apps-in-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="abe25-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="abe25-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-installed-apps-in-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="abe25-140">Java</span><span class="sxs-lookup"><span data-stu-id="abe25-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-installed-apps-in-chat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="abe25-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="abe25-141">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.teamsAppInstallation)"
}
-->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats('19%3Ad65713bc498c4a428c71ef9353e6ce20%40thread.v2')/installedApps",
    "value": [
        {
            "id": "MTk6ZDY1NzEzYmM0OThjNGE0MjhjNzFlZjkzNTNlNmNlMjBAdGhyZWFkLnYyIyMwMDAwMTAxNi1kZTA1LTQ5MmUtOTEwNi00ODI4ZmM4YTg2ODc="
        },
        {
            "id": "MTk6ZDY1NzEzYmM0OThjNGE0MjhjNzFlZjkzNTNlNmNlMjBAdGhyZWFkLnYyIyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg="
        },
        {
            "id": "MTk6ZDY1NzEzYmM0OThjNGE0MjhjNzFlZjkzNTNlNmNlMjBAdGhyZWFkLnYyIyMxYzQzNDBkZS0yYTg1LTQwZTUtOGViMC00ZjI5NTM2ODk3OGI="
        }
  ]
}
```

### <a name="example-2-get-the-names-and-other-details-of-apps-installed-in-the-specified-chat"></a><span data-ttu-id="abe25-142">Пример 2: Получение имен и других сведений о приложениях, установленных в указанном чате</span><span class="sxs-lookup"><span data-stu-id="abe25-142">Example 2: Get the names and other details of apps installed in the specified chat</span></span>

<span data-ttu-id="abe25-143">В следующем примере, если с экземпляром установленного приложения связан [бот](../resources/teamworkbot.md), сведения о нем также возвращаются.</span><span class="sxs-lookup"><span data-stu-id="abe25-143">In the following example, if an instance of an installed app has a [bot](../resources/teamworkbot.md) associated with it, then the details of the bot are returned as well.</span></span>

#### <a name="request"></a><span data-ttu-id="abe25-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="abe25-144">Request</span></span>


<!-- {
  "blockType": "request",
  "name": "list_installed_apps_in_chat_expand"
}
-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/19%3Ad65713bc498c4a428c71ef9353e6ce20%40thread.v2/installedApps?$expand=teamsAppDefinition($expand=bot)
```

#### <a name="response"></a><span data-ttu-id="abe25-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="abe25-145">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.teamsAppInstallation)"
}
-->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats('19%3Ad65713bc498c4a428c71ef9353e6ce20%40thread.v2')/installedApps(teamsAppDefinition())",
    "value": [
        {
            "id": "MTk6ZDY1NzEzYmM0OThjNGE0MjhjNzFlZjkzNTNlNmNlMjBAdGhyZWFkLnYyIyMwMDAwMTAxNi1kZTA1LTQ5MmUtOTEwNi00ODI4ZmM4YTg2ODc=",
            "teamsAppDefinition": {
                "id": "MDAwMDEwMTYtZGUwNS00OTJlLTkxMDYtNDgyOGZjOGE4Njg3IyMxLjAuMiMjUHVibGlzaGVk",
                "teamsAppId": "00001016-de05-492e-9106-4828fc8a8687",
                "azureADAppId": "7df0a125-d3be-4c96-aa54-591f83ff541c",
                "displayName": "Power Automate Actions",
                "version": "1.0.2",
                "requiredResourceSpecificApplicationPermissions": [],
                "publishingState": "published",
                "shortdescription": "Be more productive with Microsoft Flow",
                "description": "Automate time-consuming and repetitive tasks by integrating your favorite apps and services with Microsoft Power Automate.",
                "lastModifiedDateTime": null,
                "createdBy": null,
                "bot": {
                    "id":"9a58a3ec-6b68-4818-ac11-844f1c326784"
                }
            }
        },
        {
            "id": "MTk6ZDY1NzEzYmM0OThjNGE0MjhjNzFlZjkzNTNlNmNlMjBAdGhyZWFkLnYyIyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg=",
            "teamsAppDefinition": {
                "id": "MGQ4MjBlY2QtZGVmMi00Mjk3LWFkYWQtNzgwNTZjZGU3Yzc4IyMxLjAuMCMjUHVibGlzaGVk",
                "teamsAppId": "0d820ecd-def2-4297-adad-78056cde7c78",
                "azureADAppId": "2d4d3d8e-2be3-4bef-9f87-7875a61c29de",
                "displayName": "OneNote",
                "version": "1.0.0",
                "requiredResourceSpecificApplicationPermissions": [],
                "publishingState": "published",
                "shortdescription": "Capture and share ideas, to-do lists and other notes with your team.",
                "description": "Capture and share ideas, to-do lists and other thoughts with your team. You can also co-author anytime.",
                "lastModifiedDateTime": null,
                "createdBy": null
            }
        },
        {
            "id": "MTk6ZDY1NzEzYmM0OThjNGE0MjhjNzFlZjkzNTNlNmNlMjBAdGhyZWFkLnYyIyMxYzQzNDBkZS0yYTg1LTQwZTUtOGViMC00ZjI5NTM2ODk3OGI=",
            "teamsAppDefinition": {
                "id": "MWM0MzQwZGUtMmE4NS00MGU1LThlYjAtNGYyOTUzNjg5NzhiIyMxLjMjI1B1Ymxpc2hlZA==",
                "teamsAppId": "1c4340de-2a85-40e5-8eb0-4f295368978b",
                "azureADAppId": null,
                "displayName": "Power BI",
                "version": "1.3",
                "requiredResourceSpecificApplicationPermissions": [],
                "publishingState": "published",
                "shortdescription": "Easily see and chat about Power BI reports",
                "description": "Pin Power BI reports to your channel to start a conversation about your data. With reports and chats in the same place, everyone stays on the same page.",
                "lastModifiedDateTime": null,
                "createdBy": null
            }
        }
  ]
}
```

### <a name="example-3-get-the-app-installation-resource-based-on-the-manifest-id-of-the-associated-app"></a><span data-ttu-id="abe25-146">Пример 3: Получение ресурса установки приложения на основе идентификатора манифеста связанного приложения</span><span class="sxs-lookup"><span data-stu-id="abe25-146">Example 3: Get the app installation resource based on the manifest id of the associated app</span></span>

#### <a name="request"></a><span data-ttu-id="abe25-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="abe25-147">Request</span></span>

<span data-ttu-id="abe25-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="abe25-148">The following is an example of the request.</span></span> <span data-ttu-id="abe25-149">В этом примере идентификатор манифеста приложения Teams — 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'.</span><span class="sxs-lookup"><span data-stu-id="abe25-149">In the example, the manifest ID of the Teams app is 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'.</span></span>

# <a name="http"></a>[<span data-ttu-id="abe25-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="abe25-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_installed_apps_in_chat_expand_filter"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/19%3Ad65713bc498c4a428c71ef9353e6ce20%40thread.v2/installedApps?$expand=teamsApp,teamsAppDefinition&$filter=teamsApp/externalId eq 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'
```
# <a name="c"></a>[<span data-ttu-id="abe25-151">C#</span><span class="sxs-lookup"><span data-stu-id="abe25-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-installed-apps-in-chat-expand-filter-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="abe25-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="abe25-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-installed-apps-in-chat-expand-filter-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="abe25-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="abe25-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-installed-apps-in-chat-expand-filter-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="abe25-154">Java</span><span class="sxs-lookup"><span data-stu-id="abe25-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-installed-apps-in-chat-expand-filter-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="abe25-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="abe25-155">Response</span></span>

<span data-ttu-id="abe25-156">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="abe25-156">The following is an example of the response.</span></span>

><span data-ttu-id="abe25-157">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="abe25-157">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "name": "list_installed_apps_in_chat_expand_filter",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.count": 1,
    "value": [
        {
            "id": "NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwMjQwYTM2OC0yNWUwLTQ1NjktOGViZS0xMzYwMWNiNTVhMTg=",
            "teamsApp": {
                "id": "0240a368-25e0-4569-8ebe-13601cb55a18",
                "externalId": "cf1ba4c7-f94e-4d80-ba90-5594b641a8ee",
                "displayName": "YPA",
                "distributionMethod": "sideloaded"
            },
            "teamsAppDefinition": {
                "id": "MDI0MGEzNjgtMjVlMC00NTY5LThlYmUtMTM2MDFjYjU1YTE4IyM2LjAuMA==",
                "teamsAppId": "0240a368-25e0-4569-8ebe-13601cb55a18",
                "azureADAppId": "9fc97ea2-c417-4c76-a2db-197612067b28",
                "displayName": "YPA",
                "version": "6.0.0",
                "requiredResourceSpecificApplicationPermissions": [
                ],
                "publishingState": "published",
                "shortdescription": "A conversational smart assistant from MSX that surfaces real-time insights.",
                "description": "For MSX Users: A conversational role-based smart assistant that will enable Enterprise sellers (AE, ATS, SSP, TSP) to be more productive by surfacing real-time insights, recommendations, actions and notifications, and by automating repetitive tasks.",
                "lastModifiedDateTime": null,
                "createdBy": null
            }
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="abe25-158">Дополнительные материалы</span><span class="sxs-lookup"><span data-stu-id="abe25-158">See also</span></span>
- [<span data-ttu-id="abe25-159">Список приложений в каталоге</span><span class="sxs-lookup"><span data-stu-id="abe25-159">List apps in catalog</span></span>](appcatalogs-list-teamsapps.md)
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chat list installedapps",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
