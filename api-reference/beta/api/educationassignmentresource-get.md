---
title: Получение Едукатионассигнментресаурце
description: 'Получение свойств определенного ресурса для назначения.  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 1d982092d35ae12aa660bce9c9a9e229395b6df1
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35860710"
---
# <a name="get-educationassignmentresource"></a><span data-ttu-id="174a2-103">Получение Едукатионассигнментресаурце</span><span class="sxs-lookup"><span data-stu-id="174a2-103">Get educationAssignmentResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="174a2-104">Получение свойств определенного ресурса для назначения.</span><span class="sxs-lookup"><span data-stu-id="174a2-104">Get the properties of a specific resource on an assignment.</span></span>  
## <a name="permissions"></a><span data-ttu-id="174a2-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="174a2-105">Permissions</span></span>
<span data-ttu-id="174a2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="174a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="174a2-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="174a2-108">Permission type</span></span>      | <span data-ttu-id="174a2-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="174a2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="174a2-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="174a2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="174a2-111">EduAssignments. ReadBasic, EduAssignments. Реадвритебасик, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="174a2-111">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="174a2-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="174a2-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="174a2-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="174a2-113">Not supported.</span></span>  |
|<span data-ttu-id="174a2-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="174a2-114">Application</span></span> |  <span data-ttu-id="174a2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="174a2-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="174a2-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="174a2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/resources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="174a2-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="174a2-117">Optional query parameters</span></span>
<span data-ttu-id="174a2-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="174a2-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="174a2-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="174a2-119">Request headers</span></span>
| <span data-ttu-id="174a2-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="174a2-120">Header</span></span>       | <span data-ttu-id="174a2-121">Значение</span><span class="sxs-lookup"><span data-stu-id="174a2-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="174a2-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="174a2-122">Authorization</span></span>  | <span data-ttu-id="174a2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="174a2-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="174a2-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="174a2-125">Request body</span></span>
<span data-ttu-id="174a2-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="174a2-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="174a2-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="174a2-127">Response</span></span>
<span data-ttu-id="174a2-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [едукатионассигнментресаурце](../resources/educationassignmentresource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="174a2-128">If successful, this method returns a `200 OK` response code and an [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="174a2-129">Пример</span><span class="sxs-lookup"><span data-stu-id="174a2-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="174a2-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="174a2-130">Request</span></span>
<span data-ttu-id="174a2-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="174a2-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="174a2-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="174a2-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationassignmentresource"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources/22002
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="174a2-133">C#</span><span class="sxs-lookup"><span data-stu-id="174a2-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationassignmentresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="174a2-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="174a2-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationassignmentresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="174a2-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="174a2-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationassignmentresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="174a2-136">Java</span><span class="sxs-lookup"><span data-stu-id="174a2-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationassignmentresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="174a2-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="174a2-137">Response</span></span>
<span data-ttu-id="174a2-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="174a2-138">The following is an example of the response.</span></span> 

><span data-ttu-id="174a2-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="174a2-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="174a2-140">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="174a2-140">All of the properties will be returned from an actual call.</span></span>

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
        "displayName": "Susana Rocha",
        "id": "14012"
      },
    },
    "createdDateTime": "2014-01-01T00:00:00Z",
    "displayName": "Excel workbook 1",
    "lastModifiedBy": {
      "user": {
        "displayName": "Susana Rocha",
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
