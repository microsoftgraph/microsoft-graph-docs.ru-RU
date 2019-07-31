---
title: Удаление educationSchool
description: Удаление учебного заведения.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 337bc03df9aec93bdcbfebc84db3467bf8748342
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35955203"
---
# <a name="delete-educationschool"></a><span data-ttu-id="68289-103">Удаление educationSchool</span><span class="sxs-lookup"><span data-stu-id="68289-103">Delete educationSchool</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68289-104">Удаление учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="68289-104">Delete a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="68289-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="68289-105">Permissions</span></span>
<span data-ttu-id="68289-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68289-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68289-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="68289-108">Permission type</span></span>      | <span data-ttu-id="68289-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="68289-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="68289-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="68289-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="68289-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68289-111">Not supported.</span></span>  |
|<span data-ttu-id="68289-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="68289-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="68289-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68289-113">Not supported.</span></span>  |
|<span data-ttu-id="68289-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="68289-114">Application</span></span> | <span data-ttu-id="68289-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68289-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="68289-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="68289-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}
```
## <a name="request-headers"></a><span data-ttu-id="68289-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="68289-117">Request headers</span></span>
| <span data-ttu-id="68289-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="68289-118">Header</span></span>       | <span data-ttu-id="68289-119">Значение</span><span class="sxs-lookup"><span data-stu-id="68289-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="68289-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="68289-120">Authorization</span></span>  | <span data-ttu-id="68289-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="68289-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="68289-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="68289-123">Request body</span></span>
<span data-ttu-id="68289-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="68289-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="68289-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="68289-125">Response</span></span>
<span data-ttu-id="68289-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="68289-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68289-128">Пример</span><span class="sxs-lookup"><span data-stu-id="68289-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="68289-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="68289-129">Request</span></span>
<span data-ttu-id="68289-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="68289-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="68289-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="68289-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/schools/10002
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="68289-132">C#</span><span class="sxs-lookup"><span data-stu-id="68289-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="68289-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="68289-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="68289-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="68289-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="68289-135">Java</span><span class="sxs-lookup"><span data-stu-id="68289-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationschool-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="68289-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="68289-136">Response</span></span>
<span data-ttu-id="68289-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="68289-137">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete educationSchool",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
