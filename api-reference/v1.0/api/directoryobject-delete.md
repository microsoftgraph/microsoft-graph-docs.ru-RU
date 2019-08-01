---
title: Удаление объекта directoryObject
description: Удаляет directoryObject.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 00220213337abf8dc3f5d6d006d6730322646b64
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36016841"
---
# <a name="delete-directoryobject"></a><span data-ttu-id="41e34-103">Удаление объекта directoryObject</span><span class="sxs-lookup"><span data-stu-id="41e34-103">Delete directoryObject</span></span>

<span data-ttu-id="41e34-104">Удаляет directoryObject.</span><span class="sxs-lookup"><span data-stu-id="41e34-104">Deletes a directoryObject.</span></span>

## <a name="permissions"></a><span data-ttu-id="41e34-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="41e34-105">Permissions</span></span>
<span data-ttu-id="41e34-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41e34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="41e34-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="41e34-108">Permission type</span></span>      | <span data-ttu-id="41e34-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="41e34-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="41e34-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="41e34-110">Delegated (work or school account)</span></span> | <span data-ttu-id="41e34-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="41e34-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="41e34-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="41e34-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41e34-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41e34-113">Not supported.</span></span>    |
|<span data-ttu-id="41e34-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="41e34-114">Application</span></span> | <span data-ttu-id="41e34-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41e34-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="41e34-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="41e34-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directoryObjects/{id}

```
## <a name="request-headers"></a><span data-ttu-id="41e34-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="41e34-117">Request headers</span></span>
| <span data-ttu-id="41e34-118">Имя</span><span class="sxs-lookup"><span data-stu-id="41e34-118">Name</span></span>       | <span data-ttu-id="41e34-119">Тип</span><span class="sxs-lookup"><span data-stu-id="41e34-119">Type</span></span> | <span data-ttu-id="41e34-120">Описание</span><span class="sxs-lookup"><span data-stu-id="41e34-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="41e34-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="41e34-121">Authorization</span></span>  | <span data-ttu-id="41e34-122">string</span><span class="sxs-lookup"><span data-stu-id="41e34-122">string</span></span>  | <span data-ttu-id="41e34-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="41e34-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="41e34-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="41e34-125">Request body</span></span>
<span data-ttu-id="41e34-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="41e34-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41e34-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="41e34-127">Response</span></span>

<span data-ttu-id="41e34-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="41e34-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41e34-130">Пример</span><span class="sxs-lookup"><span data-stu-id="41e34-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="41e34-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="41e34-131">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="41e34-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="41e34-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directoryObjects/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="41e34-133">C#</span><span class="sxs-lookup"><span data-stu-id="41e34-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="41e34-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="41e34-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="41e34-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="41e34-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="41e34-136">Java</span><span class="sxs-lookup"><span data-stu-id="41e34-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directoryobject-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="41e34-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="41e34-137">Response</span></span>

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
