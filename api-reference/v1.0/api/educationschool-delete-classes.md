---
title: Удаление educationClass
description: Удаление класса из учебного заведения.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 5d8ff477efc5335ddd4dadc1ac1d51fe949e57d2
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2019
ms.locfileid: "37427902"
---
# <a name="remove-educationclass"></a><span data-ttu-id="7ce09-103">Удаление educationClass</span><span class="sxs-lookup"><span data-stu-id="7ce09-103">Remove educationClass</span></span>

<span data-ttu-id="7ce09-104">Удаление класса из учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="7ce09-104">Delete a class from a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="7ce09-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7ce09-105">Permissions</span></span>
<span data-ttu-id="7ce09-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ce09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ce09-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7ce09-108">Permission type</span></span>      | <span data-ttu-id="7ce09-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7ce09-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ce09-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7ce09-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="7ce09-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ce09-111">Not supported.</span></span>  |
|<span data-ttu-id="7ce09-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7ce09-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="7ce09-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ce09-113">Not supported.</span></span>  |
|<span data-ttu-id="7ce09-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="7ce09-114">Application</span></span> | <span data-ttu-id="7ce09-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ce09-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="7ce09-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7ce09-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}/classes/{classId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="7ce09-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7ce09-117">Request headers</span></span>
| <span data-ttu-id="7ce09-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7ce09-118">Header</span></span>       | <span data-ttu-id="7ce09-119">Значение</span><span class="sxs-lookup"><span data-stu-id="7ce09-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7ce09-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7ce09-120">Authorization</span></span>  | <span data-ttu-id="7ce09-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7ce09-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7ce09-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7ce09-123">Request body</span></span>
<span data-ttu-id="7ce09-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7ce09-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="7ce09-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="7ce09-125">Response</span></span>
<span data-ttu-id="7ce09-126">При успешном выполнении этот метод возвращает код отклика `204 No Content` и тело отклика.</span><span class="sxs-lookup"><span data-stu-id="7ce09-126">If successful, this method returns a `204 No Content` response code and a response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ce09-127">Пример</span><span class="sxs-lookup"><span data-stu-id="7ce09-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7ce09-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="7ce09-128">Request</span></span>
<span data-ttu-id="7ce09-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7ce09-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7ce09-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="7ce09-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/schools/{school-id}/classes/{class-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7ce09-131">C#</span><span class="sxs-lookup"><span data-stu-id="7ce09-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationclass-from-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7ce09-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7ce09-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationclass-from-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7ce09-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7ce09-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationclass-from-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7ce09-134">Java</span><span class="sxs-lookup"><span data-stu-id="7ce09-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationclass-from-educationschool-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7ce09-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ce09-135">Response</span></span>
<span data-ttu-id="7ce09-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7ce09-136">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
