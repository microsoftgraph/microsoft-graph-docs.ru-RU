---
title: Список приложений в команде
description: Извлечение списка приложений, установленных в указанной группе.
author: akjo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7daf041f27697a99c23ad0dc16c861ea6a8ef10c
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060553"
---
# <a name="list-apps-in-team"></a><span data-ttu-id="788b7-103">Список приложений в команде</span><span class="sxs-lookup"><span data-stu-id="788b7-103">List apps in team</span></span>

<span data-ttu-id="788b7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="788b7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="788b7-105">Извлечение списка [приложений, установленных](../resources/teamsappinstallation.md) в указанной [группе.](../resources/team.md)</span><span class="sxs-lookup"><span data-stu-id="788b7-105">Retrieve a list of [apps installed](../resources/teamsappinstallation.md) in the specified [team](../resources/team.md).</span></span>


> [!NOTE]
> <span data-ttu-id="788b7-106">`id`Ресурс **teamsAppInstallation** имеет не то же значение, что и `id` связанный ресурс **teamsApp**.</span><span class="sxs-lookup"><span data-stu-id="788b7-106">The `id` of a **teamsAppInstallation** resource is not the same value as the `id` of the associated **teamsApp** resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="788b7-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="788b7-107">Permissions</span></span>

<span data-ttu-id="788b7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="788b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="788b7-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="788b7-110">Permission type</span></span>      | <span data-ttu-id="788b7-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="788b7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="788b7-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="788b7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="788b7-113">TeamsAppInstallation.ReadForTeam, TeamsAppInstallation.ReadWriteForTeam, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="788b7-113">TeamsAppInstallation.ReadForTeam, TeamsAppInstallation.ReadWriteForTeam, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="788b7-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="788b7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="788b7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="788b7-115">Not supported.</span></span>    |
|<span data-ttu-id="788b7-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="788b7-116">Application</span></span> | <span data-ttu-id="788b7-117">TeamsAppInstallation.Read.Group\*, TeamsAppInstallation.ReadForTeam.All, TeamsAppInstallation.ReadWriteForTeam.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="788b7-117">TeamsAppInstallation.Read.Group\*, TeamsAppInstallation.ReadForTeam.All, TeamsAppInstallation.ReadWriteForTeam.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="788b7-118">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="788b7-118">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

## <a name="http-request"></a><span data-ttu-id="788b7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="788b7-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{team-id}/installedApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="788b7-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="788b7-120">Optional query parameters</span></span>

<span data-ttu-id="788b7-121">Этот метод поддерживает `$filter` параметры `$select` запроса `$expand` [OData и OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="788b7-121">This method supports the `$filter`, `$select`, and `$expand` [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="788b7-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="788b7-122">Request headers</span></span>

| <span data-ttu-id="788b7-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="788b7-123">Header</span></span>       | <span data-ttu-id="788b7-124">Значение</span><span class="sxs-lookup"><span data-stu-id="788b7-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="788b7-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="788b7-125">Authorization</span></span>  | <span data-ttu-id="788b7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="788b7-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="788b7-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="788b7-128">Request body</span></span>

<span data-ttu-id="788b7-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="788b7-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="788b7-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="788b7-130">Response</span></span>

<span data-ttu-id="788b7-131">В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` [объектов teamsAppInstallation](../resources/teamsappinstallation.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="788b7-131">If successful, this method returns a `200 OK` response code and collection of [teamsAppInstallation](../resources/teamsappinstallation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="788b7-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="788b7-132">Examples</span></span>

### <a name="example-1-list-installed-apps"></a><span data-ttu-id="788b7-133">Пример 1. Список установленных приложений</span><span class="sxs-lookup"><span data-stu-id="788b7-133">Example 1: List installed apps</span></span>
#### <a name="request"></a><span data-ttu-id="788b7-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="788b7-134">Request</span></span>

<span data-ttu-id="788b7-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="788b7-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="788b7-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="788b7-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_installed_apps_in_team"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/6903fa93-605b-43ef-920e-77c4729f8258/installedApps
```
# <a name="c"></a>[<span data-ttu-id="788b7-137">C#</span><span class="sxs-lookup"><span data-stu-id="788b7-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-installed-apps-in-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="788b7-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="788b7-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-installed-apps-in-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="788b7-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="788b7-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-installed-apps-in-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="788b7-140">Java</span><span class="sxs-lookup"><span data-stu-id="788b7-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-installed-apps-in-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="788b7-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="788b7-141">Response</span></span>

<span data-ttu-id="788b7-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="788b7-142">The following is an example of the response.</span></span>
><span data-ttu-id="788b7-143">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="788b7-143">**Note:** The response object shown here might be shortened for readability.</span></span>
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
   "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#teams('6903fa93-605b-43ef-920e-77c4729f8258')/installedApps",
   "@odata.count":3,
   "value":[
      {
         "id":"NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwMDAwMTAxNi1kZTA1LTQ5MmUtOTEwNi00ODI4ZmM4YTg2ODc="
      },
      {
         "id":"NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwYWUzNWIzNi0wZmQ3LTQyMmUtODA1Yi1kNTNhZjE1NzkwOTM="
      },
      {
         "id":"NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg="
      }
   ]
}
```

### <a name="example-2-get-the-names-and-other-details-of-installed-apps"></a><span data-ttu-id="788b7-144">Пример 2. Получить имена и другие сведения об установленных приложениях</span><span class="sxs-lookup"><span data-stu-id="788b7-144">Example 2: Get the names and other details of installed apps</span></span>

#### <a name="request"></a><span data-ttu-id="788b7-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="788b7-145">Request</span></span>

<span data-ttu-id="788b7-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="788b7-146">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="788b7-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="788b7-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_installed_teams_apps_expand"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/6903fa93-605b-43ef-920e-77c4729f8258/installedApps?$expand=teamsAppDefinition
```
# <a name="c"></a>[<span data-ttu-id="788b7-148">C#</span><span class="sxs-lookup"><span data-stu-id="788b7-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-installed-teams-apps-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="788b7-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="788b7-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-installed-teams-apps-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="788b7-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="788b7-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-installed-teams-apps-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="788b7-151">Java</span><span class="sxs-lookup"><span data-stu-id="788b7-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-installed-teams-apps-expand-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="788b7-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="788b7-152">Response</span></span>

<span data-ttu-id="788b7-153">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="788b7-153">The following is an example of the response.</span></span>

><span data-ttu-id="788b7-154">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="788b7-154">**Note:** The response object shown here might be shortened for readability.</span></span>
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
   "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#teams('6903fa93-605b-43ef-920e-77c4729f8258')/installedApps(teamsAppDefinition())",
   "@odata.count":3,
   "value":[
      {
         "id":"NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwMDAwMTAxNi1kZTA1LTQ5MmUtOTEwNi00ODI4ZmM4YTg2ODc=",
         "teamsAppDefinition":{
            "id":"MDAwMDEwMTYtZGUwNS00OTJlLTkxMDYtNDgyOGZjOGE4Njg3IyMxLjAuMg==",
            "teamsAppId":"00001016-de05-492e-9106-4828fc8a8687",
            "azureADAppId":"7df0a125-d3be-4c96-aa54-591f83ff541c",
            "displayName":"Power Automate Actions",
            "version":"1.0.2",
            "requiredResourceSpecificApplicationPermissions":[
               
            ],
            "publishingState":"published",
            "shortDescription":"Be more productive with Microsoft Flow",
            "description":"Automate time-consuming and repetitive tasks by integrating your favorite apps and services with Microsoft Power Automate.",
            "lastModifiedDateTime":null,
            "createdBy":null
         }
      },
      {
         "id":"NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwYWUzNWIzNi0wZmQ3LTQyMmUtODA1Yi1kNTNhZjE1NzkwOTM=",
         "teamsAppDefinition":{
            "id":"MGFlMzViMzYtMGZkNy00MjJlLTgwNWItZDUzYWYxNTc5MDkzIyMxLjI=",
            "teamsAppId":"0ae35b36-0fd7-422e-805b-d53af1579093",
            "azureADAppId":"00000003-0000-0ff1-ce00-000000000000",
            "displayName":"SharePoint Pages",
            "version":"1.2",
            "requiredResourceSpecificApplicationPermissions":[
               
            ],
            "publishingState":"published",
            "shortDescription":"Add a tab for a SharePoint news article or page.",
            "description":"This app allows you to tab intranet pages from any SharePoint site so that they can be viewed by your team inside Teams channels.",
            "lastModifiedDateTime":null,
            "createdBy":null
         }
      },
      {
         "id":"NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg=",
         "teamsAppDefinition":{
            "id":"MGQ4MjBlY2QtZGVmMi00Mjk3LWFkYWQtNzgwNTZjZGU3Yzc4IyMxLjAuMA==",
            "teamsAppId":"0d820ecd-def2-4297-adad-78056cde7c78",
            "azureADAppId":"2d4d3d8e-2be3-4bef-9f87-7875a61c29de",
            "displayName":"OneNote",
            "version":"1.0.0",
            "requiredResourceSpecificApplicationPermissions":[
               
            ],
            "publishingState":"published",
            "shortDescription":"Capture and share ideas, to-do lists and other notes with your team.",
            "description":"Capture and share ideas, to-do lists and other thoughts with your team. You can also co-author anytime.",
            "lastModifiedDateTime":null,
            "createdBy":null
         }
      }
   ]
}
```

### <a name="example-3-get-the-app-installation-resource-based-on-the-manifest-id-of-the-associated-app"></a><span data-ttu-id="788b7-155">Пример 3. Получить ресурс установки приложения на основе манифеста ID связанного приложения</span><span class="sxs-lookup"><span data-stu-id="788b7-155">Example 3: Get the app installation resource based on the manifest ID of the associated app</span></span>

#### <a name="request"></a><span data-ttu-id="788b7-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="788b7-156">Request</span></span>

<span data-ttu-id="788b7-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="788b7-157">The following is an example of the request.</span></span> <span data-ttu-id="788b7-158">В этом примере идентификатор манифеста приложения Teams — 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'.</span><span class="sxs-lookup"><span data-stu-id="788b7-158">In the example, the manifest ID of the Teams app is 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'.</span></span>

# <a name="http"></a>[<span data-ttu-id="788b7-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="788b7-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_installed_apps_in_team_expand_filter_externalid"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/acda442c-78d2-491b-8204-4ef5019c0193/installedApps?$expand=teamsApp,teamsAppDefinition&$filter=teamsApp/externalId eq 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'
```
# <a name="c"></a>[<span data-ttu-id="788b7-160">C#</span><span class="sxs-lookup"><span data-stu-id="788b7-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-installed-apps-in-team-expand-filter-externalid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="788b7-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="788b7-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-installed-apps-in-team-expand-filter-externalid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="788b7-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="788b7-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-installed-apps-in-team-expand-filter-externalid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="788b7-163">Java</span><span class="sxs-lookup"><span data-stu-id="788b7-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-installed-apps-in-team-expand-filter-externalid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="788b7-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="788b7-164">Response</span></span>

<span data-ttu-id="788b7-165">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="788b7-165">The following is an example of the response.</span></span>

><span data-ttu-id="788b7-166">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="788b7-166">**Note:** The response object shown here might be shortened for readability.</span></span>
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
   "@odata.count":1,
   "value":[
      {
         "id":"NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwMjQwYTM2OC0yNWUwLTQ1NjktOGViZS0xMzYwMWNiNTVhMTg=",
         "teamsApp":{
            "id":"0240a368-25e0-4569-8ebe-13601cb55a18",
            "externalId":"cf1ba4c7-f94e-4d80-ba90-5594b641a8ee",
            "displayName":"YPA",
            "distributionMethod":"sideloaded"
         },
         "teamsAppDefinition":{
            "id":"MDI0MGEzNjgtMjVlMC00NTY5LThlYmUtMTM2MDFjYjU1YTE4IyM2LjAuMA==",
            "teamsAppId":"0240a368-25e0-4569-8ebe-13601cb55a18",
            "azureADAppId":"9fc97ea2-c417-4c76-a2db-197612067b28",
            "displayName":"YPA",
            "version":"6.0.0",
            "requiredResourceSpecificApplicationPermissions":[
               
            ],
            "publishingState":"published",
            "shortDescription":"A conversational smart assistant from MSX that surfaces real-time insights.",
            "description":"For MSX Users: A conversational role-based smart assistant that will enable Enterprise sellers (AE, ATS, SSP, TSP) to be more productive by surfacing real-time insights, recommendations, actions and notifications, and by automating repetitive tasks.",
            "lastModifiedDateTime":null,
            "createdBy":null
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

## <a name="see-also"></a><span data-ttu-id="788b7-167">Дополнительные материалы</span><span class="sxs-lookup"><span data-stu-id="788b7-167">See also</span></span>
- [<span data-ttu-id="788b7-168">Список приложений в каталоге</span><span class="sxs-lookup"><span data-stu-id="788b7-168">List apps in catalog</span></span>](appcatalogs-list-teamsapps.md)
