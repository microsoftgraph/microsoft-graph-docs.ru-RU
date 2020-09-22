---
title: Список приложений в команде
description: Получение списка приложений, установленных в указанной команде.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: dfe6d2748fa3fd148292e005a9f600a0568627fd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47978379"
---
# <a name="list-apps-in-team"></a><span data-ttu-id="801a8-103">Список приложений в команде</span><span class="sxs-lookup"><span data-stu-id="801a8-103">List apps in team</span></span>

<span data-ttu-id="801a8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="801a8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="801a8-105">Получение списка приложений, [установленных](../resources/teamsappinstallation.md) в указанной [команде](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="801a8-105">Retrieve the list of [apps installed](../resources/teamsappinstallation.md) in the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="801a8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="801a8-106">Permissions</span></span>

<span data-ttu-id="801a8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="801a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="801a8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="801a8-109">Permission type</span></span>      | <span data-ttu-id="801a8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="801a8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="801a8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="801a8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="801a8-112">Теамсаппинсталлатион. Реадфортеам, Теамсаппинсталлатион. Реадвритефортеам, Group. Read. ALL, Group. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="801a8-112">TeamsAppInstallation.ReadForTeam, TeamsAppInstallation.ReadWriteForTeam, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="801a8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="801a8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="801a8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="801a8-114">Not supported.</span></span>    |
|<span data-ttu-id="801a8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="801a8-115">Application</span></span> | <span data-ttu-id="801a8-116">Теамсаппинсталлатион. Реадфортеам. ALL, Теамсаппинсталлатион. Реадвритефортеам. ALL, Group. Read. ALL, Group. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="801a8-116">TeamsAppInstallation.ReadForTeam.All, TeamsAppInstallation.ReadWriteForTeam.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="801a8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="801a8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/installedApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="801a8-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="801a8-118">Optional query parameters</span></span>

<span data-ttu-id="801a8-119">Этот метод поддерживает [параметры запросов](/graph/query-parameters) $filter, $select и $Expand OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="801a8-119">This method supports the $filter, $select, and $expand [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="801a8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="801a8-120">Request headers</span></span>

| <span data-ttu-id="801a8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="801a8-121">Header</span></span>       | <span data-ttu-id="801a8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="801a8-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="801a8-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="801a8-123">Authorization</span></span>  | <span data-ttu-id="801a8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="801a8-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="801a8-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="801a8-126">Request body</span></span>

<span data-ttu-id="801a8-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="801a8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="801a8-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="801a8-128">Response</span></span>

<span data-ttu-id="801a8-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [теамсаппинсталлатион](../resources/teamsappinstallation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="801a8-129">If successful, this method returns a `200 OK` response code and collection of [teamsAppInstallation](../resources/teamsappinstallation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="801a8-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="801a8-130">Examples</span></span>

### <a name="example-1-list-installed-apps"></a><span data-ttu-id="801a8-131">Пример 1: список установленных приложений</span><span class="sxs-lookup"><span data-stu-id="801a8-131">Example 1: List installed apps</span></span>
#### <a name="request"></a><span data-ttu-id="801a8-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="801a8-132">Request</span></span>

<span data-ttu-id="801a8-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="801a8-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="801a8-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="801a8-134">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_installed_teams_apps"
}-->

```msgraph-interactive
GET /teams/{id}/installedApps
```
# <a name="c"></a>[<span data-ttu-id="801a8-135">C#</span><span class="sxs-lookup"><span data-stu-id="801a8-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-installed-teams-apps-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="801a8-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="801a8-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-installed-teams-apps-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="801a8-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="801a8-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-installed-teams-apps-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="801a8-138">Java</span><span class="sxs-lookup"><span data-stu-id="801a8-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-installed-teams-apps-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="801a8-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="801a8-139">Response</span></span>

<span data-ttu-id="801a8-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="801a8-140">The following is an example of the response.</span></span>
><span data-ttu-id="801a8-141">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="801a8-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="801a8-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="801a8-142">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_installed_teams_apps",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

### <a name="example-2-get-the-names-and-other-details-of-installed-apps"></a><span data-ttu-id="801a8-143">Пример 2: получение имен и других сведений об установленных приложениях</span><span class="sxs-lookup"><span data-stu-id="801a8-143">Example 2: Get the names and other details of installed apps</span></span>

#### <a name="request"></a><span data-ttu-id="801a8-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="801a8-144">Request</span></span>

<span data-ttu-id="801a8-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="801a8-145">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="801a8-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="801a8-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_installed_teams_apps_expand"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{id}/installedApps?$expand=teamsAppDefinition
```
# <a name="c"></a>[<span data-ttu-id="801a8-147">C#</span><span class="sxs-lookup"><span data-stu-id="801a8-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-installed-teams-apps-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="801a8-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="801a8-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-installed-teams-apps-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="801a8-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="801a8-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-installed-teams-apps-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="801a8-150">Java</span><span class="sxs-lookup"><span data-stu-id="801a8-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-installed-teams-apps-expand-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="801a8-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="801a8-151">Response</span></span>

<span data-ttu-id="801a8-152">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="801a8-152">The following is an example of the response.</span></span>

><span data-ttu-id="801a8-153">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="801a8-153">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="801a8-154">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="801a8-154">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_installed_teams_apps_expand",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg=",
            "teamsAppDefinition": {
                "id": "MGQ4MjBlY2QtZGVmMi00Mjk3LWFkYWQtNzgwNTZjZGU3Yzc4IyMxLjAuMA==",
                "teamsAppId": "0d820ecd-def2-4297-adad-78056cde7c78",
                "displayName": "OneNote",
                "version": "1.0.0"
            }
        },
        {
            "id": "NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMwZmQ5MjVhMC0zNTdmLTRkMjUtODQ1Ni1iMzAyMmFhYTQxYTk=",
            "teamsAppDefinition": {
                "id": "MGZkOTI1YTAtMzU3Zi00ZDI1LTg0NTYtYjMwMjJhYWE0MWE5IyMxLjc=",
                "teamsAppId": "0fd925a0-357f-4d25-8456-b3022aaa41a9",
                "displayName": "SurveyMonkey",
                "version": "1.7"
            }
        },
        {
            "id": "NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMyYTUyNzcwMy0xZjZmLTQ1NTktYTMzMi1kOGE3ZDI4OGNkODg=",
            "teamsAppDefinition": {
                "id": "MmE1Mjc3MDMtMWY2Zi00NTU5LWEzMzItZDhhN2QyODhjZDg4IyMxLjA=",
                "teamsAppId": "2a527703-1f6f-4559-a332-d8a7d288cd88",
                "displayName": "SharePoint",
                "version": "1.0"
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

