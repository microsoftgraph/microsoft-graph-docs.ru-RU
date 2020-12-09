---
title: Список приложений в команде
description: Получение списка приложений, установленных в указанной команде.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 72393fb3c76c7d9b79aac80c3888bb42f4ccc3cc
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607679"
---
# <a name="list-apps-in-team"></a><span data-ttu-id="0ce9e-103">Список приложений в команде</span><span class="sxs-lookup"><span data-stu-id="0ce9e-103">List apps in team</span></span>

<span data-ttu-id="0ce9e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ce9e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0ce9e-105">Получение списка приложений, [установленных](../resources/teamsappinstallation.md) в указанной [команде](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="0ce9e-105">Retrieve the list of [apps installed](../resources/teamsappinstallation.md) in the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0ce9e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0ce9e-106">Permissions</span></span>

<span data-ttu-id="0ce9e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ce9e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ce9e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ce9e-109">Permission type</span></span>      | <span data-ttu-id="0ce9e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ce9e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ce9e-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ce9e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0ce9e-112">Теамсаппинсталлатион. Реадфортеам, Теамсаппинсталлатион. Реадвритефортеам, Group. Read. ALL, Group. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0ce9e-112">TeamsAppInstallation.ReadForTeam, TeamsAppInstallation.ReadWriteForTeam, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="0ce9e-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ce9e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ce9e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ce9e-114">Not supported.</span></span>    |
|<span data-ttu-id="0ce9e-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="0ce9e-115">Application</span></span> | <span data-ttu-id="0ce9e-116">Теамсаппинсталлатион. Read. Group \*, Теамсаппинсталлатион. Реадфортеам. ALL, Теамсаппинсталлатион. Реадвритефортеам. ALL, Group. Read. ALL, Group. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="0ce9e-116">TeamsAppInstallation.Read.Group\*, TeamsAppInstallation.ReadForTeam.All, TeamsAppInstallation.ReadWriteForTeam.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="0ce9e-117">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="0ce9e-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

## <a name="http-request"></a><span data-ttu-id="0ce9e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ce9e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{team-id}/installedApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0ce9e-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0ce9e-119">Optional query parameters</span></span>

<span data-ttu-id="0ce9e-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$filter`, `$select` и `$expand` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="0ce9e-120">This method supports the `$filter`, `$select`, and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0ce9e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0ce9e-121">Request headers</span></span>

| <span data-ttu-id="0ce9e-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0ce9e-122">Header</span></span>       | <span data-ttu-id="0ce9e-123">Значение</span><span class="sxs-lookup"><span data-stu-id="0ce9e-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0ce9e-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0ce9e-124">Authorization</span></span>  | <span data-ttu-id="0ce9e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0ce9e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0ce9e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0ce9e-127">Request body</span></span>

<span data-ttu-id="0ce9e-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0ce9e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ce9e-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ce9e-129">Response</span></span>

<span data-ttu-id="0ce9e-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [теамсаппинсталлатион](../resources/teamsappinstallation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0ce9e-130">If successful, this method returns a `200 OK` response code and collection of [teamsAppInstallation](../resources/teamsappinstallation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0ce9e-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="0ce9e-131">Examples</span></span>

### <a name="example-1-list-installed-apps"></a><span data-ttu-id="0ce9e-132">Пример 1: список установленных приложений</span><span class="sxs-lookup"><span data-stu-id="0ce9e-132">Example 1: List installed apps</span></span>
#### <a name="request"></a><span data-ttu-id="0ce9e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ce9e-133">Request</span></span>

<span data-ttu-id="0ce9e-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0ce9e-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_installed_apps_in_team"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/6903fa93-605b-43ef-920e-77c4729f8258/installedApps
```

#### <a name="response"></a><span data-ttu-id="0ce9e-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ce9e-135">Response</span></span>

<span data-ttu-id="0ce9e-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0ce9e-136">The following is an example of the response.</span></span>
><span data-ttu-id="0ce9e-137">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0ce9e-137">**Note:** The response object shown here might be shortened for readability.</span></span> 
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

### <a name="example-2-get-the-names-and-other-details-of-installed-apps"></a><span data-ttu-id="0ce9e-138">Пример 2: получение имен и других сведений об установленных приложениях</span><span class="sxs-lookup"><span data-stu-id="0ce9e-138">Example 2: Get the names and other details of installed apps</span></span>

#### <a name="request"></a><span data-ttu-id="0ce9e-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ce9e-139">Request</span></span>

<span data-ttu-id="0ce9e-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0ce9e-140">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_installed_teams_apps_expand"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/6903fa93-605b-43ef-920e-77c4729f8258/installedApps?$expand=teamsAppDefinition
```

#### <a name="response"></a><span data-ttu-id="0ce9e-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ce9e-141">Response</span></span>

<span data-ttu-id="0ce9e-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0ce9e-142">The following is an example of the response.</span></span>

><span data-ttu-id="0ce9e-143">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0ce9e-143">**Note:** The response object shown here might be shortened for readability.</span></span> 
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
                "createdBy": null
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

### <a name="example-3-get-the-app-installation-resource-based-on-the-manifest-id-of-the-associated-app"></a><span data-ttu-id="0ce9e-144">Пример 3: получение ресурса установки приложения на основе идентификатора манифеста связанного приложения</span><span class="sxs-lookup"><span data-stu-id="0ce9e-144">Example 3: Get the app installation resource based on the manifest ID of the associated app</span></span>

#### <a name="request"></a><span data-ttu-id="0ce9e-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ce9e-145">Request</span></span>

<span data-ttu-id="0ce9e-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0ce9e-146">The following is an example of the request.</span></span> <span data-ttu-id="0ce9e-147">В этом примере идентификатор манифеста приложения Teams — `cf1ba4c7-f94e-4d80-ba90-5594b641a8ee` .</span><span class="sxs-lookup"><span data-stu-id="0ce9e-147">In the example, the manifest ID of the Teams app is `cf1ba4c7-f94e-4d80-ba90-5594b641a8ee`.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_installed_apps_in_team_expand_filter_externalid"
}-->
```http
GET https://graph.microsoft.com/beta/teams/acda442c-78d2-491b-8204-4ef5019c0193/installedApps?$expand=teamsApp,teamsAppDefinition&$filter=teamsApp/externalId eq 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'
```

#### <a name="response"></a><span data-ttu-id="0ce9e-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ce9e-148">Response</span></span>

<span data-ttu-id="0ce9e-149">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="0ce9e-149">The following is an example of the response.</span></span>

><span data-ttu-id="0ce9e-150">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0ce9e-150">**Note:** The response object shown here might be shortened for readability.</span></span> 
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

