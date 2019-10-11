---
title: Удаление educationUser из educationSchool.
description: Удаление пользователя из учебного заведения.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 8ff75f7c40e1eade2b3fbfc67b16141f69b43bae
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2019
ms.locfileid: "37427895"
---
# <a name="remove-educationuser-from-an-educationschool"></a><span data-ttu-id="a5a2b-103">Удаление educationUser из educationSchool.</span><span class="sxs-lookup"><span data-stu-id="a5a2b-103">Remove educationUser from an educationSchool</span></span>

<span data-ttu-id="a5a2b-104">Удаление пользователя из учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="a5a2b-104">Delete a user from a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5a2b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a5a2b-105">Permissions</span></span>
<span data-ttu-id="a5a2b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5a2b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5a2b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a5a2b-108">Permission type</span></span>      | <span data-ttu-id="a5a2b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a5a2b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5a2b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a5a2b-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="a5a2b-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5a2b-111">Not supported.</span></span>  |
|<span data-ttu-id="a5a2b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a5a2b-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="a5a2b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5a2b-113">Not supported.</span></span>  |
|<span data-ttu-id="a5a2b-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="a5a2b-114">Application</span></span> | <span data-ttu-id="a5a2b-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5a2b-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="a5a2b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a5a2b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}/users/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="a5a2b-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a5a2b-117">Request headers</span></span>
| <span data-ttu-id="a5a2b-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a5a2b-118">Header</span></span>       | <span data-ttu-id="a5a2b-119">Значение</span><span class="sxs-lookup"><span data-stu-id="a5a2b-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a5a2b-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a5a2b-120">Authorization</span></span>  | <span data-ttu-id="a5a2b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a5a2b-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a5a2b-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a5a2b-123">Request body</span></span>
<span data-ttu-id="a5a2b-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a5a2b-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="a5a2b-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="a5a2b-125">Response</span></span>
<span data-ttu-id="a5a2b-126">При успешном выполнении этот метод возвращает код отклика `204 No Content` и пустое тело отклика.</span><span class="sxs-lookup"><span data-stu-id="a5a2b-126">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5a2b-127">Пример</span><span class="sxs-lookup"><span data-stu-id="a5a2b-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a5a2b-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="a5a2b-128">Request</span></span>
<span data-ttu-id="a5a2b-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a5a2b-129">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a5a2b-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="a5a2b-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/schools/{school-id}/users/{user-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a5a2b-131">C#</span><span class="sxs-lookup"><span data-stu-id="a5a2b-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationclass-from-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a5a2b-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a5a2b-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationclass-from-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a5a2b-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a5a2b-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationclass-from-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a5a2b-134">Java</span><span class="sxs-lookup"><span data-stu-id="a5a2b-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationclass-from-educationschool-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a5a2b-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="a5a2b-135">Response</span></span>
<span data-ttu-id="a5a2b-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a5a2b-136">The following is an example of the response.</span></span> 
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
