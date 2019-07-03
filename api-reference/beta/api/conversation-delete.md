---
title: Удаление беседы
description: Удаление беседы.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: adb4f4e626eaf23da48e7bf6287057e14719b49f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35437482"
---
# <a name="delete-conversation"></a><span data-ttu-id="a059c-103">Удаление беседы</span><span class="sxs-lookup"><span data-stu-id="a059c-103">Delete conversation</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a059c-104">Удаление беседы.</span><span class="sxs-lookup"><span data-stu-id="a059c-104">Delete conversation.</span></span>
## <a name="permissions"></a><span data-ttu-id="a059c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a059c-105">Permissions</span></span>
<span data-ttu-id="a059c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a059c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a059c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a059c-108">Permission type</span></span>      | <span data-ttu-id="a059c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a059c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a059c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a059c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a059c-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a059c-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a059c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a059c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a059c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a059c-113">Not supported.</span></span>    |
|<span data-ttu-id="a059c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a059c-114">Application</span></span> | <span data-ttu-id="a059c-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a059c-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a059c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a059c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/conversations/{id}
```
## <a name="request-headers"></a><span data-ttu-id="a059c-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a059c-117">Request headers</span></span>
| <span data-ttu-id="a059c-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a059c-118">Header</span></span>       | <span data-ttu-id="a059c-119">Значение</span><span class="sxs-lookup"><span data-stu-id="a059c-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a059c-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a059c-120">Authorization</span></span>  | <span data-ttu-id="a059c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a059c-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a059c-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a059c-123">Request body</span></span>
<span data-ttu-id="a059c-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a059c-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a059c-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="a059c-125">Response</span></span>

<span data-ttu-id="a059c-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a059c-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a059c-128">Пример</span><span class="sxs-lookup"><span data-stu-id="a059c-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a059c-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="a059c-129">Request</span></span>
<span data-ttu-id="a059c-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a059c-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a059c-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="a059c-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_conversation"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/conversations/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a059c-132">C#</span><span class="sxs-lookup"><span data-stu-id="a059c-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-conversation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a059c-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="a059c-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-conversation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a059c-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="a059c-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-conversation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a059c-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="a059c-135">Response</span></span>
<span data-ttu-id="a059c-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a059c-136">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
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
  "description": "Delete conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
