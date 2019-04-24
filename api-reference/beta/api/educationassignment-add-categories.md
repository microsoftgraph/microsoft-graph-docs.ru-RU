---
title: Добавление Едукатионкатегориес
description: Добавление существующего Едукатионкатегори к этому educationAssignment
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: d5fbf5d6db4ade6e44f65c256879c535d2e2a0e2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32458336"
---
# <a name="add-educationcategories"></a><span data-ttu-id="f567b-103">Добавление Едукатионкатегориес</span><span class="sxs-lookup"><span data-stu-id="f567b-103">Add educationCategories</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f567b-104">Добавьте один или несколько существующих объектов [едукатионкатегори](../resources/educationcategory.md) в этот [educationAssignment](../resources/educationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f567b-104">Add one or more existing [educationCategory](../resources/educationcategory.md) objects to this [educationAssignment](../resources/educationassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f567b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f567b-105">Permissions</span></span>
<span data-ttu-id="f567b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f567b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f567b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f567b-108">Permission type</span></span>      | <span data-ttu-id="f567b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f567b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f567b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f567b-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="f567b-111">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f567b-111">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="f567b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f567b-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f567b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f567b-113">Not supported.</span></span>  |
|<span data-ttu-id="f567b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f567b-114">Application</span></span> | <span data-ttu-id="f567b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f567b-115">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="f567b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f567b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/categories/$ref
```
## <a name="request-headers"></a><span data-ttu-id="f567b-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f567b-117">Request headers</span></span>
| <span data-ttu-id="f567b-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f567b-118">Header</span></span>       | <span data-ttu-id="f567b-119">Значение</span><span class="sxs-lookup"><span data-stu-id="f567b-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f567b-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f567b-120">Authorization</span></span>  | <span data-ttu-id="f567b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f567b-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f567b-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f567b-123">Content-Type</span></span>  | <span data-ttu-id="f567b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f567b-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f567b-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f567b-125">Request body</span></span>
<span data-ttu-id="f567b-126">В тексте запроса укажите odata.id существующих объектов [едукатионкатегори](../resources/educationcategory.md) , которые требуется добавить к этому назначению.</span><span class="sxs-lookup"><span data-stu-id="f567b-126">In the request body, supply the odata.id of the existing [educationCategory](../resources/educationcategory.md) object(s) to add to this assignment.</span></span>


## <a name="response"></a><span data-ttu-id="f567b-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="f567b-127">Response</span></span>
<span data-ttu-id="f567b-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f567b-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f567b-129">Пример</span><span class="sxs-lookup"><span data-stu-id="f567b-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f567b-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="f567b-130">Request</span></span>
<span data-ttu-id="f567b-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f567b-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "add_educationcategory_to_educationassignment"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/categories/$ref
Content-type: application/json
Content-length: 212

{
  "@odata.id": "https://graph.microsoft.com/v1.0/education/classes/11021/assignmentCategories/ec98f158-341d-4fea-9f8c-14a250d489ac"
}

```
<span data-ttu-id="f567b-132">В тексте запроса укажите odata.id существующего объекта [едукатионкатегори](../resources/educationcategory.md) , который требуется добавить к этому назначению.</span><span class="sxs-lookup"><span data-stu-id="f567b-132">In the request body, supply the odata.id of the existing [educationCategory](../resources/educationcategory.md) object to add to this assignment.</span></span>
##### <a name="response"></a><span data-ttu-id="f567b-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="f567b-133">Response</span></span>
<span data-ttu-id="f567b-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f567b-134">The following is an example of the response.</span></span> 

><span data-ttu-id="f567b-135">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f567b-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f567b-136">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f567b-136">All of the properties will be returned from an actual call.</span></span>


<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentResource"
} -->
```http
HTTP/1.1 204 No Content
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Add educationCategory to educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignment-add-category.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
