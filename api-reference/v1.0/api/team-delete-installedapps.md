---
title: Удаление приложения из группы
description: Uninstalls an app from the specified team.
author: akjo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 768c7e58ff55ff01b48462c3ff621a95f066a247
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/22/2021
ms.locfileid: "53059460"
---
# <a name="remove-app-from-team"></a><span data-ttu-id="53bd7-103">Удаление приложения из группы</span><span class="sxs-lookup"><span data-stu-id="53bd7-103">Remove app from team</span></span>

<span data-ttu-id="53bd7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53bd7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53bd7-105">Uninstalls an [app](../resources/teamsappinstallation.md) from the specified [team.](../resources/team.md)</span><span class="sxs-lookup"><span data-stu-id="53bd7-105">Uninstalls an [app](../resources/teamsappinstallation.md) from the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="53bd7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="53bd7-106">Permissions</span></span>

<span data-ttu-id="53bd7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53bd7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53bd7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="53bd7-109">Permission type</span></span>      | <span data-ttu-id="53bd7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="53bd7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53bd7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="53bd7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="53bd7-112">TeamsAppInstallation.ReadWriteForTeam, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53bd7-112">TeamsAppInstallation.ReadWriteForTeam, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="53bd7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="53bd7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53bd7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53bd7-114">Not supported.</span></span>    |
|<span data-ttu-id="53bd7-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="53bd7-115">Application</span></span> | <span data-ttu-id="53bd7-116">TeamsAppInstallation.ReadWriteForTeam.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53bd7-116">TeamsAppInstallation.ReadWriteForTeam.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="53bd7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="53bd7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{team-id}/installedApps/{app-installation-id}
```

## <a name="request-headers"></a><span data-ttu-id="53bd7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="53bd7-118">Request headers</span></span>

| <span data-ttu-id="53bd7-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="53bd7-119">Header</span></span>       | <span data-ttu-id="53bd7-120">Значение</span><span class="sxs-lookup"><span data-stu-id="53bd7-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="53bd7-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="53bd7-121">Authorization</span></span>  | <span data-ttu-id="53bd7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="53bd7-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="53bd7-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="53bd7-124">Request body</span></span>

<span data-ttu-id="53bd7-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="53bd7-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53bd7-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="53bd7-126">Response</span></span>

<span data-ttu-id="53bd7-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="53bd7-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53bd7-129">Пример</span><span class="sxs-lookup"><span data-stu-id="53bd7-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="53bd7-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="53bd7-130">Request</span></span>

<span data-ttu-id="53bd7-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="53bd7-131">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="53bd7-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="53bd7-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "uninstall_teamsapp_in_team"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/teams/6903fa93-605b-43ef-920e-77c4729f8258/installedApps/NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwMDAwMTAxNi1kZTA1LTQ5MmUtOTEwNi00ODI4ZmM4YTg2ODc=
```
# <a name="c"></a>[<span data-ttu-id="53bd7-133">C#</span><span class="sxs-lookup"><span data-stu-id="53bd7-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/uninstall-teamsapp-in-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="53bd7-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="53bd7-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/uninstall-teamsapp-in-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="53bd7-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="53bd7-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/uninstall-teamsapp-in-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="53bd7-136">Java</span><span class="sxs-lookup"><span data-stu-id="53bd7-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/uninstall-teamsapp-in-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="53bd7-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="53bd7-137">Response</span></span>

<span data-ttu-id="53bd7-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="53bd7-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "name": "uninstall_teamsapp_in_team",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Remove app from team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


