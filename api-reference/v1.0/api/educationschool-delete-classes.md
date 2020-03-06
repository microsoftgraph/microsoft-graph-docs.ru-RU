---
title: Удаление educationClass
description: Удаление класса из учебного заведения.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 25fcdd6ee4c7f001ca69796b17f54dbd93150843
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517504"
---
# <a name="remove-educationclass"></a><span data-ttu-id="41de0-103">Удаление educationClass</span><span class="sxs-lookup"><span data-stu-id="41de0-103">Remove educationClass</span></span>

<span data-ttu-id="41de0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41de0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="41de0-105">Удаление класса из учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="41de0-105">Delete a class from a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="41de0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="41de0-106">Permissions</span></span>
<span data-ttu-id="41de0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41de0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41de0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="41de0-109">Permission type</span></span>      | <span data-ttu-id="41de0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="41de0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="41de0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="41de0-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="41de0-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41de0-112">Not supported.</span></span>  |
|<span data-ttu-id="41de0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="41de0-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="41de0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41de0-114">Not supported.</span></span>  |
|<span data-ttu-id="41de0-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="41de0-115">Application</span></span> | <span data-ttu-id="41de0-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41de0-116">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="41de0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="41de0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}/classes/{classId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="41de0-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="41de0-118">Request headers</span></span>
| <span data-ttu-id="41de0-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="41de0-119">Header</span></span>       | <span data-ttu-id="41de0-120">Значение</span><span class="sxs-lookup"><span data-stu-id="41de0-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="41de0-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="41de0-121">Authorization</span></span>  | <span data-ttu-id="41de0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="41de0-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="41de0-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="41de0-124">Request body</span></span>
<span data-ttu-id="41de0-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="41de0-125">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="41de0-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="41de0-126">Response</span></span>
<span data-ttu-id="41de0-127">При успешном выполнении этот метод возвращает код отклика `204 No Content` и тело отклика.</span><span class="sxs-lookup"><span data-stu-id="41de0-127">If successful, this method returns a `204 No Content` response code and a response body.</span></span>

## <a name="example"></a><span data-ttu-id="41de0-128">Пример</span><span class="sxs-lookup"><span data-stu-id="41de0-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="41de0-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="41de0-129">Request</span></span>
<span data-ttu-id="41de0-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="41de0-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="41de0-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="41de0-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/schools/{school-id}/classes/{class-id}
```
# <a name="c"></a>[<span data-ttu-id="41de0-132">C#</span><span class="sxs-lookup"><span data-stu-id="41de0-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationclass-from-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="41de0-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="41de0-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationclass-from-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="41de0-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="41de0-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationclass-from-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="41de0-135">Java</span><span class="sxs-lookup"><span data-stu-id="41de0-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationclass-from-educationschool-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="41de0-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="41de0-136">Response</span></span>
<span data-ttu-id="41de0-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="41de0-137">The following is an example of the response.</span></span> 

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
