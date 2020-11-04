---
title: Список приложений в команде
description: Получение списка приложений, установленных в указанной команде.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 35007111dd697a3568aa08b4a850263e0508d57a
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2020
ms.locfileid: "48848719"
---
# <a name="list-apps-in-team"></a><span data-ttu-id="b25a6-103">Список приложений в команде</span><span class="sxs-lookup"><span data-stu-id="b25a6-103">List apps in team</span></span>

<span data-ttu-id="b25a6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b25a6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b25a6-105">Получение списка приложений, [установленных](../resources/teamsappinstallation.md) в указанной [команде](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="b25a6-105">Retrieve the list of [apps installed](../resources/teamsappinstallation.md) in the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b25a6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b25a6-106">Permissions</span></span>

<span data-ttu-id="b25a6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b25a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b25a6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b25a6-109">Permission type</span></span>      | <span data-ttu-id="b25a6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b25a6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b25a6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b25a6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b25a6-112">Теамсаппинсталлатион. Реадфортеам, Теамсаппинсталлатион. Реадвритефортеам, Group. Read. ALL, Group. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="b25a6-112">TeamsAppInstallation.ReadForTeam, TeamsAppInstallation.ReadWriteForTeam, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="b25a6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b25a6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b25a6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b25a6-114">Not supported.</span></span>    |
|<span data-ttu-id="b25a6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b25a6-115">Application</span></span> | <span data-ttu-id="b25a6-116">Теамсаппинсталлатион. Read. Group \*, Теамсаппинсталлатион. Реадфортеам. ALL, Теамсаппинсталлатион. Реадвритефортеам. ALL, Group. Read. ALL, Group. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="b25a6-116">TeamsAppInstallation.Read.Group\*, TeamsAppInstallation.ReadForTeam.All, TeamsAppInstallation.ReadWriteForTeam.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="b25a6-117">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов]( https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="b25a6-117">**Note** : Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

## <a name="http-request"></a><span data-ttu-id="b25a6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b25a6-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/installedApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b25a6-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b25a6-119">Optional query parameters</span></span>

<span data-ttu-id="b25a6-120">Этот метод поддерживает [параметры запросов](/graph/query-parameters) $filter, $select и $Expand OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="b25a6-120">This method supports the $filter, $select, and $expand [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b25a6-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b25a6-121">Request headers</span></span>

| <span data-ttu-id="b25a6-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b25a6-122">Header</span></span>       | <span data-ttu-id="b25a6-123">Значение</span><span class="sxs-lookup"><span data-stu-id="b25a6-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b25a6-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b25a6-124">Authorization</span></span>  | <span data-ttu-id="b25a6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b25a6-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b25a6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b25a6-127">Request body</span></span>

<span data-ttu-id="b25a6-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b25a6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b25a6-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="b25a6-129">Response</span></span>

<span data-ttu-id="b25a6-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [теамсаппинсталлатион](../resources/teamsappinstallation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b25a6-130">If successful, this method returns a `200 OK` response code and collection of [teamsAppInstallation](../resources/teamsappinstallation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b25a6-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="b25a6-131">Examples</span></span>

### <a name="example-1-list-installed-apps"></a><span data-ttu-id="b25a6-132">Пример 1: список установленных приложений</span><span class="sxs-lookup"><span data-stu-id="b25a6-132">Example 1: List installed apps</span></span>
#### <a name="request"></a><span data-ttu-id="b25a6-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b25a6-133">Request</span></span>

<span data-ttu-id="b25a6-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b25a6-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b25a6-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="b25a6-135">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_installed_teams_apps"
}-->

```msgraph-interactive
GET /teams/{id}/installedApps
```
# <a name="c"></a>[<span data-ttu-id="b25a6-136">C#</span><span class="sxs-lookup"><span data-stu-id="b25a6-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-installed-teams-apps-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b25a6-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b25a6-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-installed-teams-apps-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b25a6-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b25a6-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-installed-teams-apps-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b25a6-139">Java</span><span class="sxs-lookup"><span data-stu-id="b25a6-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-installed-teams-apps-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="b25a6-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="b25a6-140">Response</span></span>

<span data-ttu-id="b25a6-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b25a6-141">The following is an example of the response.</span></span>
><span data-ttu-id="b25a6-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b25a6-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

### <a name="example-2-get-the-names-and-other-details-of-installed-apps"></a><span data-ttu-id="b25a6-144">Пример 2: получение имен и других сведений об установленных приложениях</span><span class="sxs-lookup"><span data-stu-id="b25a6-144">Example 2: Get the names and other details of installed apps</span></span>

#### <a name="request"></a><span data-ttu-id="b25a6-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="b25a6-145">Request</span></span>

<span data-ttu-id="b25a6-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b25a6-146">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b25a6-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="b25a6-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_installed_teams_apps_expand"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{id}/installedApps?$expand=teamsAppDefinition
```
# <a name="c"></a>[<span data-ttu-id="b25a6-148">C#</span><span class="sxs-lookup"><span data-stu-id="b25a6-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-installed-teams-apps-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b25a6-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b25a6-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-installed-teams-apps-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b25a6-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b25a6-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-installed-teams-apps-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b25a6-151">Java</span><span class="sxs-lookup"><span data-stu-id="b25a6-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-installed-teams-apps-expand-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="b25a6-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="b25a6-152">Response</span></span>

<span data-ttu-id="b25a6-153">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b25a6-153">The following is an example of the response.</span></span>

><span data-ttu-id="b25a6-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b25a6-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

