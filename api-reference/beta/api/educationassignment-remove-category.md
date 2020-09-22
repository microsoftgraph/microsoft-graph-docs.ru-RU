---
title: Удаление Едукатионкатегори
description: Удаление существующего Едукатионкатегори из educationAssignment
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: edcc71fcacf96dacdd9200e48f2ddedbbcda381e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48002536"
---
# <a name="remove-educationcategory"></a><span data-ttu-id="bf4f5-103">Удаление Едукатионкатегори</span><span class="sxs-lookup"><span data-stu-id="bf4f5-103">Remove educationCategory</span></span>

<span data-ttu-id="bf4f5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf4f5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf4f5-105">Удаление [едукатионкатегори](../resources/educationcategory.md) из [educationAssignment](../resources/educationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="bf4f5-105">Remove an [educationCategory](../resources/educationcategory.md) from an [educationAssignment](../resources/educationassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bf4f5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bf4f5-106">Permissions</span></span>
<span data-ttu-id="bf4f5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf4f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf4f5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bf4f5-109">Permission type</span></span>      | <span data-ttu-id="bf4f5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bf4f5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bf4f5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bf4f5-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="bf4f5-112">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bf4f5-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="bf4f5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bf4f5-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="bf4f5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf4f5-114">Not supported.</span></span>  |
|<span data-ttu-id="bf4f5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bf4f5-115">Application</span></span> | <span data-ttu-id="bf4f5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf4f5-116">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="bf4f5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bf4f5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/assignments/{id}/categories/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="bf4f5-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bf4f5-118">Request headers</span></span>
| <span data-ttu-id="bf4f5-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bf4f5-119">Header</span></span>       | <span data-ttu-id="bf4f5-120">Значение</span><span class="sxs-lookup"><span data-stu-id="bf4f5-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bf4f5-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bf4f5-121">Authorization</span></span>  | <span data-ttu-id="bf4f5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bf4f5-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bf4f5-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bf4f5-124">Content-Type</span></span>  | <span data-ttu-id="bf4f5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bf4f5-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bf4f5-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bf4f5-126">Request body</span></span>
<span data-ttu-id="bf4f5-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bf4f5-127">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="bf4f5-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf4f5-128">Response</span></span>
<span data-ttu-id="bf4f5-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="bf4f5-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bf4f5-130">Пример</span><span class="sxs-lookup"><span data-stu-id="bf4f5-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bf4f5-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="bf4f5-131">Request</span></span>
<span data-ttu-id="bf4f5-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bf4f5-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "add_educationcategory_to_educationassignment"
}-->
```http
DELETE https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/categories/ec98f158-341d-4fea-9f8c-14a250d489ac/$ref
```

##### <a name="response"></a><span data-ttu-id="bf4f5-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf4f5-133">Response</span></span>
<span data-ttu-id="bf4f5-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="bf4f5-134">The following is an example of the response.</span></span> 

><span data-ttu-id="bf4f5-135">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="bf4f5-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="bf4f5-136">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bf4f5-136">All of the properties will be returned from an actual call.</span></span>


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


