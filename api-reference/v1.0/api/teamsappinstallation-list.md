---
title: Список приложений в команде
description: Получение списка приложений, установленных в указанной команде.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a961d849e62b40cd4017b9abe83a42535ddedd16
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893249"
---
# <a name="list-apps-in-team"></a><span data-ttu-id="dcc5e-103">Список приложений в команде</span><span class="sxs-lookup"><span data-stu-id="dcc5e-103">List apps in team</span></span>



<span data-ttu-id="dcc5e-104">Получение списка приложений, [установленных](../resources/teamsappinstallation.md) в указанной [команде](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="dcc5e-104">Retrieve the list of [apps installed](../resources/teamsappinstallation.md) in the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="dcc5e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dcc5e-105">Permissions</span></span>

<span data-ttu-id="dcc5e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dcc5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dcc5e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dcc5e-108">Permission type</span></span>      | <span data-ttu-id="dcc5e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dcc5e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dcc5e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dcc5e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dcc5e-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dcc5e-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="dcc5e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dcc5e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dcc5e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dcc5e-113">Not supported.</span></span>    |
|<span data-ttu-id="dcc5e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dcc5e-114">Application</span></span> | <span data-ttu-id="dcc5e-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dcc5e-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="dcc5e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dcc5e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/installedApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dcc5e-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="dcc5e-117">Optional query parameters</span></span>

<span data-ttu-id="dcc5e-118">Этот метод поддерживает [параметры запросов](/graph/query-parameters) $filter, $select и $Expand OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="dcc5e-118">This method supports the $filter, $select, and $expand [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dcc5e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dcc5e-119">Request headers</span></span>

| <span data-ttu-id="dcc5e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dcc5e-120">Header</span></span>       | <span data-ttu-id="dcc5e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="dcc5e-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="dcc5e-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dcc5e-122">Authorization</span></span>  | <span data-ttu-id="dcc5e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dcc5e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dcc5e-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dcc5e-125">Request body</span></span>

<span data-ttu-id="dcc5e-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dcc5e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dcc5e-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="dcc5e-127">Response</span></span>

<span data-ttu-id="dcc5e-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [teamsApp](../resources/teamsapp.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dcc5e-128">If successful, this method returns a `200 OK` response code and collection of [teamsApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dcc5e-129">Пример</span><span class="sxs-lookup"><span data-stu-id="dcc5e-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="dcc5e-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="dcc5e-130">Request</span></span>

<span data-ttu-id="dcc5e-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dcc5e-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="dcc5e-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="dcc5e-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_installed_teams_apps"
}-->

```http
GET /teams/{id}/installedApps
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dcc5e-133">C#</span><span class="sxs-lookup"><span data-stu-id="dcc5e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-installed-teams-apps-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dcc5e-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="dcc5e-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-installed-teams-apps-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dcc5e-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="dcc5e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-installed-teams-apps-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="dcc5e-136">Java</span><span class="sxs-lookup"><span data-stu-id="dcc5e-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-installed-teams-apps-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="dcc5e-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="dcc5e-137">Response</span></span>

<span data-ttu-id="dcc5e-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dcc5e-138">The following is an example of the response.</span></span>
><span data-ttu-id="dcc5e-139">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="dcc5e-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="dcc5e-140">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dcc5e-140">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

## <a name="example----getting-the-names-of-the-installed-apps"></a><span data-ttu-id="dcc5e-141">Пример: извлечение имен установленных приложений</span><span class="sxs-lookup"><span data-stu-id="dcc5e-141">Example -- getting the names of the installed apps</span></span>

### <a name="request"></a><span data-ttu-id="dcc5e-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="dcc5e-142">Request</span></span>

<span data-ttu-id="dcc5e-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dcc5e-143">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="dcc5e-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="dcc5e-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_installed_teams_apps_expand"
}-->

```http
GET https://graph.microsoft.com/v1.0/teams/{id}/installedApps?$expand=teamsAppDefinition
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dcc5e-145">C#</span><span class="sxs-lookup"><span data-stu-id="dcc5e-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-installed-teams-apps-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dcc5e-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="dcc5e-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-installed-teams-apps-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dcc5e-147">Цель — C</span><span class="sxs-lookup"><span data-stu-id="dcc5e-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-installed-teams-apps-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="dcc5e-148">Java</span><span class="sxs-lookup"><span data-stu-id="dcc5e-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-installed-teams-apps-expand-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="dcc5e-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="dcc5e-149">Response</span></span>

<span data-ttu-id="dcc5e-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dcc5e-150">The following is an example of the response.</span></span>

><span data-ttu-id="dcc5e-151">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="dcc5e-151">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="dcc5e-152">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dcc5e-152">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

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
