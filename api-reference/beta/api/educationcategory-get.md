---
title: Get educationCategory
description: Извлечение объекта категории.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 43e26c09b1f5c29e7c096ee0a905e5141d79191f
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2021
ms.locfileid: "52991691"
---
# <a name="get-educationcategory"></a><span data-ttu-id="91615-103">Get educationCategory</span><span class="sxs-lookup"><span data-stu-id="91615-103">Get educationCategory</span></span>

<span data-ttu-id="91615-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91615-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91615-105">Извлечение [объекта educationCategory.](../resources/educationcategory.md)</span><span class="sxs-lookup"><span data-stu-id="91615-105">Retrieve an [educationCategory](../resources/educationcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="91615-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="91615-106">Permissions</span></span>

<span data-ttu-id="91615-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91615-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="91615-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="91615-109">Permission type</span></span>                        | <span data-ttu-id="91615-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="91615-110">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="91615-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="91615-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="91615-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="91615-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="91615-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="91615-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91615-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91615-114">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="91615-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="91615-115">Application</span></span>                            | <span data-ttu-id="91615-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="91615-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="91615-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="91615-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignmentCategories/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="91615-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="91615-118">Optional query parameters</span></span>

<span data-ttu-id="91615-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="91615-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="91615-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="91615-120">Request headers</span></span>
| <span data-ttu-id="91615-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="91615-121">Header</span></span>        | <span data-ttu-id="91615-122">Значение</span><span class="sxs-lookup"><span data-stu-id="91615-122">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="91615-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="91615-123">Authorization</span></span> | <span data-ttu-id="91615-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="91615-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="91615-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="91615-126">Request body</span></span>

<span data-ttu-id="91615-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="91615-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="91615-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="91615-128">Response</span></span>

<span data-ttu-id="91615-129">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект educationCategory](../resources/educationcategory.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="91615-129">If successful, this method returns a `200 OK` response code and a [educationCategory](../resources/educationcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91615-130">Пример</span><span class="sxs-lookup"><span data-stu-id="91615-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="91615-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="91615-131">Request</span></span>

<span data-ttu-id="91615-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="91615-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="91615-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="91615-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["dacbf757-888d-42ae-b701-5e57cec300ae"],
  "name": "get_class_category"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/dacbf757-888d-42ae-b701-5e57cec300ae/assignmentCategories/7f64924d-4cdb-4e54-8c37-c0f3d46f0747
```
# <a name="c"></a>[<span data-ttu-id="91615-134">C#</span><span class="sxs-lookup"><span data-stu-id="91615-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-class-category-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="91615-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="91615-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-class-category-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="91615-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="91615-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-class-category-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="91615-137">Java</span><span class="sxs-lookup"><span data-stu-id="91615-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-class-category-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="91615-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="91615-138">Response</span></span>

<span data-ttu-id="91615-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="91615-139">The following is an example of the response.</span></span>

><span data-ttu-id="91615-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="91615-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory",
  "isCollection": false
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 85

{
    "@odata.context": "https://graph.microsoft.com/v1.0/education/classes/dacbf757-888d-42ae-b701-5e57cec300ae/assignmentCategories/$entity",
    "displayName": "Quizzes",
    "id": "7f64924d-4cdb-4e54-8c37-c0f3d46f0747"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get category",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
