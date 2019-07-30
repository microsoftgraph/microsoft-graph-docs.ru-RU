---
title: Удаление приложения из группы
description: Удаляет приложение из указанной команды.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 59caed63c53dacd86b6303dfdf29ad018e0f4677
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932449"
---
# <a name="remove-app-from-team"></a><span data-ttu-id="c2ace-103">Удаление приложения из группы</span><span class="sxs-lookup"><span data-stu-id="c2ace-103">Remove app from team</span></span>

<span data-ttu-id="c2ace-104">Удаляет [приложение](../resources/teamsappinstallation.md) из указанной [команды](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="c2ace-104">Uninstalls an [app](../resources/teamsappinstallation.md) from the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c2ace-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c2ace-105">Permissions</span></span>

<span data-ttu-id="c2ace-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2ace-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2ace-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2ace-108">Permission type</span></span>      | <span data-ttu-id="c2ace-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2ace-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2ace-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2ace-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c2ace-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2ace-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c2ace-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2ace-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2ace-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2ace-113">Not supported.</span></span>    |
|<span data-ttu-id="c2ace-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c2ace-114">Application</span></span> | <span data-ttu-id="c2ace-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2ace-115">Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="c2ace-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2ace-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /teams/{id}/installedApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c2ace-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c2ace-117">Request headers</span></span>

| <span data-ttu-id="c2ace-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c2ace-118">Header</span></span>       | <span data-ttu-id="c2ace-119">Значение</span><span class="sxs-lookup"><span data-stu-id="c2ace-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c2ace-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c2ace-120">Authorization</span></span>  | <span data-ttu-id="c2ace-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c2ace-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c2ace-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c2ace-123">Request body</span></span>

<span data-ttu-id="c2ace-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c2ace-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2ace-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2ace-125">Response</span></span>

<span data-ttu-id="c2ace-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c2ace-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2ace-128">Пример</span><span class="sxs-lookup"><span data-stu-id="c2ace-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="c2ace-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2ace-129">Request</span></span>

<span data-ttu-id="c2ace-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2ace-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c2ace-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="c2ace-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "uninstall_teamsapp"
}-->

```http
DELETE /teams/{id}/installedApps/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c2ace-132">C#</span><span class="sxs-lookup"><span data-stu-id="c2ace-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/uninstall-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c2ace-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="c2ace-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/uninstall-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c2ace-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c2ace-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/uninstall-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c2ace-135">Java</span><span class="sxs-lookup"><span data-stu-id="c2ace-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/uninstall-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c2ace-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2ace-136">Response</span></span>

<span data-ttu-id="c2ace-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c2ace-137">The following is an example of the response.</span></span> 
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
<!-- {
  "type": "#page.annotation",
  "description": "Get team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
