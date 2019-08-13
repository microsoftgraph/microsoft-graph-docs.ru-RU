---
title: Удаление outlookTaskGroup
description: Удаление указанного outlookTaskGroup.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 54707253b90a1e070542b056fac6ef9001fad1f2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36349770"
---
# <a name="delete-outlooktaskgroup"></a><span data-ttu-id="28398-103">Удаление outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="28398-103">Delete outlookTaskGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28398-104">Удаление указанного [outlookTaskGroup](../resources/outlooktaskgroup.md).</span><span class="sxs-lookup"><span data-stu-id="28398-104">Delete the specified [outlookTaskGroup](../resources/outlooktaskgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="28398-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="28398-105">Permissions</span></span>
<span data-ttu-id="28398-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28398-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28398-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="28398-108">Permission type</span></span>      | <span data-ttu-id="28398-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="28398-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="28398-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="28398-110">Delegated (work or school account)</span></span> | <span data-ttu-id="28398-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="28398-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="28398-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="28398-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28398-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="28398-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="28398-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="28398-114">Application</span></span> | <span data-ttu-id="28398-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28398-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="28398-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="28398-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/taskGroups/{id}
DELETE /users/{id|userPrincipalName}/outlook/taskGroups/{id}
```
## <a name="request-headers"></a><span data-ttu-id="28398-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="28398-117">Request headers</span></span>
| <span data-ttu-id="28398-118">Имя</span><span class="sxs-lookup"><span data-stu-id="28398-118">Name</span></span>       | <span data-ttu-id="28398-119">Описание</span><span class="sxs-lookup"><span data-stu-id="28398-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="28398-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="28398-120">Authorization</span></span>  | <span data-ttu-id="28398-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="28398-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="28398-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="28398-123">Request body</span></span>
<span data-ttu-id="28398-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="28398-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="28398-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="28398-125">Response</span></span>

<span data-ttu-id="28398-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="28398-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28398-128">Пример</span><span class="sxs-lookup"><span data-stu-id="28398-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="28398-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="28398-129">Request</span></span>
<span data-ttu-id="28398-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="28398-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="28398-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="28398-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_outlooktaskgroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/outlook/taskgroups/AAMkADIyAAAhrbe-AAA=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="28398-132">C#</span><span class="sxs-lookup"><span data-stu-id="28398-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-outlooktaskgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="28398-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="28398-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-outlooktaskgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="28398-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="28398-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-outlooktaskgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="28398-135">Java</span><span class="sxs-lookup"><span data-stu-id="28398-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-outlooktaskgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="28398-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="28398-136">Response</span></span>
<span data-ttu-id="28398-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="28398-137">Here is an example of the response.</span></span>
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
  "description": "Delete outlookTaskGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
