---
title: Удаление фотографии
description: Удаление фотографии.
localization_priority: Normal
author: kevinbellinger
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 57cc725d5b668d4db72ec9b96c3be0cbdf20db46
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808748"
---
# <a name="delete-photo"></a><span data-ttu-id="9eb49-103">Удаление фотографии</span><span class="sxs-lookup"><span data-stu-id="9eb49-103">Delete photo</span></span>

<span data-ttu-id="9eb49-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9eb49-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9eb49-105">Удаление фотографии.</span><span class="sxs-lookup"><span data-stu-id="9eb49-105">Delete a photo.</span></span>
## <a name="permissions"></a><span data-ttu-id="9eb49-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9eb49-106">Permissions</span></span>
<span data-ttu-id="9eb49-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9eb49-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9eb49-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9eb49-109">Permission type</span></span>      | <span data-ttu-id="9eb49-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9eb49-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9eb49-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9eb49-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9eb49-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9eb49-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9eb49-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9eb49-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9eb49-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9eb49-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9eb49-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9eb49-115">Application</span></span> | <span data-ttu-id="9eb49-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9eb49-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9eb49-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9eb49-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}/photo
DELETE /groups/{id}/photo
DELETE /drive/root/createdByUser/photo

```
## <a name="request-headers"></a><span data-ttu-id="9eb49-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9eb49-118">Request headers</span></span>
| <span data-ttu-id="9eb49-119">Имя</span><span class="sxs-lookup"><span data-stu-id="9eb49-119">Name</span></span>       | <span data-ttu-id="9eb49-120">Тип</span><span class="sxs-lookup"><span data-stu-id="9eb49-120">Type</span></span> | <span data-ttu-id="9eb49-121">Описание</span><span class="sxs-lookup"><span data-stu-id="9eb49-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9eb49-122">if-match</span><span class="sxs-lookup"><span data-stu-id="9eb49-122">if-match</span></span>  | <span data-ttu-id="9eb49-123">string</span><span class="sxs-lookup"><span data-stu-id="9eb49-123">string</span></span>  | <span data-ttu-id="9eb49-124">Если указан заголовок запроса, а предоставленный тег eTag (или cTag) не совпадает с текущим тегом элемента, то возвращается отклик `412 Precondition Failed`, а элемент не удаляется.</span><span class="sxs-lookup"><span data-stu-id="9eb49-124">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>|
| <span data-ttu-id="9eb49-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="9eb49-125">Authorization</span></span>  | <span data-ttu-id="9eb49-126">string</span><span class="sxs-lookup"><span data-stu-id="9eb49-126">string</span></span>  | <span data-ttu-id="9eb49-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9eb49-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9eb49-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9eb49-129">Request body</span></span>
<span data-ttu-id="9eb49-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9eb49-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9eb49-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="9eb49-131">Response</span></span>

<span data-ttu-id="9eb49-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="9eb49-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9eb49-134">Пример</span><span class="sxs-lookup"><span data-stu-id="9eb49-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9eb49-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="9eb49-135">Request</span></span>
<span data-ttu-id="9eb49-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9eb49-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9eb49-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="9eb49-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
"name": "delete_photo"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
```
# <a name="c"></a>[<span data-ttu-id="9eb49-138">C#</span><span class="sxs-lookup"><span data-stu-id="9eb49-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-photo-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9eb49-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9eb49-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-photo-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9eb49-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9eb49-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-photo-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9eb49-141">Java</span><span class="sxs-lookup"><span data-stu-id="9eb49-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-photo-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9eb49-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="9eb49-142">Response</span></span>
<span data-ttu-id="9eb49-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9eb49-143">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
