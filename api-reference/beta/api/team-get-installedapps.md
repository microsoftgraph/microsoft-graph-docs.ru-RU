---
title: Получить установленное приложение в команде
description: Получите приложение, установленное в команде.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3a46a661dd324331a15e334548825af8af0180f2
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659557"
---
# <a name="get-installed-app-in-team"></a><span data-ttu-id="f439d-103">Получить установленное приложение в команде</span><span class="sxs-lookup"><span data-stu-id="f439d-103">Get installed app in team</span></span>

<span data-ttu-id="f439d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f439d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f439d-105">Извлекать [приложение,](../resources/teamsappinstallation.md) установленное в указанной [команде.](../resources/team.md)</span><span class="sxs-lookup"><span data-stu-id="f439d-105">Retrieve the [app](../resources/teamsappinstallation.md) installed in the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f439d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f439d-106">Permissions</span></span>

<span data-ttu-id="f439d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f439d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f439d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f439d-109">Permission type</span></span>      | <span data-ttu-id="f439d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f439d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f439d-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f439d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f439d-112">TeamsAppInstallation.ReadWriteSelfForTeam, TeamsAppInstallation.ReadForUser, TeamsAppInstallation.ReadForTeam, TeamsAppInstallation.ReadWriteForTeam, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f439d-112">TeamsAppInstallation.ReadWriteSelfForTeam, TeamsAppInstallation.ReadForUser, TeamsAppInstallation.ReadForTeam, TeamsAppInstallation.ReadWriteForTeam, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="f439d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f439d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f439d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f439d-114">Not supported.</span></span>    |
|<span data-ttu-id="f439d-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="f439d-115">Application</span></span> | <span data-ttu-id="f439d-116">TeamsAppInstallation.ReadWriteSelfForTeam, TeamsAppInstallation.ReadForTeam.All, TeamsAppInstallation.ReadWriteForTeam.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f439d-116">TeamsAppInstallation.ReadWriteSelfForTeam, TeamsAppInstallation.ReadForTeam.All, TeamsAppInstallation.ReadWriteForTeam.All, Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f439d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f439d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/installedApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f439d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f439d-118">Request headers</span></span>

| <span data-ttu-id="f439d-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f439d-119">Header</span></span>       | <span data-ttu-id="f439d-120">Значение</span><span class="sxs-lookup"><span data-stu-id="f439d-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f439d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f439d-121">Authorization</span></span>  | <span data-ttu-id="f439d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f439d-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f439d-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f439d-124">Request body</span></span>

<span data-ttu-id="f439d-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f439d-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f439d-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="f439d-126">Response</span></span>

<span data-ttu-id="f439d-127">В случае успеха этот метод возвращает код отклика и объект `200 OK` [teamsAppInstallation](../resources/teamsappinstallation.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f439d-127">If successful, this method returns a `200 OK` response code and a [teamsAppInstallation](../resources/teamsappinstallation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f439d-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="f439d-128">Examples</span></span>

### <a name="example-1-get-the-installed-app"></a><span data-ttu-id="f439d-129">Пример 1. Получите установленное приложение</span><span class="sxs-lookup"><span data-stu-id="f439d-129">Example 1: Get the installed app</span></span>
#### <a name="request"></a><span data-ttu-id="f439d-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="f439d-130">Request</span></span>

<span data-ttu-id="f439d-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f439d-131">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f439d-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="f439d-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_installed_teams_apps"
}-->

```msgraph-interactive
GET /teams/{id}/installedApps/{id}
```
# <a name="c"></a>[<span data-ttu-id="f439d-133">C#</span><span class="sxs-lookup"><span data-stu-id="f439d-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-installed-teams-apps-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f439d-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f439d-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-installed-teams-apps-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f439d-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f439d-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-installed-teams-apps-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f439d-136">Java</span><span class="sxs-lookup"><span data-stu-id="f439d-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-installed-teams-apps-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="f439d-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="f439d-137">Response</span></span>

<span data-ttu-id="f439d-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f439d-138">The following is an example of the response.</span></span>
><span data-ttu-id="f439d-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f439d-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_installed_teams_apps",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "isCollection": false
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

### <a name="example-2-get-the-names-and-other-details-of-the-installed-app"></a><span data-ttu-id="f439d-141">Пример 2. Просмотр имен и других сведений об установленном приложении</span><span class="sxs-lookup"><span data-stu-id="f439d-141">Example 2: Get the names and other details of the installed app</span></span>

#### <a name="request"></a><span data-ttu-id="f439d-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="f439d-142">Request</span></span>

<span data-ttu-id="f439d-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f439d-143">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f439d-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="f439d-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_installed_teams_apps_expand"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{id}/installedApps/{id}?$expand=teamsAppDefinition
```
# <a name="c"></a>[<span data-ttu-id="f439d-145">C#</span><span class="sxs-lookup"><span data-stu-id="f439d-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-installed-teams-apps-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f439d-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f439d-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-installed-teams-apps-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f439d-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f439d-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-installed-teams-apps-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f439d-148">Java</span><span class="sxs-lookup"><span data-stu-id="f439d-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-installed-teams-apps-expand-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="f439d-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="f439d-149">Response</span></span>

<span data-ttu-id="f439d-150">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f439d-150">The following is an example of the response.</span></span>

><span data-ttu-id="f439d-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f439d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_installed_teams_apps_expand",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "isCollection": false
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
                "version": "beta"
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

