---
title: Удаление категории Outlook
description: Удаление указанного объекта outlookCategory.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 4245584ce229c6d2d3fa9bb258ef6a7324259c78
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36309469"
---
# <a name="delete-outlook-category"></a><span data-ttu-id="00e3c-103">Удаление категории Outlook</span><span class="sxs-lookup"><span data-stu-id="00e3c-103">Delete Outlook category</span></span>


<span data-ttu-id="00e3c-104">Удаление указанного объекта [outlookCategory](../resources/outlookcategory.md).</span><span class="sxs-lookup"><span data-stu-id="00e3c-104">Delete the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="00e3c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="00e3c-105">Permissions</span></span>
<span data-ttu-id="00e3c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00e3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00e3c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="00e3c-108">Permission type</span></span>      | <span data-ttu-id="00e3c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="00e3c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="00e3c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="00e3c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="00e3c-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00e3c-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="00e3c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="00e3c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00e3c-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00e3c-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="00e3c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="00e3c-114">Application</span></span> | <span data-ttu-id="00e3c-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00e3c-115">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="00e3c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="00e3c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/masterCategories/{id}
DELETE /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="00e3c-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="00e3c-117">Request headers</span></span>
| <span data-ttu-id="00e3c-118">Имя</span><span class="sxs-lookup"><span data-stu-id="00e3c-118">Name</span></span>      |<span data-ttu-id="00e3c-119">Описание</span><span class="sxs-lookup"><span data-stu-id="00e3c-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="00e3c-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="00e3c-120">Authorization</span></span>  | <span data-ttu-id="00e3c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="00e3c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="00e3c-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="00e3c-123">Request body</span></span>
<span data-ttu-id="00e3c-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="00e3c-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="00e3c-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="00e3c-125">Response</span></span>

<span data-ttu-id="00e3c-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="00e3c-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00e3c-128">Пример</span><span class="sxs-lookup"><span data-stu-id="00e3c-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="00e3c-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="00e3c-129">Request</span></span>
<span data-ttu-id="00e3c-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="00e3c-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="00e3c-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="00e3c-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["4b1c2495-54c9-4a5e-90a2-0ab0b31987d8"],
  "name": "delete_outlookcategory"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/outlook/masterCategories/4b1c2495-54c9-4a5e-90a2-0ab0b31987d8
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="00e3c-132">C#</span><span class="sxs-lookup"><span data-stu-id="00e3c-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-outlookcategory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="00e3c-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="00e3c-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-outlookcategory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="00e3c-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="00e3c-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-outlookcategory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="00e3c-135">Java</span><span class="sxs-lookup"><span data-stu-id="00e3c-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-outlookcategory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="00e3c-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="00e3c-136">Response</span></span>
<span data-ttu-id="00e3c-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="00e3c-137">Here is an example of the response.</span></span>
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
