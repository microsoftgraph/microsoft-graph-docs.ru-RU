---
title: Удаление educationCategory
description: Удаление существующей системы educationCategory из этого образованияAssignment
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: c60fd9a3de1d6c66d326ecb0d87416556839c72e
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911552"
---
# <a name="remove-educationcategory"></a><span data-ttu-id="76568-103">Удаление educationCategory</span><span class="sxs-lookup"><span data-stu-id="76568-103">Remove educationCategory</span></span>

<span data-ttu-id="76568-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76568-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="76568-105">Удалите [educationCategory](../resources/educationcategory.md) из [educationAssignment](../resources/educationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="76568-105">Remove an [educationCategory](../resources/educationcategory.md) from an [educationAssignment](../resources/educationassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="76568-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="76568-106">Permissions</span></span>
<span data-ttu-id="76568-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76568-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76568-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="76568-109">Permission type</span></span>      | <span data-ttu-id="76568-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="76568-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="76568-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="76568-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="76568-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="76568-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="76568-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="76568-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="76568-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76568-114">Not supported.</span></span>  |
|<span data-ttu-id="76568-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="76568-115">Application</span></span> | <span data-ttu-id="76568-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76568-116">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="76568-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="76568-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /education/classes/{id}/assignments/{id}/categories/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="76568-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="76568-118">Request headers</span></span>
| <span data-ttu-id="76568-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="76568-119">Header</span></span>       | <span data-ttu-id="76568-120">Значение</span><span class="sxs-lookup"><span data-stu-id="76568-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="76568-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="76568-121">Authorization</span></span>  | <span data-ttu-id="76568-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="76568-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="76568-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="76568-124">Content-Type</span></span>  | <span data-ttu-id="76568-125">application/json</span><span class="sxs-lookup"><span data-stu-id="76568-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="76568-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="76568-126">Request body</span></span>
<span data-ttu-id="76568-127">Не поставляем тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="76568-127">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="76568-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="76568-128">Response</span></span>
<span data-ttu-id="76568-129">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="76568-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="76568-130">Пример</span><span class="sxs-lookup"><span data-stu-id="76568-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="76568-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="76568-131">Request</span></span>
<span data-ttu-id="76568-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="76568-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["ec98f158-341d-4fea-9f8c-14a250d489ac"],
  "name": "add_educationcategory_to_educationassignment"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/categories/ec98f158-341d-4fea-9f8c-14a250d489ac/$ref
```

### <a name="response"></a><span data-ttu-id="76568-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="76568-133">Response</span></span>
<span data-ttu-id="76568-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="76568-134">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentResource"
} -->
```http
HTTP/1.1 204 No Content

{
}
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


