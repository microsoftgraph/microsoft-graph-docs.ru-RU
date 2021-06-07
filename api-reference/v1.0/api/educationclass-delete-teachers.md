---
title: 'Удаление преподавателя из educationClass '
description: Удаление преподавателя для курса.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: fa58d3f20e73b603e4a04c2da204870d0b7a10e0
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52783689"
---
# <a name="remove-teacher-from-educationclass"></a><span data-ttu-id="e0a1e-103">Удаление преподавателя из educationClass</span><span class="sxs-lookup"><span data-stu-id="e0a1e-103">Remove teacher from educationClass</span></span>
<span data-ttu-id="e0a1e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0a1e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e0a1e-105">Удаление преподавателя из [класса educationClass](../resources/educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="e0a1e-105">Remove teacher from an [educationClass](../resources/educationclass.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e0a1e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e0a1e-106">Permissions</span></span>
<span data-ttu-id="e0a1e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0a1e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0a1e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e0a1e-109">Permission type</span></span>      | <span data-ttu-id="e0a1e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e0a1e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e0a1e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e0a1e-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="e0a1e-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0a1e-112">Not supported.</span></span>  |
|<span data-ttu-id="e0a1e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e0a1e-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e0a1e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0a1e-114">Not supported.</span></span>  |
|<span data-ttu-id="e0a1e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e0a1e-115">Application</span></span> | <span data-ttu-id="e0a1e-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0a1e-116">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e0a1e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e0a1e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/teachers/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="e0a1e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e0a1e-118">Request headers</span></span>
| <span data-ttu-id="e0a1e-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e0a1e-119">Header</span></span>       | <span data-ttu-id="e0a1e-120">Значение</span><span class="sxs-lookup"><span data-stu-id="e0a1e-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e0a1e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e0a1e-121">Authorization</span></span>  | <span data-ttu-id="e0a1e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e0a1e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e0a1e-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e0a1e-124">Request body</span></span>
<span data-ttu-id="e0a1e-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e0a1e-125">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="e0a1e-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0a1e-126">Response</span></span>
<span data-ttu-id="e0a1e-127">При успешном выполнении этот метод возвращает код отклика `204 No Content` и пустое тело отклика.</span><span class="sxs-lookup"><span data-stu-id="e0a1e-127">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0a1e-128">Пример</span><span class="sxs-lookup"><span data-stu-id="e0a1e-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e0a1e-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="e0a1e-129">Request</span></span>
<span data-ttu-id="e0a1e-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e0a1e-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e0a1e-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="e0a1e-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool_2"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/classes/{class-id}/teachers/{teacher-id}
```
# <a name="c"></a>[<span data-ttu-id="e0a1e-132">C#</span><span class="sxs-lookup"><span data-stu-id="e0a1e-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationclass-from-educationschool-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e0a1e-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e0a1e-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationclass-from-educationschool-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e0a1e-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e0a1e-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationclass-from-educationschool-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e0a1e-135">Java</span><span class="sxs-lookup"><span data-stu-id="e0a1e-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationclass-from-educationschool-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e0a1e-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="e0a1e-136">Response</span></span>
<span data-ttu-id="e0a1e-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e0a1e-137">The following is an example of the response.</span></span> 
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
