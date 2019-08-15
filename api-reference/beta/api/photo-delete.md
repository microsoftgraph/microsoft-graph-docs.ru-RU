---
title: Удаление фотографии
description: Удаление фотографии.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: d16b858822681d7ff77fc4cb0ab7db5f7b395642
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36413652"
---
# <a name="delete-photo"></a><span data-ttu-id="d7d43-103">Удаление фотографии</span><span class="sxs-lookup"><span data-stu-id="d7d43-103">Delete photo</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7d43-104">Удаление фотографии.</span><span class="sxs-lookup"><span data-stu-id="d7d43-104">Delete a photo.</span></span>
## <a name="permissions"></a><span data-ttu-id="d7d43-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d7d43-105">Permissions</span></span>
<span data-ttu-id="d7d43-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7d43-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7d43-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d7d43-108">Permission type</span></span>      | <span data-ttu-id="d7d43-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d7d43-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7d43-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d7d43-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d7d43-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d7d43-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d7d43-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d7d43-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7d43-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d7d43-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d7d43-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d7d43-114">Application</span></span> | <span data-ttu-id="d7d43-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7d43-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7d43-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d7d43-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}/photo
DELETE /groups/{id}/photo
DELETE /drive/root/createdByUser/photo

```
## <a name="request-headers"></a><span data-ttu-id="d7d43-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d7d43-117">Request headers</span></span>
| <span data-ttu-id="d7d43-118">Имя</span><span class="sxs-lookup"><span data-stu-id="d7d43-118">Name</span></span>       | <span data-ttu-id="d7d43-119">Тип</span><span class="sxs-lookup"><span data-stu-id="d7d43-119">Type</span></span> | <span data-ttu-id="d7d43-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d7d43-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d7d43-121">if-match</span><span class="sxs-lookup"><span data-stu-id="d7d43-121">if-match</span></span>  | <span data-ttu-id="d7d43-122">string</span><span class="sxs-lookup"><span data-stu-id="d7d43-122">string</span></span>  | <span data-ttu-id="d7d43-123">Если указан заголовок запроса, а предоставленный тег eTag (или cTag) не совпадает с текущим тегом элемента, то возвращается отклик `412 Precondition Failed`, а элемент не удаляется.</span><span class="sxs-lookup"><span data-stu-id="d7d43-123">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>|
| <span data-ttu-id="d7d43-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7d43-124">Authorization</span></span>  | <span data-ttu-id="d7d43-125">string</span><span class="sxs-lookup"><span data-stu-id="d7d43-125">string</span></span>  | <span data-ttu-id="d7d43-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d7d43-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d7d43-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d7d43-128">Request body</span></span>
<span data-ttu-id="d7d43-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d7d43-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d7d43-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7d43-130">Response</span></span>

<span data-ttu-id="d7d43-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="d7d43-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7d43-133">Пример</span><span class="sxs-lookup"><span data-stu-id="d7d43-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d7d43-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="d7d43-134">Request</span></span>
<span data-ttu-id="d7d43-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d7d43-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d7d43-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="d7d43-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_photo"
}-->
```http
DELETE https://graph.microsoft.com/beta/users/{id|userPrincipalName}/photo
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d7d43-137">C#</span><span class="sxs-lookup"><span data-stu-id="d7d43-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-photo-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d7d43-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d7d43-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-photo-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d7d43-139">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d7d43-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-photo-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d7d43-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7d43-140">Response</span></span>
<span data-ttu-id="d7d43-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d7d43-141">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
