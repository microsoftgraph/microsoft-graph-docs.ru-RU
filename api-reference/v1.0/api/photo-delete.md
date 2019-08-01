---
title: Удаление фотографии
description: Удаление фотографии.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: f4e5a1650e2c75ec16c7625597fccd6111d94b83
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35976259"
---
# <a name="delete-photo"></a><span data-ttu-id="0fb5a-103">Удаление фотографии</span><span class="sxs-lookup"><span data-stu-id="0fb5a-103">Delete photo</span></span>

<span data-ttu-id="0fb5a-104">Удаление фотографии.</span><span class="sxs-lookup"><span data-stu-id="0fb5a-104">Delete a photo.</span></span>
## <a name="permissions"></a><span data-ttu-id="0fb5a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0fb5a-105">Permissions</span></span>
<span data-ttu-id="0fb5a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0fb5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0fb5a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0fb5a-108">Permission type</span></span>      | <span data-ttu-id="0fb5a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0fb5a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0fb5a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0fb5a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0fb5a-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0fb5a-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0fb5a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0fb5a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0fb5a-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0fb5a-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0fb5a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0fb5a-114">Application</span></span> | <span data-ttu-id="0fb5a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0fb5a-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0fb5a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0fb5a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}/photo
DELETE /groups/{id}/photo
DELETE /drive/root/createdByUser/photo

```
## <a name="request-headers"></a><span data-ttu-id="0fb5a-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0fb5a-117">Request headers</span></span>
| <span data-ttu-id="0fb5a-118">Имя</span><span class="sxs-lookup"><span data-stu-id="0fb5a-118">Name</span></span>       | <span data-ttu-id="0fb5a-119">Тип</span><span class="sxs-lookup"><span data-stu-id="0fb5a-119">Type</span></span> | <span data-ttu-id="0fb5a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0fb5a-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0fb5a-121">if-match</span><span class="sxs-lookup"><span data-stu-id="0fb5a-121">if-match</span></span>  | <span data-ttu-id="0fb5a-122">string</span><span class="sxs-lookup"><span data-stu-id="0fb5a-122">string</span></span>  | <span data-ttu-id="0fb5a-123">Если указан заголовок запроса, а предоставленный тег eTag (или cTag) не совпадает с текущим тегом элемента, то возвращается отклик `412 Precondition Failed`, а элемент не удаляется.</span><span class="sxs-lookup"><span data-stu-id="0fb5a-123">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>|
| <span data-ttu-id="0fb5a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0fb5a-124">Authorization</span></span>  | <span data-ttu-id="0fb5a-125">string</span><span class="sxs-lookup"><span data-stu-id="0fb5a-125">string</span></span>  | <span data-ttu-id="0fb5a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0fb5a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0fb5a-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0fb5a-128">Request body</span></span>
<span data-ttu-id="0fb5a-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0fb5a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0fb5a-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="0fb5a-130">Response</span></span>

<span data-ttu-id="0fb5a-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="0fb5a-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0fb5a-133">Пример</span><span class="sxs-lookup"><span data-stu-id="0fb5a-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0fb5a-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="0fb5a-134">Request</span></span>
<span data-ttu-id="0fb5a-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0fb5a-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0fb5a-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="0fb5a-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
"name": "delete_photo"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0fb5a-137">C#</span><span class="sxs-lookup"><span data-stu-id="0fb5a-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-photo-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0fb5a-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="0fb5a-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-photo-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0fb5a-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="0fb5a-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-photo-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0fb5a-140">Java</span><span class="sxs-lookup"><span data-stu-id="0fb5a-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-photo-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0fb5a-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="0fb5a-141">Response</span></span>
<span data-ttu-id="0fb5a-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0fb5a-142">Here is an example of the response.</span></span>
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
