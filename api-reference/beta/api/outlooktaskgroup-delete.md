---
title: Удаление outlookTaskGroup
description: Удаление указанного outlookTaskGroup.
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 1128156f2df59e06600e47ca4b3d96f0cd296a10
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48974798"
---
# <a name="delete-outlooktaskgroup-deprecated"></a><span data-ttu-id="cae93-103">Delete outlookTaskGroup (устаревшее)</span><span class="sxs-lookup"><span data-stu-id="cae93-103">Delete outlookTaskGroup (deprecated)</span></span>

<span data-ttu-id="cae93-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cae93-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-allup](../../includes/outlooktask-deprecate-allup.md)]


<span data-ttu-id="cae93-105">Удаление указанного [outlookTaskGroup](../resources/outlooktaskgroup.md).</span><span class="sxs-lookup"><span data-stu-id="cae93-105">Delete the specified [outlookTaskGroup](../resources/outlooktaskgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="cae93-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cae93-106">Permissions</span></span>
<span data-ttu-id="cae93-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cae93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cae93-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cae93-109">Permission type</span></span>      | <span data-ttu-id="cae93-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cae93-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cae93-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cae93-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cae93-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cae93-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="cae93-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cae93-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cae93-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cae93-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="cae93-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cae93-115">Application</span></span> | <span data-ttu-id="cae93-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cae93-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cae93-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cae93-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/taskGroups/{id}
DELETE /users/{id|userPrincipalName}/outlook/taskGroups/{id}
```
## <a name="request-headers"></a><span data-ttu-id="cae93-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cae93-118">Request headers</span></span>
| <span data-ttu-id="cae93-119">Имя</span><span class="sxs-lookup"><span data-stu-id="cae93-119">Name</span></span>       | <span data-ttu-id="cae93-120">Описание</span><span class="sxs-lookup"><span data-stu-id="cae93-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cae93-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cae93-121">Authorization</span></span>  | <span data-ttu-id="cae93-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cae93-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cae93-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cae93-124">Request body</span></span>
<span data-ttu-id="cae93-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cae93-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cae93-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="cae93-126">Response</span></span>

<span data-ttu-id="cae93-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="cae93-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cae93-129">Пример</span><span class="sxs-lookup"><span data-stu-id="cae93-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cae93-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="cae93-130">Request</span></span>
<span data-ttu-id="cae93-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cae93-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cae93-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="cae93-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_outlooktaskgroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/outlook/taskgroups/AAMkADIyAAAhrbe-AAA=
```
# <a name="c"></a>[<span data-ttu-id="cae93-133">C#</span><span class="sxs-lookup"><span data-stu-id="cae93-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-outlooktaskgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cae93-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cae93-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-outlooktaskgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cae93-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cae93-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-outlooktaskgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cae93-136">Java</span><span class="sxs-lookup"><span data-stu-id="cae93-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-outlooktaskgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="cae93-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="cae93-137">Response</span></span>
<span data-ttu-id="cae93-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cae93-138">Here is an example of the response.</span></span>
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


