---
title: Удаление страницы
description: Удаление страницы OneNote.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 80a190c1e8725479d9e209981f02a4465f710649
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35976280"
---
# <a name="delete-page"></a><span data-ttu-id="4c3e9-103">Удаление страницы</span><span class="sxs-lookup"><span data-stu-id="4c3e9-103">Delete page</span></span>

<span data-ttu-id="4c3e9-104">Удаление страницы OneNote.</span><span class="sxs-lookup"><span data-stu-id="4c3e9-104">Delete a OneNote page.</span></span>
## <a name="permissions"></a><span data-ttu-id="4c3e9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4c3e9-105">Permissions</span></span>
<span data-ttu-id="4c3e9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c3e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c3e9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c3e9-108">Permission type</span></span>      | <span data-ttu-id="4c3e9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c3e9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c3e9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c3e9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4c3e9-111">Notes. ReadWrite, Notes. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="4c3e9-111">Notes.ReadWrite, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="4c3e9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c3e9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c3e9-113">Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4c3e9-113">Notes.ReadWrite</span></span>    |
|<span data-ttu-id="4c3e9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4c3e9-114">Application</span></span> | <span data-ttu-id="4c3e9-115">Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c3e9-115">Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c3e9-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c3e9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/onenote/pages/{id}
DELETE /users/{id | userPrincipalName}/onenote/pages/{id}
DELETE /groups/{id}/onenote/pages/{id}
DELETE /sites/{id}/onenote/pages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="4c3e9-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4c3e9-117">Request headers</span></span>
| <span data-ttu-id="4c3e9-118">Имя</span><span class="sxs-lookup"><span data-stu-id="4c3e9-118">Name</span></span>       | <span data-ttu-id="4c3e9-119">Тип</span><span class="sxs-lookup"><span data-stu-id="4c3e9-119">Type</span></span> | <span data-ttu-id="4c3e9-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4c3e9-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4c3e9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c3e9-121">Authorization</span></span>  | <span data-ttu-id="4c3e9-122">string</span><span class="sxs-lookup"><span data-stu-id="4c3e9-122">string</span></span>  | <span data-ttu-id="4c3e9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c3e9-p102">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="4c3e9-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c3e9-125">Response</span></span>

<span data-ttu-id="4c3e9-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4c3e9-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c3e9-128">Пример</span><span class="sxs-lookup"><span data-stu-id="4c3e9-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4c3e9-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c3e9-129">Request</span></span>
<span data-ttu-id="4c3e9-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c3e9-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4c3e9-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="4c3e9-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_page"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/onenote/pages/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4c3e9-132">C#</span><span class="sxs-lookup"><span data-stu-id="4c3e9-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-page-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4c3e9-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="4c3e9-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-page-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4c3e9-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="4c3e9-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-page-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4c3e9-135">Java</span><span class="sxs-lookup"><span data-stu-id="4c3e9-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-page-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4c3e9-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c3e9-136">Response</span></span>
<span data-ttu-id="4c3e9-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4c3e9-137">Here is an example of the response.</span></span>
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
  "description": "Delete page",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
