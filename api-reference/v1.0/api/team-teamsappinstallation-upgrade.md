---
title: 'teamsAppInstallation в команде: обновление'
description: Обновление установки приложения в команде
author: akjo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4c3df922e9fc15238bb5531fc38a935f613b1c98
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060023"
---
# <a name="teamsappinstallation-in-team-upgrade"></a><span data-ttu-id="11cb4-103">teamsAppInstallation в команде: обновление</span><span class="sxs-lookup"><span data-stu-id="11cb4-103">teamsAppInstallation in team: upgrade</span></span>

<span data-ttu-id="11cb4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11cb4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="11cb4-105">Обновление [установки приложения](../resources/teamsappinstallation.md) в [команде до](../resources/team.md) последней версии приложения.</span><span class="sxs-lookup"><span data-stu-id="11cb4-105">Upgrade an [app installation](../resources/teamsappinstallation.md) in a [team](../resources/team.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="11cb4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="11cb4-106">Permissions</span></span>

<span data-ttu-id="11cb4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11cb4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11cb4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="11cb4-109">Permission type</span></span>      | <span data-ttu-id="11cb4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="11cb4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="11cb4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="11cb4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="11cb4-112">TeamsAppInstallation.ReadWriteForTeam, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11cb4-112">TeamsAppInstallation.ReadWriteForTeam, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="11cb4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="11cb4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11cb4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11cb4-114">Not supported.</span></span>    |
|<span data-ttu-id="11cb4-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="11cb4-115">Application</span></span> | <span data-ttu-id="11cb4-116">TeamsAppInstallation.ReadWriteForTeam.All, Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11cb4-116">TeamsAppInstallation.ReadWriteForTeam.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="11cb4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="11cb4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{team-id}/installedApps/{app-installation-id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="11cb4-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="11cb4-118">Request headers</span></span>

| <span data-ttu-id="11cb4-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="11cb4-119">Header</span></span>       | <span data-ttu-id="11cb4-120">Значение</span><span class="sxs-lookup"><span data-stu-id="11cb4-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="11cb4-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="11cb4-121">Authorization</span></span>  | <span data-ttu-id="11cb4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="11cb4-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="11cb4-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="11cb4-124">Request body</span></span>

<span data-ttu-id="11cb4-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="11cb4-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="11cb4-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="11cb4-126">Response</span></span>

<span data-ttu-id="11cb4-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="11cb4-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11cb4-129">Пример</span><span class="sxs-lookup"><span data-stu-id="11cb4-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="11cb4-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="11cb4-130">Request</span></span>

<span data-ttu-id="11cb4-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="11cb4-131">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="11cb4-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="11cb4-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "upgrade_teamsapp_in_team"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/db5e04be-daa2-4a35-beb1-5e73cc381599/installedApps/NjkwM2ZhOTMtNjA1Yi00M2VmLTkyMGUtNzdjNDcyOWY4MjU4IyMwMjQwYTM2OC0yNWUwLTQ1NjktOGViZS0xMzYwMWNiNTVhMTg=/upgrade
```
# <a name="c"></a>[<span data-ttu-id="11cb4-133">C#</span><span class="sxs-lookup"><span data-stu-id="11cb4-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/upgrade-teamsapp-in-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="11cb4-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="11cb4-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/upgrade-teamsapp-in-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="11cb4-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="11cb4-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/upgrade-teamsapp-in-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="11cb4-136">Java</span><span class="sxs-lookup"><span data-stu-id="11cb4-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/upgrade-teamsapp-in-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="11cb4-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="11cb4-137">Response</span></span>

<span data-ttu-id="11cb4-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="11cb4-138">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "name": "upgrade_teamsapp_in_team",
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
  "description": "Upgrade app in team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


