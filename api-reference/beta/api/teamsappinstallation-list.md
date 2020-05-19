---
title: Список приложений в команде
description: Получение списка приложений, установленных в указанной команде.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ae4e60a824189e24f8347d352c5f6f5b42528eeb
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289930"
---
# <a name="list-apps-in-team"></a><span data-ttu-id="d74b0-103">Список приложений в команде</span><span class="sxs-lookup"><span data-stu-id="d74b0-103">List apps in team</span></span>

<span data-ttu-id="d74b0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d74b0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d74b0-105">Получение списка приложений, [установленных](../resources/teamsappinstallation.md) в указанной [команде](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="d74b0-105">Retrieve the list of [apps installed](../resources/teamsappinstallation.md) in the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d74b0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d74b0-106">Permissions</span></span>

<span data-ttu-id="d74b0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d74b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d74b0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d74b0-109">Permission type</span></span>      | <span data-ttu-id="d74b0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d74b0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d74b0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d74b0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d74b0-112">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d74b0-112">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="d74b0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d74b0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d74b0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d74b0-114">Not supported.</span></span>    |
|<span data-ttu-id="d74b0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d74b0-115">Application</span></span> | <span data-ttu-id="d74b0-116">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d74b0-116">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d74b0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d74b0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/installedApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d74b0-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d74b0-118">Optional query parameters</span></span>

<span data-ttu-id="d74b0-119">Этот метод поддерживает [параметры запросов](/graph/query-parameters) $filter, $select и $Expand OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="d74b0-119">This method supports the $filter, $select, and $expand [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d74b0-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d74b0-120">Request headers</span></span>

| <span data-ttu-id="d74b0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d74b0-121">Header</span></span>       | <span data-ttu-id="d74b0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d74b0-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d74b0-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d74b0-123">Authorization</span></span>  | <span data-ttu-id="d74b0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d74b0-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d74b0-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d74b0-126">Request body</span></span>

<span data-ttu-id="d74b0-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d74b0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d74b0-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="d74b0-128">Response</span></span>

<span data-ttu-id="d74b0-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [теамсаппинсталлатион](../resources/teamsappinstallation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d74b0-129">If successful, this method returns a `200 OK` response code and collection of [teamsAppInstallation](../resources/teamsappinstallation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d74b0-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="d74b0-130">Examples</span></span>

### <a name="example-1-list-installed-apps"></a><span data-ttu-id="d74b0-131">Пример 1: список установленных приложений</span><span class="sxs-lookup"><span data-stu-id="d74b0-131">Example 1: List installed apps</span></span>

#### <a name="request"></a><span data-ttu-id="d74b0-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="d74b0-132">Request</span></span>

<span data-ttu-id="d74b0-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d74b0-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d74b0-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="d74b0-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_installed_teams_apps"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{id}/installedApps
```

# <a name="c"></a>[<span data-ttu-id="d74b0-135">C#</span><span class="sxs-lookup"><span data-stu-id="d74b0-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-installed-teams-apps-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d74b0-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d74b0-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-installed-teams-apps-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d74b0-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d74b0-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-installed-teams-apps-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="d74b0-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="d74b0-138">Response</span></span>

<span data-ttu-id="d74b0-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d74b0-139">The following is an example of the response.</span></span>
><span data-ttu-id="d74b0-140">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d74b0-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d74b0-141">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d74b0-141">All the properties will be returned from an actual call.</span></span>
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

### <a name="example-2-get-the-names-and-other-details-of-installed-apps"></a><span data-ttu-id="d74b0-142">Пример 2: получение имен и других сведений об установленных приложениях</span><span class="sxs-lookup"><span data-stu-id="d74b0-142">Example 2: Get the names and other details of installed apps</span></span>

#### <a name="request"></a><span data-ttu-id="d74b0-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="d74b0-143">Request</span></span>

<span data-ttu-id="d74b0-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d74b0-144">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d74b0-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="d74b0-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_installed_teams_apps_expand"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{id}/installedApps?$expand=teamsAppDefinition
```
# <a name="c"></a>[<span data-ttu-id="d74b0-146">C#</span><span class="sxs-lookup"><span data-stu-id="d74b0-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-installed-teams-apps-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d74b0-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d74b0-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-installed-teams-apps-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d74b0-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d74b0-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-installed-teams-apps-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d74b0-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="d74b0-149">Response</span></span>

<span data-ttu-id="d74b0-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d74b0-150">The following is an example of the response.</span></span>

><span data-ttu-id="d74b0-151">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d74b0-151">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d74b0-152">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d74b0-152">All the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
