---
title: Список приложений в каталоге
description: Список приложений, установленных в чате.
author: subray
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3a277c2c9d3e78243fa640ff95d3047f9df2d542
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50958543"
---
# <a name="list-apps-in-chat"></a><span data-ttu-id="3a1f1-103">Список приложений в каталоге</span><span class="sxs-lookup"><span data-stu-id="3a1f1-103">List apps in chat</span></span>

<span data-ttu-id="3a1f1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a1f1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3a1f1-105">Список всех [установок приложений](../resources/teamsappinstallation.md) в [чате](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="3a1f1-105">List all [app installations](../resources/teamsappinstallation.md) within a [chat](../resources/chat.md).</span></span>

> <span data-ttu-id="3a1f1-106">**Примечание.** Если чат связан с экземпляром [onlineMeeting](../resources/onlinemeeting.md), объект **teamsApp**, установленный для собрания, будет отражаться в списке.</span><span class="sxs-lookup"><span data-stu-id="3a1f1-106">**Note**: If the chat is associated with an [onlineMeeting](../resources/onlinemeeting.md) instance, then, effectively, the **teamsApp** s installed in the meeting will be listed.</span></span>

> [!NOTE]
> <span data-ttu-id="3a1f1-107">`id`Ресурс **teamsAppInstallation** имеет не то же значение, что и `id` связанный ресурс **teamsApp**.</span><span class="sxs-lookup"><span data-stu-id="3a1f1-107">The `id` of a **teamsAppInstallation** resource is not the same value as the `id` of the associated **teamsApp** resource.</span></span>


## <a name="permissions"></a><span data-ttu-id="3a1f1-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3a1f1-108">Permissions</span></span>

<span data-ttu-id="3a1f1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a1f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a1f1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a1f1-111">Permission type</span></span>      | <span data-ttu-id="3a1f1-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a1f1-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a1f1-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a1f1-113">Delegated (work or school account)</span></span> | <span data-ttu-id="3a1f1-114">TeamsAppInstallation.ReadForChat, TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span><span class="sxs-lookup"><span data-stu-id="3a1f1-114">TeamsAppInstallation.ReadForChat, TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span></span> |
|<span data-ttu-id="3a1f1-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a1f1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a1f1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a1f1-116">Not supported.</span></span>    |
|<span data-ttu-id="3a1f1-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="3a1f1-117">Application</span></span> | <span data-ttu-id="3a1f1-118">TeamsAppInstallation.ReadForChat.All, TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span><span class="sxs-lookup"><span data-stu-id="3a1f1-118">TeamsAppInstallation.ReadForChat.All, TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a1f1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a1f1-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /chats/{chat-id}/installedApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3a1f1-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3a1f1-120">Optional query parameters</span></span>

<span data-ttu-id="3a1f1-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$filter`, `$select` и `$expand` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="3a1f1-121">This method supports the `$filter`, `$select`, and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3a1f1-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3a1f1-122">Request headers</span></span>

| <span data-ttu-id="3a1f1-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3a1f1-123">Header</span></span>       | <span data-ttu-id="3a1f1-124">Значение</span><span class="sxs-lookup"><span data-stu-id="3a1f1-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3a1f1-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3a1f1-125">Authorization</span></span>  | <span data-ttu-id="3a1f1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3a1f1-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3a1f1-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3a1f1-128">Request body</span></span>

<span data-ttu-id="3a1f1-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3a1f1-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a1f1-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a1f1-130">Response</span></span>

<span data-ttu-id="3a1f1-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [teamsAppInstallation](../resources/teamsappinstallation.md) в тексте сообщения.</span><span class="sxs-lookup"><span data-stu-id="3a1f1-131">If successful, this method returns a `200 OK` response code and a collection of [teamsAppInstallation](../resources/teamsappinstallation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3a1f1-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="3a1f1-132">Examples</span></span>

### <a name="example-1-get-all-the-apps-installed-in-the-specified-chat"></a><span data-ttu-id="3a1f1-133">Пример 1: Получение всех приложений, установленных в указанном чате</span><span class="sxs-lookup"><span data-stu-id="3a1f1-133">Example 1: Get all the apps installed in the specified chat</span></span>

#### <a name="request"></a><span data-ttu-id="3a1f1-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a1f1-134">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="3a1f1-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="3a1f1-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_installed_apps_in_chat"
}
-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/chats/19%3Ad65713bc498c4a428c71ef9353e6ce20%40thread.v2/installedApps
```
# <a name="c"></a>[<span data-ttu-id="3a1f1-136">C#</span><span class="sxs-lookup"><span data-stu-id="3a1f1-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-installed-apps-in-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3a1f1-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3a1f1-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-installed-apps-in-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3a1f1-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3a1f1-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-installed-apps-in-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3a1f1-139">Java</span><span class="sxs-lookup"><span data-stu-id="3a1f1-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-installed-apps-in-chat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="3a1f1-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a1f1-140">Response</span></span>

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#chats('19%3Ad65713bc498c4a428c71ef9353e6ce20%40thread.v2')/installedApps",
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

### <a name="example-2-get-the-names-and-other-details-of-apps-installed-in-the-specified-chat"></a><span data-ttu-id="3a1f1-141">Пример 2: Получение имен и других сведений о приложениях, установленных в указанном чате</span><span class="sxs-lookup"><span data-stu-id="3a1f1-141">Example 2: Get the names and other details of apps installed in the specified chat</span></span>

<span data-ttu-id="3a1f1-142">В следующем примере, если с экземпляром установленного приложения связан [бот](../resources/teamworkbot.md), сведения о нем также возвращаются.</span><span class="sxs-lookup"><span data-stu-id="3a1f1-142">In the following example, if an instance of an installed app has a [bot](../resources/teamworkbot.md) associated with it, then the details of the bot are returned as well.</span></span>

#### <a name="request"></a><span data-ttu-id="3a1f1-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a1f1-143">Request</span></span>



# <a name="http"></a>[<span data-ttu-id="3a1f1-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="3a1f1-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_installed_apps_in_chat_expand"
}
-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/chats/19%3Ad65713bc498c4a428c71ef9353e6ce20%40thread.v2/installedApps?$expand=teamsAppDefinition($expand=bot)
```
# <a name="c"></a>[<span data-ttu-id="3a1f1-145">C#</span><span class="sxs-lookup"><span data-stu-id="3a1f1-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-installed-apps-in-chat-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3a1f1-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3a1f1-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-installed-apps-in-chat-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3a1f1-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3a1f1-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-installed-apps-in-chat-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3a1f1-148">Java</span><span class="sxs-lookup"><span data-stu-id="3a1f1-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-installed-apps-in-chat-expand-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3a1f1-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a1f1-149">Response</span></span>

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#chats('19%3Ad65713bc498c4a428c71ef9353e6ce20%40thread.v2')/installedApps(teamsAppDefinition())",
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

### <a name="example-3-get-the-app-installation-resource-based-on-the-manifest-id-of-the-associated-app"></a><span data-ttu-id="3a1f1-150">Пример 3: Получение ресурса установки приложения на основе идентификатора манифеста связанного приложения</span><span class="sxs-lookup"><span data-stu-id="3a1f1-150">Example 3: Get the app installation resource based on the manifest id of the associated app</span></span>

#### <a name="request"></a><span data-ttu-id="3a1f1-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a1f1-151">Request</span></span>

<span data-ttu-id="3a1f1-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3a1f1-152">The following is an example of the request.</span></span> <span data-ttu-id="3a1f1-153">В этом примере идентификатор манифеста приложения Teams — 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'.</span><span class="sxs-lookup"><span data-stu-id="3a1f1-153">In the example, the manifest ID of the Teams app is 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'.</span></span>


# <a name="http"></a>[<span data-ttu-id="3a1f1-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="3a1f1-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_installed_apps_in_chat_expand_filter"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/chats/19%3Ad65713bc498c4a428c71ef9353e6ce20%40thread.v2/installedApps?$expand=teamsApp,teamsAppDefinition&$filter=teamsApp/externalId eq 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'
```
# <a name="c"></a>[<span data-ttu-id="3a1f1-155">C#</span><span class="sxs-lookup"><span data-stu-id="3a1f1-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-installed-apps-in-chat-expand-filter-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3a1f1-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3a1f1-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-installed-apps-in-chat-expand-filter-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3a1f1-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3a1f1-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-installed-apps-in-chat-expand-filter-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3a1f1-158">Java</span><span class="sxs-lookup"><span data-stu-id="3a1f1-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-installed-apps-in-chat-expand-filter-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="3a1f1-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a1f1-159">Response</span></span>

<span data-ttu-id="3a1f1-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3a1f1-160">The following is an example of the response.</span></span>

><span data-ttu-id="3a1f1-161">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3a1f1-161">**Note:** The response object shown here might be shortened for readability.</span></span> 
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

## <a name="see-also"></a><span data-ttu-id="3a1f1-162">Дополнительные материалы</span><span class="sxs-lookup"><span data-stu-id="3a1f1-162">See also</span></span>
- [<span data-ttu-id="3a1f1-163">Список приложений в каталоге</span><span class="sxs-lookup"><span data-stu-id="3a1f1-163">List apps in catalog</span></span>](appcatalogs-list-teamsapps.md)
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chat list installedapps",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
