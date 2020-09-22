---
title: Обновление приложения в команде
description: Обновление установки приложения в команде
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6bf3a366b5e500bdd5fd928851ed2730e3280650
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47978372"
---
# <a name="upgrade-an-app-in-a-team"></a><span data-ttu-id="2bf1f-103">Обновление приложения в команде</span><span class="sxs-lookup"><span data-stu-id="2bf1f-103">Upgrade an app in a team</span></span>

<span data-ttu-id="2bf1f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2bf1f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2bf1f-105">Обновляет [установку приложения](../resources/teamsappinstallation.md) в [команде](../resources/team.md) до последней версии приложения.</span><span class="sxs-lookup"><span data-stu-id="2bf1f-105">Upgrades an [app installation](../resources/teamsappinstallation.md) in a [team](../resources/team.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="2bf1f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2bf1f-106">Permissions</span></span>

<span data-ttu-id="2bf1f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2bf1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2bf1f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2bf1f-109">Permission type</span></span>      | <span data-ttu-id="2bf1f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2bf1f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2bf1f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2bf1f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2bf1f-112">Теамсаппинсталлатион. Реадвритефортеам, Group. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="2bf1f-112">TeamsAppInstallation.ReadWriteForTeam, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="2bf1f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2bf1f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2bf1f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2bf1f-114">Not supported.</span></span>    |
|<span data-ttu-id="2bf1f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2bf1f-115">Application</span></span> | <span data-ttu-id="2bf1f-116">Теамсаппинсталлатион. Реадвритефортеам. ALL, Group. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="2bf1f-116">TeamsAppInstallation.ReadWriteForTeam.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2bf1f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2bf1f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps/{id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="2bf1f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2bf1f-118">Request headers</span></span>

| <span data-ttu-id="2bf1f-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2bf1f-119">Header</span></span>       | <span data-ttu-id="2bf1f-120">Значение</span><span class="sxs-lookup"><span data-stu-id="2bf1f-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2bf1f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2bf1f-121">Authorization</span></span>  | <span data-ttu-id="2bf1f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2bf1f-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2bf1f-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2bf1f-124">Request body</span></span>

<span data-ttu-id="2bf1f-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2bf1f-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2bf1f-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="2bf1f-126">Response</span></span>

<span data-ttu-id="2bf1f-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="2bf1f-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2bf1f-129">Пример</span><span class="sxs-lookup"><span data-stu-id="2bf1f-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="2bf1f-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="2bf1f-130">Request</span></span>

<span data-ttu-id="2bf1f-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2bf1f-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2bf1f-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="2bf1f-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "upgrade_teamsapp"
}-->

```http
POST /teams/{id}/installedApps/{id}/upgrade
```
# <a name="c"></a>[<span data-ttu-id="2bf1f-133">C#</span><span class="sxs-lookup"><span data-stu-id="2bf1f-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/upgrade-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2bf1f-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2bf1f-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/upgrade-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2bf1f-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2bf1f-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/upgrade-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2bf1f-136">Java</span><span class="sxs-lookup"><span data-stu-id="2bf1f-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/upgrade-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2bf1f-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="2bf1f-137">Response</span></span>

<span data-ttu-id="2bf1f-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2bf1f-138">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "name": "upgrade_teamsapp",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

