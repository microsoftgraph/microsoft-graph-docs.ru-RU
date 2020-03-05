---
title: Удаление фотографии
description: Удаление фотографии.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 8003e77a908b5242635c36b54a1cdfe6d257d54b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455856"
---
# <a name="delete-photo"></a><span data-ttu-id="7f93c-103">Удаление фотографии</span><span class="sxs-lookup"><span data-stu-id="7f93c-103">Delete photo</span></span>

<span data-ttu-id="7f93c-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7f93c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f93c-105">Удаление фотографии.</span><span class="sxs-lookup"><span data-stu-id="7f93c-105">Delete a photo.</span></span>
## <a name="permissions"></a><span data-ttu-id="7f93c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7f93c-106">Permissions</span></span>
<span data-ttu-id="7f93c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f93c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f93c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7f93c-109">Permission type</span></span>      | <span data-ttu-id="7f93c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7f93c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f93c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7f93c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7f93c-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7f93c-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7f93c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7f93c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f93c-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7f93c-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7f93c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7f93c-115">Application</span></span> | <span data-ttu-id="7f93c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f93c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f93c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7f93c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}/photo
DELETE /groups/{id}/photo
DELETE /drive/root/createdByUser/photo

```
## <a name="request-headers"></a><span data-ttu-id="7f93c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7f93c-118">Request headers</span></span>
| <span data-ttu-id="7f93c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="7f93c-119">Name</span></span>       | <span data-ttu-id="7f93c-120">Тип</span><span class="sxs-lookup"><span data-stu-id="7f93c-120">Type</span></span> | <span data-ttu-id="7f93c-121">Описание</span><span class="sxs-lookup"><span data-stu-id="7f93c-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7f93c-122">if-match</span><span class="sxs-lookup"><span data-stu-id="7f93c-122">if-match</span></span>  | <span data-ttu-id="7f93c-123">string</span><span class="sxs-lookup"><span data-stu-id="7f93c-123">string</span></span>  | <span data-ttu-id="7f93c-124">Если указан заголовок запроса, а предоставленный тег eTag (или cTag) не совпадает с текущим тегом элемента, то возвращается отклик `412 Precondition Failed`, а элемент не удаляется.</span><span class="sxs-lookup"><span data-stu-id="7f93c-124">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>|
| <span data-ttu-id="7f93c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f93c-125">Authorization</span></span>  | <span data-ttu-id="7f93c-126">string</span><span class="sxs-lookup"><span data-stu-id="7f93c-126">string</span></span>  | <span data-ttu-id="7f93c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7f93c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7f93c-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7f93c-129">Request body</span></span>
<span data-ttu-id="7f93c-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7f93c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f93c-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="7f93c-131">Response</span></span>

<span data-ttu-id="7f93c-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="7f93c-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f93c-134">Пример</span><span class="sxs-lookup"><span data-stu-id="7f93c-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7f93c-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="7f93c-135">Request</span></span>
<span data-ttu-id="7f93c-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7f93c-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7f93c-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="7f93c-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_photo"
}-->
```http
DELETE https://graph.microsoft.com/beta/users/{id|userPrincipalName}/photo
```
# <a name="c"></a>[<span data-ttu-id="7f93c-138">C#</span><span class="sxs-lookup"><span data-stu-id="7f93c-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-photo-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7f93c-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7f93c-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-photo-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7f93c-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7f93c-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-photo-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7f93c-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f93c-141">Response</span></span>
<span data-ttu-id="7f93c-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7f93c-142">Here is an example of the response.</span></span>
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
