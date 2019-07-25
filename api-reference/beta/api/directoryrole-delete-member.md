---
title: Удаление элемента роли каталога
description: Удаление элемента из объекта directoryRole.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c4ec110aa671ddd11327e515308929fb8865235f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35862308"
---
# <a name="remove-directory-role-member"></a><span data-ttu-id="cfe24-103">Удаление элемента роли каталога</span><span class="sxs-lookup"><span data-stu-id="cfe24-103">Remove directory role member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cfe24-104">Удаление элемента из объекта directoryRole.</span><span class="sxs-lookup"><span data-stu-id="cfe24-104">Remove a member from a directoryRole.</span></span>

## <a name="permissions"></a><span data-ttu-id="cfe24-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cfe24-105">Permissions</span></span>

<span data-ttu-id="cfe24-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cfe24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="cfe24-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cfe24-108">Permission type</span></span>      | <span data-ttu-id="cfe24-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cfe24-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cfe24-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cfe24-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cfe24-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cfe24-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cfe24-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cfe24-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cfe24-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cfe24-113">Not supported.</span></span>    |
|<span data-ttu-id="cfe24-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cfe24-114">Application</span></span> | <span data-ttu-id="cfe24-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cfe24-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cfe24-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cfe24-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directoryroles/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="cfe24-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cfe24-117">Request headers</span></span>

| <span data-ttu-id="cfe24-118">Имя</span><span class="sxs-lookup"><span data-stu-id="cfe24-118">Name</span></span>       | <span data-ttu-id="cfe24-119">Тип</span><span class="sxs-lookup"><span data-stu-id="cfe24-119">Type</span></span> | <span data-ttu-id="cfe24-120">Описание</span><span class="sxs-lookup"><span data-stu-id="cfe24-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cfe24-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cfe24-121">Authorization</span></span>  | <span data-ttu-id="cfe24-122">string</span><span class="sxs-lookup"><span data-stu-id="cfe24-122">string</span></span>  | <span data-ttu-id="cfe24-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cfe24-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cfe24-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cfe24-125">Request body</span></span>

<span data-ttu-id="cfe24-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cfe24-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cfe24-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="cfe24-127">Response</span></span>

<span data-ttu-id="cfe24-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="cfe24-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cfe24-130">Пример</span><span class="sxs-lookup"><span data-stu-id="cfe24-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="cfe24-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="cfe24-131">Request</span></span>

<span data-ttu-id="cfe24-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cfe24-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="cfe24-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="cfe24-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole"
}-->

```http
DELETE https://graph.microsoft.com/beta/directoryroles/{id}/members/{id}/$ref
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cfe24-134">C#</span><span class="sxs-lookup"><span data-stu-id="cfe24-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-from-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cfe24-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="cfe24-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-from-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cfe24-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="cfe24-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-from-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="cfe24-137">Java</span><span class="sxs-lookup"><span data-stu-id="cfe24-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directoryobject-from-directoryrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="cfe24-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="cfe24-138">Response</span></span>

<span data-ttu-id="cfe24-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cfe24-139">Here is an example of the response.</span></span> 
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
  "description": "Delete a member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
