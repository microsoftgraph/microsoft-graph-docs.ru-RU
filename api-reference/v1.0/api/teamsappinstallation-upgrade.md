---
title: Обновление приложения в команде
description: Обновление установки приложения в команде
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 987907552f691de3fe0861323b770c7d72fc64f5
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932413"
---
# <a name="upgrade-an-app-in-a-team"></a><span data-ttu-id="3acde-103">Обновление приложения в команде</span><span class="sxs-lookup"><span data-stu-id="3acde-103">Upgrade an app in a team</span></span>

<span data-ttu-id="3acde-104">Обновляет [установку приложения](../resources/teamsappinstallation.md) в [команде](../resources/team.md) до последней версии приложения.</span><span class="sxs-lookup"><span data-stu-id="3acde-104">Upgrades an [app installation](../resources/teamsappinstallation.md) in a [team](../resources/team.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="3acde-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3acde-105">Permissions</span></span>

<span data-ttu-id="3acde-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3acde-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3acde-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3acde-108">Permission type</span></span>      | <span data-ttu-id="3acde-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3acde-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3acde-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3acde-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3acde-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3acde-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3acde-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3acde-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3acde-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3acde-113">Not supported.</span></span>    |
|<span data-ttu-id="3acde-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3acde-114">Application</span></span> | <span data-ttu-id="3acde-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3acde-115">Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="3acde-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3acde-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/installedApps/{id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="3acde-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3acde-117">Request headers</span></span>

| <span data-ttu-id="3acde-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3acde-118">Header</span></span>       | <span data-ttu-id="3acde-119">Значение</span><span class="sxs-lookup"><span data-stu-id="3acde-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3acde-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3acde-120">Authorization</span></span>  | <span data-ttu-id="3acde-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3acde-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3acde-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3acde-123">Request body</span></span>

<span data-ttu-id="3acde-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3acde-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3acde-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="3acde-125">Response</span></span>

<span data-ttu-id="3acde-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="3acde-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3acde-128">Пример</span><span class="sxs-lookup"><span data-stu-id="3acde-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="3acde-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="3acde-129">Request</span></span>

<span data-ttu-id="3acde-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3acde-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3acde-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="3acde-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "upgrade_teamsapp"
}-->

```http
POST /teams/{id}/installedApps/{id}/upgrade
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3acde-132">C#</span><span class="sxs-lookup"><span data-stu-id="3acde-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/upgrade-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3acde-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="3acde-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/upgrade-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3acde-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="3acde-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/upgrade-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3acde-135">Java</span><span class="sxs-lookup"><span data-stu-id="3acde-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/upgrade-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3acde-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="3acde-136">Response</span></span>

<span data-ttu-id="3acde-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3acde-137">The following is an example of the response.</span></span> 

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
