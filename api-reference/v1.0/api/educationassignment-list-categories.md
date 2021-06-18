---
title: Перечисление категорий
description: Список всех категорий, связанных с этим назначением.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 820068cafa4667e4a1d4ea47b6e25b725e8b63fe
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2021
ms.locfileid: "52991083"
---
# <a name="list-categories"></a><span data-ttu-id="b247a-103">Перечисление категорий</span><span class="sxs-lookup"><span data-stu-id="b247a-103">List categories</span></span>

<span data-ttu-id="b247a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b247a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b247a-105">Список всех категорий, связанных с назначением.</span><span class="sxs-lookup"><span data-stu-id="b247a-105">List all the categories associated with an assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="b247a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b247a-106">Permissions</span></span>
<span data-ttu-id="b247a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b247a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b247a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b247a-109">Permission type</span></span>      | <span data-ttu-id="b247a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b247a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b247a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b247a-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="b247a-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b247a-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="b247a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b247a-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="b247a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b247a-114">Not supported.</span></span>  |
|<span data-ttu-id="b247a-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="b247a-115">Application</span></span> | <span data-ttu-id="b247a-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b247a-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b247a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b247a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/categories
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b247a-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b247a-118">Optional query parameters</span></span>
<span data-ttu-id="b247a-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="b247a-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b247a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b247a-120">Request headers</span></span>
| <span data-ttu-id="b247a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b247a-121">Header</span></span>       | <span data-ttu-id="b247a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b247a-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b247a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b247a-123">Authorization</span></span>  | <span data-ttu-id="b247a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b247a-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b247a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b247a-126">Request body</span></span>
<span data-ttu-id="b247a-127">Не поставляем тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b247a-127">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b247a-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="b247a-128">Response</span></span>
<span data-ttu-id="b247a-129">В случае успешной работы этот метод возвращает код ответа и коллекцию `200 OK` [объектов educationCategory](../resources/educationcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b247a-129">If successful, this method returns a `200 OK` response code and collection of [educationCategory](../resources/educationcategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b247a-130">Пример</span><span class="sxs-lookup"><span data-stu-id="b247a-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="b247a-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="b247a-131">Request</span></span>
<span data-ttu-id="b247a-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b247a-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b247a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="b247a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["1fdf61ee-c129-4960-9b7c-8df159aa64b0"],
  "name": "get_assignment_categories"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/a17025d0-62a8-4450-9e6e-db31d8c8feb8/assignments/1fdf61ee-c129-4960-9b7c-8df159aa64b0/categories
```
# <a name="c"></a>[<span data-ttu-id="b247a-134">C#</span><span class="sxs-lookup"><span data-stu-id="b247a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-assignment-categories-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b247a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b247a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-assignment-categories-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b247a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b247a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-assignment-categories-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b247a-137">Java</span><span class="sxs-lookup"><span data-stu-id="b247a-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-assignment-categories-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b247a-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="b247a-138">Response</span></span>
<span data-ttu-id="b247a-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b247a-139">The following is an example of the response.</span></span> 

><span data-ttu-id="b247a-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b247a-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 873

{
    "@odata.context": "https://graph.microsoft.com/v1.0/education/classes('a17025d0-62a8-4450-9e6e-db31d8c8feb8')/assignments('1fdf61ee-c129-4960-9b7c-8df159aa64b0')/categories",
    "value": [
        {
            "displayName": "Quizzes",
            "id": "9b8f8f88-ddfc-4aad-9fe9-280513fffc74"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List categories added to an assignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
