---
title: Удаление Едукатионкатегори
description: Удаление существующего Едукатионкатегори из educationAssignment
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: deb55b14c40acb25b366eec140cbc433e9ee203d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35955671"
---
# <a name="remove-educationcategory"></a><span data-ttu-id="04d39-103">Удаление Едукатионкатегори</span><span class="sxs-lookup"><span data-stu-id="04d39-103">Remove educationCategory</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04d39-104">Удаление [едукатионкатегори](../resources/educationcategory.md) из [educationAssignment](../resources/educationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="04d39-104">Remove an [educationCategory](../resources/educationcategory.md) from an [educationAssignment](../resources/educationassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="04d39-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="04d39-105">Permissions</span></span>
<span data-ttu-id="04d39-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04d39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04d39-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="04d39-108">Permission type</span></span>      | <span data-ttu-id="04d39-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="04d39-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="04d39-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="04d39-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="04d39-111">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04d39-111">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="04d39-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="04d39-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="04d39-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04d39-113">Not supported.</span></span>  |
|<span data-ttu-id="04d39-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="04d39-114">Application</span></span> | <span data-ttu-id="04d39-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04d39-115">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="04d39-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="04d39-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/assignments/{id}/categories/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="04d39-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="04d39-117">Request headers</span></span>
| <span data-ttu-id="04d39-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="04d39-118">Header</span></span>       | <span data-ttu-id="04d39-119">Значение</span><span class="sxs-lookup"><span data-stu-id="04d39-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="04d39-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="04d39-120">Authorization</span></span>  | <span data-ttu-id="04d39-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="04d39-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="04d39-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="04d39-123">Content-Type</span></span>  | <span data-ttu-id="04d39-124">application/json</span><span class="sxs-lookup"><span data-stu-id="04d39-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="04d39-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="04d39-125">Request body</span></span>
<span data-ttu-id="04d39-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="04d39-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="04d39-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="04d39-127">Response</span></span>
<span data-ttu-id="04d39-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="04d39-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="04d39-129">Пример</span><span class="sxs-lookup"><span data-stu-id="04d39-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="04d39-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="04d39-130">Request</span></span>
<span data-ttu-id="04d39-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="04d39-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "add_educationcategory_to_educationassignment"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/categories/ec98f158-341d-4fea-9f8c-14a250d489ac/$ref
```

##### <a name="response"></a><span data-ttu-id="04d39-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="04d39-132">Response</span></span>
<span data-ttu-id="04d39-133">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="04d39-133">The following is an example of the response.</span></span> 

><span data-ttu-id="04d39-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="04d39-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="04d39-135">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="04d39-135">All of the properties will be returned from an actual call.</span></span>


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
  "description": "Remove an educationCategory from an educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
