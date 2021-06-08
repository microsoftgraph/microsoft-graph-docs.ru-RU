---
title: Удаление educationUser из educationSchool.
description: Удаление пользователя из учебного заведения.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 3dfdb0e2f0bcefefc4b4d0f6c35926cf36b08d43
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787466"
---
# <a name="remove-educationuser-from-an-educationschool"></a><span data-ttu-id="12cf6-103">Удаление educationUser из educationSchool.</span><span class="sxs-lookup"><span data-stu-id="12cf6-103">Remove educationUser from an educationSchool</span></span>

<span data-ttu-id="12cf6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12cf6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="12cf6-105">Удаление пользователя из учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="12cf6-105">Delete a user from a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="12cf6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="12cf6-106">Permissions</span></span>
<span data-ttu-id="12cf6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12cf6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12cf6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="12cf6-109">Permission type</span></span>      | <span data-ttu-id="12cf6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="12cf6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="12cf6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="12cf6-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="12cf6-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12cf6-112">Not supported.</span></span>  |
|<span data-ttu-id="12cf6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="12cf6-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="12cf6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12cf6-114">Not supported.</span></span>  |
|<span data-ttu-id="12cf6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="12cf6-115">Application</span></span> | <span data-ttu-id="12cf6-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12cf6-116">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="12cf6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="12cf6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}/users/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="12cf6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="12cf6-118">Request headers</span></span>
| <span data-ttu-id="12cf6-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="12cf6-119">Header</span></span>       | <span data-ttu-id="12cf6-120">Значение</span><span class="sxs-lookup"><span data-stu-id="12cf6-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="12cf6-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="12cf6-121">Authorization</span></span>  | <span data-ttu-id="12cf6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="12cf6-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="12cf6-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="12cf6-124">Request body</span></span>
<span data-ttu-id="12cf6-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="12cf6-125">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="12cf6-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="12cf6-126">Response</span></span>
<span data-ttu-id="12cf6-127">При успешном выполнении этот метод возвращает код отклика `204 No Content` и пустое тело отклика.</span><span class="sxs-lookup"><span data-stu-id="12cf6-127">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="12cf6-128">Пример</span><span class="sxs-lookup"><span data-stu-id="12cf6-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="12cf6-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="12cf6-129">Request</span></span>
<span data-ttu-id="12cf6-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="12cf6-130">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="12cf6-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="12cf6-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool_4"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/schools/{school-id}/users/{user-id}
```
# <a name="c"></a>[<span data-ttu-id="12cf6-132">C#</span><span class="sxs-lookup"><span data-stu-id="12cf6-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationclass-from-educationschool-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="12cf6-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="12cf6-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationclass-from-educationschool-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="12cf6-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="12cf6-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationclass-from-educationschool-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="12cf6-135">Java</span><span class="sxs-lookup"><span data-stu-id="12cf6-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationclass-from-educationschool-4-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="12cf6-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="12cf6-136">Response</span></span>
<span data-ttu-id="12cf6-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="12cf6-137">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
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

