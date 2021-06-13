---
title: Создание educationCategories
description: Добавление существующей системы educationCategory в educationAssignment
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 847e720e65da2604a1188d9854e4e10320d0d181
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912969"
---
# <a name="create-educationcategories"></a><span data-ttu-id="728c9-103">Создание educationCategories</span><span class="sxs-lookup"><span data-stu-id="728c9-103">Create educationCategories</span></span>

<span data-ttu-id="728c9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="728c9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="728c9-105">Добавьте в это [educationAssignment](../resources/educationcategory.md) один или несколько существующих объектов [educationCategory.](../resources/educationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="728c9-105">Add one or more existing [educationCategory](../resources/educationcategory.md) objects to this [educationAssignment](../resources/educationassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="728c9-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="728c9-106">Permissions</span></span>
<span data-ttu-id="728c9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="728c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="728c9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="728c9-109">Permission type</span></span>      | <span data-ttu-id="728c9-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="728c9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="728c9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="728c9-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="728c9-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="728c9-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="728c9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="728c9-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="728c9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="728c9-114">Not supported.</span></span>  |
|<span data-ttu-id="728c9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="728c9-115">Application</span></span> | <span data-ttu-id="728c9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="728c9-116">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="728c9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="728c9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/categories/$ref
```
## <a name="request-headers"></a><span data-ttu-id="728c9-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="728c9-118">Request headers</span></span>
| <span data-ttu-id="728c9-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="728c9-119">Header</span></span>       | <span data-ttu-id="728c9-120">Значение</span><span class="sxs-lookup"><span data-stu-id="728c9-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="728c9-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="728c9-121">Authorization</span></span>  | <span data-ttu-id="728c9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="728c9-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="728c9-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="728c9-124">Content-Type</span></span>  | <span data-ttu-id="728c9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="728c9-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="728c9-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="728c9-126">Request body</span></span>
<span data-ttu-id="728c9-127">В теле запроса odata.id существующего объекта [educationCategory(ы)](../resources/educationcategory.md) для добавления к этому назначению.</span><span class="sxs-lookup"><span data-stu-id="728c9-127">In the request body, supply the odata.id of the existing [educationCategory](../resources/educationcategory.md) object(s) to add to this assignment.</span></span>


## <a name="response"></a><span data-ttu-id="728c9-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="728c9-128">Response</span></span>
<span data-ttu-id="728c9-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="728c9-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="728c9-130">Пример</span><span class="sxs-lookup"><span data-stu-id="728c9-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="728c9-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="728c9-131">Request</span></span>
<span data-ttu-id="728c9-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="728c9-132">The following is an example of the request.</span></span>
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
<span data-ttu-id="728c9-133">В теле запроса укажи odata.id существующего объекта [educationCategory,](../resources/educationcategory.md) чтобы добавить к этому назначению.</span><span class="sxs-lookup"><span data-stu-id="728c9-133">In the request body, supply the odata.id of the existing [educationCategory](../resources/educationcategory.md) object to add to this assignment.</span></span>
##### <a name="response"></a><span data-ttu-id="728c9-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="728c9-134">Response</span></span>
<span data-ttu-id="728c9-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="728c9-135">The following is an example of the response.</span></span> 

><span data-ttu-id="728c9-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="728c9-136">**Note:** The response object shown here might be shortened for readability.</span></span>


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
  "suppressions": []
}
-->


