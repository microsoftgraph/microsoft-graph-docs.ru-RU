---
title: Удаление объекта directoryObject
description: Удаляет directoryObject.
author: keylimesoda
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 02311d5908237325e627e61706d25ee1b3d16c2f
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181946"
---
# <a name="delete-directoryobject"></a><span data-ttu-id="ebc41-103">Удаление объекта directoryObject</span><span class="sxs-lookup"><span data-stu-id="ebc41-103">Delete directoryObject</span></span>

<span data-ttu-id="ebc41-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ebc41-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ebc41-105">Удаляет directoryObject.</span><span class="sxs-lookup"><span data-stu-id="ebc41-105">Deletes a directoryObject.</span></span>

## <a name="permissions"></a><span data-ttu-id="ebc41-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ebc41-106">Permissions</span></span>
<span data-ttu-id="ebc41-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ebc41-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ebc41-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ebc41-109">Permission type</span></span>      | <span data-ttu-id="ebc41-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ebc41-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ebc41-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ebc41-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ebc41-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ebc41-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ebc41-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ebc41-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ebc41-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ebc41-114">Not supported.</span></span>    |
|<span data-ttu-id="ebc41-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ebc41-115">Application</span></span> | <span data-ttu-id="ebc41-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ebc41-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ebc41-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ebc41-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directoryObjects/{id}

```
## <a name="request-headers"></a><span data-ttu-id="ebc41-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ebc41-118">Request headers</span></span>
| <span data-ttu-id="ebc41-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ebc41-119">Name</span></span>       | <span data-ttu-id="ebc41-120">Тип</span><span class="sxs-lookup"><span data-stu-id="ebc41-120">Type</span></span> | <span data-ttu-id="ebc41-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ebc41-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ebc41-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ebc41-122">Authorization</span></span>  | <span data-ttu-id="ebc41-123">string</span><span class="sxs-lookup"><span data-stu-id="ebc41-123">string</span></span>  | <span data-ttu-id="ebc41-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ebc41-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ebc41-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ebc41-126">Request body</span></span>
<span data-ttu-id="ebc41-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ebc41-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ebc41-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="ebc41-128">Response</span></span>

<span data-ttu-id="ebc41-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="ebc41-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ebc41-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ebc41-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ebc41-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ebc41-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ebc41-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ebc41-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/directoryObjects/{id}
```
# <a name="c"></a>[<span data-ttu-id="ebc41-134">C#</span><span class="sxs-lookup"><span data-stu-id="ebc41-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ebc41-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ebc41-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ebc41-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ebc41-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ebc41-137">Java</span><span class="sxs-lookup"><span data-stu-id="ebc41-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directoryobject-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ebc41-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="ebc41-138">Response</span></span>

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
