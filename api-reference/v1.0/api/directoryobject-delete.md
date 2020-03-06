---
title: Удаление объекта directoryObject
description: Удаляет directoryObject.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 46e5faec04b28cd6d48f8f4344d6c5237e4a29e5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518009"
---
# <a name="delete-directoryobject"></a><span data-ttu-id="ab4a4-103">Удаление объекта directoryObject</span><span class="sxs-lookup"><span data-stu-id="ab4a4-103">Delete directoryObject</span></span>

<span data-ttu-id="ab4a4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab4a4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ab4a4-105">Удаляет directoryObject.</span><span class="sxs-lookup"><span data-stu-id="ab4a4-105">Deletes a directoryObject.</span></span>

## <a name="permissions"></a><span data-ttu-id="ab4a4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ab4a4-106">Permissions</span></span>
<span data-ttu-id="ab4a4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab4a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ab4a4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ab4a4-109">Permission type</span></span>      | <span data-ttu-id="ab4a4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ab4a4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab4a4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ab4a4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ab4a4-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ab4a4-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ab4a4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ab4a4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab4a4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab4a4-114">Not supported.</span></span>    |
|<span data-ttu-id="ab4a4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ab4a4-115">Application</span></span> | <span data-ttu-id="ab4a4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab4a4-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab4a4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ab4a4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directoryObjects/{id}

```
## <a name="request-headers"></a><span data-ttu-id="ab4a4-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ab4a4-118">Request headers</span></span>
| <span data-ttu-id="ab4a4-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ab4a4-119">Name</span></span>       | <span data-ttu-id="ab4a4-120">Тип</span><span class="sxs-lookup"><span data-stu-id="ab4a4-120">Type</span></span> | <span data-ttu-id="ab4a4-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ab4a4-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ab4a4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab4a4-122">Authorization</span></span>  | <span data-ttu-id="ab4a4-123">string</span><span class="sxs-lookup"><span data-stu-id="ab4a4-123">string</span></span>  | <span data-ttu-id="ab4a4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ab4a4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ab4a4-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ab4a4-126">Request body</span></span>
<span data-ttu-id="ab4a4-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ab4a4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab4a4-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="ab4a4-128">Response</span></span>

<span data-ttu-id="ab4a4-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="ab4a4-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab4a4-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ab4a4-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ab4a4-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ab4a4-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ab4a4-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ab4a4-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directoryObjects/{id}
```
# <a name="c"></a>[<span data-ttu-id="ab4a4-134">C#</span><span class="sxs-lookup"><span data-stu-id="ab4a4-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ab4a4-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ab4a4-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ab4a4-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ab4a4-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ab4a4-137">Java</span><span class="sxs-lookup"><span data-stu-id="ab4a4-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directoryobject-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ab4a4-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab4a4-138">Response</span></span>

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
