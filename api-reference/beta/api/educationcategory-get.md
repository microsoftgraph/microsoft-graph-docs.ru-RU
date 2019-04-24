---
title: Получение Едукатионкатегори
description: Получение объекта Category.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: a26edfd8fe3296f92c7f62b40eea7d3be35722a5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457931"
---
# <a name="get-educationcategory"></a><span data-ttu-id="076d6-103">Получение Едукатионкатегори</span><span class="sxs-lookup"><span data-stu-id="076d6-103">Get educationCategory</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="076d6-104">Получение объекта [едукатионкатегори](../resources/educationcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="076d6-104">Retrieve an [educationCategory](../resources/educationcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="076d6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="076d6-105">Permissions</span></span>
<span data-ttu-id="076d6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="076d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="076d6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="076d6-108">Permission type</span></span>      | <span data-ttu-id="076d6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="076d6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="076d6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="076d6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="076d6-111">EduAssignments. ReadBasic, EduAssignments. Реадвритебасик, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="076d6-111">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="076d6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="076d6-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="076d6-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="076d6-113">Not supported.</span></span>  |
|<span data-ttu-id="076d6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="076d6-114">Application</span></span> | <span data-ttu-id="076d6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="076d6-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="076d6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="076d6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignmentCategories/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="076d6-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="076d6-117">Optional query parameters</span></span>
<span data-ttu-id="076d6-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="076d6-118">This method supports the [OData query parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="076d6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="076d6-119">Request headers</span></span>
| <span data-ttu-id="076d6-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="076d6-120">Header</span></span>       | <span data-ttu-id="076d6-121">Значение</span><span class="sxs-lookup"><span data-stu-id="076d6-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="076d6-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="076d6-122">Authorization</span></span>  | <span data-ttu-id="076d6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="076d6-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="076d6-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="076d6-125">Request body</span></span>
<span data-ttu-id="076d6-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="076d6-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="076d6-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="076d6-127">Response</span></span>
<span data-ttu-id="076d6-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [едукатионкатегори](../resources/educationcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="076d6-128">If successful, this method returns a `200 OK` response code and a [educationCategory](../resources/educationcategory.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="076d6-129">Пример</span><span class="sxs-lookup"><span data-stu-id="076d6-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="076d6-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="076d6-130">Request</span></span>
<span data-ttu-id="076d6-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="076d6-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_assignments"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/<id>/assignmentCategories/<id>
```
##### <a name="response"></a><span data-ttu-id="076d6-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="076d6-132">Response</span></span>
<span data-ttu-id="076d6-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="076d6-133">The following is an example of the response.</span></span> 

><span data-ttu-id="076d6-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="076d6-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 85

{
    "displayName": "Quizzes",
    "id": "ec98f158-341d-4fea-9f8c-14a250d489ac"
}```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get category",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationclass-get-category.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
