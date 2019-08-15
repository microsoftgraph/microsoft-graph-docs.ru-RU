---
title: Удаление приложения из группы
description: Удаляет приложение из указанной команды.
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8e86ef713cee1f638f626a3475afc341b9aa9cb5
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36421360"
---
# <a name="remove-app-from-team"></a><span data-ttu-id="4a26f-103">Удаление приложения из группы</span><span class="sxs-lookup"><span data-stu-id="4a26f-103">Remove app from team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a26f-104">Удаляет [приложение](../resources/teamsappinstallation.md) из указанной [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="4a26f-104">Uninstalls an [app](../resources/teamsappinstallation.md) from the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4a26f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4a26f-105">Permissions</span></span>

<span data-ttu-id="4a26f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a26f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a26f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a26f-108">Permission type</span></span>      | <span data-ttu-id="4a26f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a26f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a26f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a26f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4a26f-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a26f-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4a26f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a26f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a26f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a26f-113">Not supported.</span></span>    |
|<span data-ttu-id="4a26f-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4a26f-114">Application</span></span> | <span data-ttu-id="4a26f-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a26f-115">Group.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="4a26f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a26f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/installedApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4a26f-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4a26f-117">Request headers</span></span>

| <span data-ttu-id="4a26f-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4a26f-118">Header</span></span>       | <span data-ttu-id="4a26f-119">Значение</span><span class="sxs-lookup"><span data-stu-id="4a26f-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4a26f-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4a26f-120">Authorization</span></span>  | <span data-ttu-id="4a26f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a26f-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4a26f-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4a26f-123">Request body</span></span>

<span data-ttu-id="4a26f-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4a26f-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4a26f-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a26f-125">Response</span></span>

<span data-ttu-id="4a26f-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="4a26f-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a26f-128">Пример</span><span class="sxs-lookup"><span data-stu-id="4a26f-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="4a26f-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a26f-129">Request</span></span>

<span data-ttu-id="4a26f-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4a26f-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4a26f-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="4a26f-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "uninstall_teamsapp"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{id}/installedApps/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4a26f-132">C#</span><span class="sxs-lookup"><span data-stu-id="4a26f-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/uninstall-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4a26f-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4a26f-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/uninstall-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4a26f-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="4a26f-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/uninstall-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4a26f-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a26f-135">Response</span></span>

<span data-ttu-id="4a26f-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4a26f-136">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "name": "uninstall_teamsapp",
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
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
