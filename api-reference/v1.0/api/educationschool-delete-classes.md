---
title: Удаление educationClass
description: Удаление класса из учебного заведения.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 7b71f1f104a15b1772f92717cac6136f29b2a565
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956647"
---
# <a name="remove-educationclass"></a><span data-ttu-id="8a961-103">Удаление educationClass</span><span class="sxs-lookup"><span data-stu-id="8a961-103">Remove educationClass</span></span>

<span data-ttu-id="8a961-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a961-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8a961-105">Удаление класса из учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="8a961-105">Delete a class from a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="8a961-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8a961-106">Permissions</span></span>
<span data-ttu-id="8a961-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a961-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a961-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8a961-109">Permission type</span></span>      | <span data-ttu-id="8a961-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8a961-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a961-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8a961-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="8a961-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a961-112">Not supported.</span></span>  |
|<span data-ttu-id="8a961-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8a961-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="8a961-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8a961-114">Not supported.</span></span>  |
|<span data-ttu-id="8a961-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8a961-115">Application</span></span> | <span data-ttu-id="8a961-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a961-116">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="8a961-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8a961-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/schools/{id}/classes/{classId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="8a961-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8a961-118">Request headers</span></span>
| <span data-ttu-id="8a961-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8a961-119">Header</span></span>       | <span data-ttu-id="8a961-120">Значение</span><span class="sxs-lookup"><span data-stu-id="8a961-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8a961-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8a961-121">Authorization</span></span>  | <span data-ttu-id="8a961-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8a961-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8a961-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8a961-124">Request body</span></span>
<span data-ttu-id="8a961-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8a961-125">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="8a961-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a961-126">Response</span></span>
<span data-ttu-id="8a961-127">При успешном выполнении этот метод возвращает код отклика `204 No Content` и тело отклика.</span><span class="sxs-lookup"><span data-stu-id="8a961-127">If successful, this method returns a `204 No Content` response code and a response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a961-128">Пример</span><span class="sxs-lookup"><span data-stu-id="8a961-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8a961-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="8a961-129">Request</span></span>
<span data-ttu-id="8a961-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8a961-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8a961-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="8a961-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool_3"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/schools/{school-id}/classes/{class-id}
```
# <a name="c"></a>[<span data-ttu-id="8a961-132">C#</span><span class="sxs-lookup"><span data-stu-id="8a961-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationclass-from-educationschool-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8a961-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8a961-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationclass-from-educationschool-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8a961-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8a961-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationclass-from-educationschool-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8a961-135">Java</span><span class="sxs-lookup"><span data-stu-id="8a961-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationclass-from-educationschool-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="8a961-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="8a961-136">Response</span></span>
<span data-ttu-id="8a961-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8a961-137">The following is an example of the response.</span></span> 

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

