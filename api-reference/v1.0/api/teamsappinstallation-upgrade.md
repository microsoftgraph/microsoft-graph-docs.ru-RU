---
title: Обновление приложения в команде
description: Обновление установки приложения в команде
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8525ae7afa33f34d3630a8b5fbac53b3d89dedbc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027281"
---
# <a name="upgrade-an-app-in-a-team"></a><span data-ttu-id="99073-103">Обновление приложения в команде</span><span class="sxs-lookup"><span data-stu-id="99073-103">Upgrade an app in a team</span></span>

<span data-ttu-id="99073-104">Обновляет [установку приложения](../resources/teamsappinstallation.md) в [команде](../resources/team.md) до последней версии приложения.</span><span class="sxs-lookup"><span data-stu-id="99073-104">Upgrades an [app installation](../resources/teamsappinstallation.md) in a [team](../resources/team.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="99073-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="99073-105">Permissions</span></span>

<span data-ttu-id="99073-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99073-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99073-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="99073-108">Permission type</span></span>      | <span data-ttu-id="99073-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="99073-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="99073-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="99073-110">Delegated (work or school account)</span></span> | <span data-ttu-id="99073-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99073-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="99073-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="99073-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99073-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99073-113">Not supported.</span></span>    |
|<span data-ttu-id="99073-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="99073-114">Application</span></span> | <span data-ttu-id="99073-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99073-115">Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="99073-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="99073-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps/{id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="99073-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="99073-117">Request headers</span></span>

| <span data-ttu-id="99073-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="99073-118">Header</span></span>       | <span data-ttu-id="99073-119">Значение</span><span class="sxs-lookup"><span data-stu-id="99073-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="99073-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="99073-120">Authorization</span></span>  | <span data-ttu-id="99073-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="99073-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="99073-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="99073-123">Request body</span></span>

<span data-ttu-id="99073-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="99073-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="99073-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="99073-125">Response</span></span>

<span data-ttu-id="99073-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="99073-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99073-128">Пример</span><span class="sxs-lookup"><span data-stu-id="99073-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="99073-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="99073-129">Request</span></span>

<span data-ttu-id="99073-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="99073-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="99073-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="99073-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "upgrade_teamsapp"
}-->

```http
POST /teams/{id}/installedApps/{id}/upgrade
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="99073-132">C#</span><span class="sxs-lookup"><span data-stu-id="99073-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/upgrade-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="99073-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="99073-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/upgrade-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="99073-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="99073-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/upgrade-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="99073-135">Java</span><span class="sxs-lookup"><span data-stu-id="99073-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/upgrade-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="99073-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="99073-136">Response</span></span>

<span data-ttu-id="99073-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="99073-137">The following is an example of the response.</span></span> 

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
