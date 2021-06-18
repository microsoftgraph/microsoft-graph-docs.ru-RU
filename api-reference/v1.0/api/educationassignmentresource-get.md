---
title: Get educationAssignmentResource
description: 'Получите свойства определенного ресурса при назначении.  '
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: c8c28c86ad77a5274d79cd00da5c04806a31ec34
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992209"
---
# <a name="get-educationassignmentresource"></a><span data-ttu-id="fcfc8-103">Get educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="fcfc8-103">Get educationAssignmentResource</span></span>

<span data-ttu-id="fcfc8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fcfc8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fcfc8-105">Получите свойства определенного ресурса при назначении.</span><span class="sxs-lookup"><span data-stu-id="fcfc8-105">Get the properties of a specific resource on an assignment.</span></span>  
## <a name="permissions"></a><span data-ttu-id="fcfc8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fcfc8-106">Permissions</span></span>
<span data-ttu-id="fcfc8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fcfc8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fcfc8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fcfc8-109">Permission type</span></span>      | <span data-ttu-id="fcfc8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fcfc8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fcfc8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fcfc8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fcfc8-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fcfc8-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="fcfc8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fcfc8-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="fcfc8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fcfc8-114">Not supported.</span></span>  |
|<span data-ttu-id="fcfc8-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="fcfc8-115">Application</span></span> |  <span data-ttu-id="fcfc8-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fcfc8-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="fcfc8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fcfc8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/resources/8b01c1d0-aafc-4f8c-bd73-89faa3df1c1c
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fcfc8-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fcfc8-118">Optional query parameters</span></span>
<span data-ttu-id="fcfc8-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fcfc8-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fcfc8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fcfc8-120">Request headers</span></span>
| <span data-ttu-id="fcfc8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fcfc8-121">Header</span></span>       | <span data-ttu-id="fcfc8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="fcfc8-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fcfc8-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fcfc8-123">Authorization</span></span>  | <span data-ttu-id="fcfc8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fcfc8-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fcfc8-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fcfc8-126">Request body</span></span>
<span data-ttu-id="fcfc8-127">Не поставляем тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fcfc8-127">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fcfc8-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="fcfc8-128">Response</span></span>
<span data-ttu-id="fcfc8-129">В случае успешного выполнения этот метод возвращает код ответа и `200 OK` объект [educationAssignmentResource](../resources/educationassignmentresource.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="fcfc8-129">If successful, this method returns a `200 OK` response code and an [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fcfc8-130">Пример</span><span class="sxs-lookup"><span data-stu-id="fcfc8-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="fcfc8-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="fcfc8-131">Request</span></span>
<span data-ttu-id="fcfc8-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fcfc8-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="fcfc8-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="fcfc8-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationassignmentresource"
}-->
```msgraph-interactive
GET /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/resources/8b01c1d0-aafc-4f8c-bd73-89faa3df1c1c
```
# <a name="c"></a>[<span data-ttu-id="fcfc8-134">C#</span><span class="sxs-lookup"><span data-stu-id="fcfc8-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationassignmentresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fcfc8-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fcfc8-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationassignmentresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fcfc8-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fcfc8-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationassignmentresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fcfc8-137">Java</span><span class="sxs-lookup"><span data-stu-id="fcfc8-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationassignmentresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fcfc8-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="fcfc8-138">Response</span></span>
<span data-ttu-id="fcfc8-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="fcfc8-139">The following is an example of the response.</span></span> 

><span data-ttu-id="fcfc8-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="fcfc8-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentResource"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 842

{
  "distributeForStudentWork": true,
  "id": "22002",
  "resource": {
    "createdBy": {
      "user": {
        "displayName": "Shawn Hughes",
        "id": "14012"
      },
    },
    "createdDateTime": "2014-01-01T00:00:00Z",
    "displayName": "Excel workbook 1",
    "lastModifiedBy": {
      "user": {
        "displayName": "Shawn Hughes",
        "id": "14012"
      },
    },
    "lastModifiedDateTime": "2014-01-01T00:00:00Z"
  }
}
    
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get educationAssignmentResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
