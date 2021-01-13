---
title: Список приложений в команде
description: Получить список приложений, установленных в указанной команде.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f7de268d3472bcef60ad77064c1c725d79174e32
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844461"
---
# <a name="list-apps-in-team"></a><span data-ttu-id="35cea-103">Список приложений в команде</span><span class="sxs-lookup"><span data-stu-id="35cea-103">List apps in team</span></span>

<span data-ttu-id="35cea-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35cea-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="35cea-105">Получить список [приложений, установленных](../resources/teamsappinstallation.md) в указанной [команде.](../resources/team.md)</span><span class="sxs-lookup"><span data-stu-id="35cea-105">Retrieve the list of [apps installed](../resources/teamsappinstallation.md) in the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="35cea-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="35cea-106">Permissions</span></span>

<span data-ttu-id="35cea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35cea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35cea-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="35cea-109">Permission type</span></span>      | <span data-ttu-id="35cea-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="35cea-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="35cea-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="35cea-111">Delegated (work or school account)</span></span> | <span data-ttu-id="35cea-112">TeamsAppInstallation.ReadForTeam, TeamsAppInstallation.ReadWriteForTeam, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35cea-112">TeamsAppInstallation.ReadForTeam, TeamsAppInstallation.ReadWriteForTeam, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="35cea-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="35cea-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35cea-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35cea-114">Not supported.</span></span>    |
|<span data-ttu-id="35cea-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="35cea-115">Application</span></span> | <span data-ttu-id="35cea-116">TeamsAppInstallation.Read.Group\*, TeamsAppInstallation.ReadForTeam.All, TeamsAppInstallation.ReadWriteForTeam.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35cea-116">TeamsAppInstallation.Read.Group\*, TeamsAppInstallation.ReadForTeam.All, TeamsAppInstallation.ReadWriteForTeam.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="35cea-117">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="35cea-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

## <a name="http-request"></a><span data-ttu-id="35cea-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="35cea-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{team-id}/installedApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="35cea-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="35cea-119">Optional query parameters</span></span>

<span data-ttu-id="35cea-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$filter`, `$select` и `$expand` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="35cea-120">This method supports the `$filter`, `$select`, and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="35cea-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="35cea-121">Request headers</span></span>

| <span data-ttu-id="35cea-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="35cea-122">Header</span></span>       | <span data-ttu-id="35cea-123">Значение</span><span class="sxs-lookup"><span data-stu-id="35cea-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="35cea-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="35cea-124">Authorization</span></span>  | <span data-ttu-id="35cea-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="35cea-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="35cea-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="35cea-127">Request body</span></span>

<span data-ttu-id="35cea-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="35cea-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="35cea-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="35cea-129">Response</span></span>

<span data-ttu-id="35cea-130">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [teamsAppInstallation](../resources/teamsappinstallation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="35cea-130">If successful, this method returns a `200 OK` response code and collection of [teamsAppInstallation](../resources/teamsappinstallation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="35cea-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="35cea-131">Examples</span></span>

### <a name="example-1-list-installed-apps"></a><span data-ttu-id="35cea-132">Пример 1. Список установленных приложений</span><span class="sxs-lookup"><span data-stu-id="35cea-132">Example 1: List installed apps</span></span>
#### <a name="request"></a><span data-ttu-id="35cea-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="35cea-133">Request</span></span>

<span data-ttu-id="35cea-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="35cea-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="35cea-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="35cea-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_installed_apps_in_team"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/6903fa93-605b-43ef-920e-77c4729f8258/installedApps
```
# <a name="c"></a>[<span data-ttu-id="35cea-136">C#</span><span class="sxs-lookup"><span data-stu-id="35cea-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-installed-apps-in-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="35cea-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="35cea-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-installed-apps-in-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="35cea-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="35cea-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-installed-apps-in-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="35cea-139">Java</span><span class="sxs-lookup"><span data-stu-id="35cea-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-installed-apps-in-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="35cea-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="35cea-140">Response</span></span>

<span data-ttu-id="35cea-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="35cea-141">The following is an example of the response.</span></span>
><span data-ttu-id="35cea-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="35cea-142">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "name": "list_installed_apps_in_team",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('6903fa93-605b-43ef-920e-77c4729f8258')/installedApps",
    "@odata.count": 3,
    "value": [
        {
            "id": "NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwMDAwMTAxNi1kZTA1LTQ5MmUtOTEwNi00ODI4ZmM4YTg2ODc="
        },
        {
            "id": "NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwYWUzNWIzNi0wZmQ3LTQyMmUtODA1Yi1kNTNhZjE1NzkwOTM="
        },
        {
            "id": "NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg="
        }
  ]
}
```

### <a name="example-2-get-the-names-and-other-details-of-installed-apps"></a><span data-ttu-id="35cea-143">Пример 2. Просмотр имен и других сведений об установленных приложениях</span><span class="sxs-lookup"><span data-stu-id="35cea-143">Example 2: Get the names and other details of installed apps</span></span>

#### <a name="request"></a><span data-ttu-id="35cea-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="35cea-144">Request</span></span>

<span data-ttu-id="35cea-145">В следующем примере, если с экземпляром установленного приложения связан [бот](../resources/teamworkbot.md), сведения о нем также возвращаются.</span><span class="sxs-lookup"><span data-stu-id="35cea-145">In the following example, if an instance of an installed app has a [bot](../resources/teamworkbot.md) associated with it, then the details of the bot are returned as well.</span></span>


<!-- {
  "blockType": "request",
  "name": "list_installed_teams_apps_expand"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/6903fa93-605b-43ef-920e-77c4729f8258/installedApps?$expand=teamsAppDefinition($expand=bot)
```

#### <a name="response"></a><span data-ttu-id="35cea-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="35cea-146">Response</span></span>

<span data-ttu-id="35cea-147">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="35cea-147">The following is an example of the response.</span></span>

><span data-ttu-id="35cea-148">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="35cea-148">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "name": "list_installed_teams_apps_expand",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('6903fa93-605b-43ef-920e-77c4729f8258')/installedApps(teamsAppDefinition())",
    "@odata.count": 3,
    "value": [
        {
            "id": "NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwMDAwMTAxNi1kZTA1LTQ5MmUtOTEwNi00ODI4ZmM4YTg2ODc=",
            "teamsAppDefinition": {
                "id": "MDAwMDEwMTYtZGUwNS00OTJlLTkxMDYtNDgyOGZjOGE4Njg3IyMxLjAuMg==",
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
            "id": "NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwYWUzNWIzNi0wZmQ3LTQyMmUtODA1Yi1kNTNhZjE1NzkwOTM=",
            "teamsAppDefinition": {
                "id": "MGFlMzViMzYtMGZkNy00MjJlLTgwNWItZDUzYWYxNTc5MDkzIyMxLjI=",
                "teamsAppId": "0ae35b36-0fd7-422e-805b-d53af1579093",
                "azureADAppId": "00000003-0000-0ff1-ce00-000000000000",
                "displayName": "SharePoint Pages",
                "version": "1.2",
                "requiredResourceSpecificApplicationPermissions": [],
                "publishingState": "published",
                "shortdescription": "Add a tab for a SharePoint news article or page.",
                "description": "This app allows you to tab intranet pages from any SharePoint site so that they can be viewed by your team inside Teams channels.",
                "lastModifiedDateTime": null,
                "createdBy": null
            }
        },
        {
            "id": "NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg=",
            "teamsAppDefinition": {
                "id": "MGQ4MjBlY2QtZGVmMi00Mjk3LWFkYWQtNzgwNTZjZGU3Yzc4IyMxLjAuMA==",
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
        }
  ]
}
```

### <a name="example-3-get-the-app-installation-resource-based-on-the-manifest-id-of-the-associated-app"></a><span data-ttu-id="35cea-149">Пример 3. Получите ресурс установки приложения на основе ИД манифеста связанного приложения</span><span class="sxs-lookup"><span data-stu-id="35cea-149">Example 3: Get the app installation resource based on the manifest ID of the associated app</span></span>

#### <a name="request"></a><span data-ttu-id="35cea-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="35cea-150">Request</span></span>

<span data-ttu-id="35cea-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="35cea-151">The following is an example of the request.</span></span> <span data-ttu-id="35cea-152">В этом примере ид манифеста приложения Teams: `cf1ba4c7-f94e-4d80-ba90-5594b641a8ee` .</span><span class="sxs-lookup"><span data-stu-id="35cea-152">In the example, the manifest ID of the Teams app is `cf1ba4c7-f94e-4d80-ba90-5594b641a8ee`.</span></span>

# <a name="http"></a>[<span data-ttu-id="35cea-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="35cea-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_installed_apps_in_team_expand_filter_externalid"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/acda442c-78d2-491b-8204-4ef5019c0193/installedApps?$expand=teamsApp,teamsAppDefinition&$filter=teamsApp/externalId eq 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'
```
# <a name="c"></a>[<span data-ttu-id="35cea-154">C#</span><span class="sxs-lookup"><span data-stu-id="35cea-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-installed-apps-in-team-expand-filter-externalid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="35cea-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="35cea-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-installed-apps-in-team-expand-filter-externalid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="35cea-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="35cea-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-installed-apps-in-team-expand-filter-externalid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="35cea-157">Java</span><span class="sxs-lookup"><span data-stu-id="35cea-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-installed-apps-in-team-expand-filter-externalid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="35cea-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="35cea-158">Response</span></span>

<span data-ttu-id="35cea-159">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="35cea-159">The following is an example of the response.</span></span>

><span data-ttu-id="35cea-160">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="35cea-160">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "name": "list_installed_apps_in_team_expand_filter_externalid",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

