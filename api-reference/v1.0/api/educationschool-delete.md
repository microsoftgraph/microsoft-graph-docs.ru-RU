---
title: Удаление educationSchool
description: Удаление учебного заведения.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 87d59c9623d8f2ca00def7ca4c974b25aef56ecc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517497"
---
# <a name="delete-educationschool"></a><span data-ttu-id="05a15-103">Удаление educationSchool</span><span class="sxs-lookup"><span data-stu-id="05a15-103">Delete educationSchool</span></span>

<span data-ttu-id="05a15-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05a15-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="05a15-105">Удаление учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="05a15-105">Delete a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="05a15-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="05a15-106">Permissions</span></span>
<span data-ttu-id="05a15-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05a15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05a15-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="05a15-109">Permission type</span></span>      | <span data-ttu-id="05a15-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="05a15-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="05a15-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="05a15-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="05a15-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05a15-112">Not supported.</span></span>  |
|<span data-ttu-id="05a15-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="05a15-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="05a15-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05a15-114">Not supported.</span></span>  |
|<span data-ttu-id="05a15-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="05a15-115">Application</span></span> | <span data-ttu-id="05a15-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05a15-116">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="05a15-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="05a15-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}
```
## <a name="request-headers"></a><span data-ttu-id="05a15-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="05a15-118">Request headers</span></span>
| <span data-ttu-id="05a15-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="05a15-119">Header</span></span>       | <span data-ttu-id="05a15-120">Значение</span><span class="sxs-lookup"><span data-stu-id="05a15-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="05a15-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="05a15-121">Authorization</span></span>  | <span data-ttu-id="05a15-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="05a15-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="05a15-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="05a15-124">Request body</span></span>
<span data-ttu-id="05a15-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="05a15-125">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="05a15-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="05a15-126">Response</span></span>
<span data-ttu-id="05a15-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="05a15-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05a15-129">Пример</span><span class="sxs-lookup"><span data-stu-id="05a15-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="05a15-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="05a15-130">Request</span></span>
<span data-ttu-id="05a15-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="05a15-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="05a15-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="05a15-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/schools/{school-id}
```
# <a name="c"></a>[<span data-ttu-id="05a15-133">C#</span><span class="sxs-lookup"><span data-stu-id="05a15-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="05a15-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="05a15-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="05a15-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="05a15-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="05a15-136">Java</span><span class="sxs-lookup"><span data-stu-id="05a15-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationschool-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="05a15-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="05a15-137">Response</span></span>
<span data-ttu-id="05a15-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="05a15-138">The following is an example of the response.</span></span> 

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
  "description": "Delete educationSchool",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
