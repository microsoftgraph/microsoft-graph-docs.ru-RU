---
title: Удаление категории Outlook
description: Удаление указанного объекта outlookCategory.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: bdc0bbb2cc27a5ad8fcb4ed14bca48d72d2b155b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35448328"
---
# <a name="delete-outlook-category"></a><span data-ttu-id="c7e19-103">Удаление категории Outlook</span><span class="sxs-lookup"><span data-stu-id="c7e19-103">Delete Outlook category</span></span>


<span data-ttu-id="c7e19-104">Удаление указанного объекта [outlookCategory](../resources/outlookcategory.md).</span><span class="sxs-lookup"><span data-stu-id="c7e19-104">Delete the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c7e19-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c7e19-105">Permissions</span></span>
<span data-ttu-id="c7e19-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7e19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7e19-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c7e19-108">Permission type</span></span>      | <span data-ttu-id="c7e19-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c7e19-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7e19-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c7e19-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c7e19-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7e19-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="c7e19-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c7e19-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7e19-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7e19-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="c7e19-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c7e19-114">Application</span></span> | <span data-ttu-id="c7e19-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7e19-115">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c7e19-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7e19-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/masterCategories/{id}
DELETE /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c7e19-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c7e19-117">Request headers</span></span>
| <span data-ttu-id="c7e19-118">Имя</span><span class="sxs-lookup"><span data-stu-id="c7e19-118">Name</span></span>      |<span data-ttu-id="c7e19-119">Описание</span><span class="sxs-lookup"><span data-stu-id="c7e19-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c7e19-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c7e19-120">Authorization</span></span>  | <span data-ttu-id="c7e19-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c7e19-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c7e19-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c7e19-123">Request body</span></span>
<span data-ttu-id="c7e19-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c7e19-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7e19-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7e19-125">Response</span></span>

<span data-ttu-id="c7e19-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="c7e19-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7e19-128">Пример</span><span class="sxs-lookup"><span data-stu-id="c7e19-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c7e19-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7e19-129">Request</span></span>
<span data-ttu-id="c7e19-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c7e19-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c7e19-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="c7e19-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["4b1c2495-54c9-4a5e-90a2-0ab0b31987d8"],
  "name": "delete_outlookcategory"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/outlook/masterCategories/4b1c2495-54c9-4a5e-90a2-0ab0b31987d8
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c7e19-132">C#</span><span class="sxs-lookup"><span data-stu-id="c7e19-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-outlookcategory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c7e19-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="c7e19-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-outlookcategory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c7e19-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c7e19-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-outlookcategory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c7e19-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7e19-135">Response</span></span>
<span data-ttu-id="c7e19-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c7e19-136">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "name": "delete_outlookcategory",
  "isEmpty": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
