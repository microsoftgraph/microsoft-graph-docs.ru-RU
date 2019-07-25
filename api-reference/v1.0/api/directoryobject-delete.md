---
title: Удаление объекта directoryObject
description: Удаляет directoryObject.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 07055c2ea3a33a96c5f7899032acc49064b64073
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35882736"
---
# <a name="delete-directoryobject"></a><span data-ttu-id="b8bba-103">Удаление объекта directoryObject</span><span class="sxs-lookup"><span data-stu-id="b8bba-103">Delete directoryObject</span></span>

<span data-ttu-id="b8bba-104">Удаляет directoryObject.</span><span class="sxs-lookup"><span data-stu-id="b8bba-104">Deletes a directoryObject.</span></span>

## <a name="permissions"></a><span data-ttu-id="b8bba-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b8bba-105">Permissions</span></span>
<span data-ttu-id="b8bba-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8bba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b8bba-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b8bba-108">Permission type</span></span>      | <span data-ttu-id="b8bba-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b8bba-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b8bba-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b8bba-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b8bba-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b8bba-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b8bba-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b8bba-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8bba-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8bba-113">Not supported.</span></span>    |
|<span data-ttu-id="b8bba-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b8bba-114">Application</span></span> | <span data-ttu-id="b8bba-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8bba-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b8bba-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b8bba-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directoryObjects/{id}

```
## <a name="request-headers"></a><span data-ttu-id="b8bba-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b8bba-117">Request headers</span></span>
| <span data-ttu-id="b8bba-118">Имя</span><span class="sxs-lookup"><span data-stu-id="b8bba-118">Name</span></span>       | <span data-ttu-id="b8bba-119">Тип</span><span class="sxs-lookup"><span data-stu-id="b8bba-119">Type</span></span> | <span data-ttu-id="b8bba-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b8bba-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b8bba-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8bba-121">Authorization</span></span>  | <span data-ttu-id="b8bba-122">string</span><span class="sxs-lookup"><span data-stu-id="b8bba-122">string</span></span>  | <span data-ttu-id="b8bba-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b8bba-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b8bba-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b8bba-125">Request body</span></span>
<span data-ttu-id="b8bba-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b8bba-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8bba-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8bba-127">Response</span></span>

<span data-ttu-id="b8bba-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="b8bba-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8bba-130">Пример</span><span class="sxs-lookup"><span data-stu-id="b8bba-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b8bba-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="b8bba-131">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b8bba-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="b8bba-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directoryObjects/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b8bba-133">C#</span><span class="sxs-lookup"><span data-stu-id="b8bba-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b8bba-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="b8bba-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b8bba-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b8bba-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b8bba-136">Java</span><span class="sxs-lookup"><span data-stu-id="b8bba-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directoryobject-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b8bba-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8bba-137">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete directoryObject",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
