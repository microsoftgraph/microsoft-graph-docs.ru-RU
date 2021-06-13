---
title: Создание educationCategory
description: Создает новую категорию.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: bf0fb3c2459fba0c309e37149e0f87013ff12449
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911776"
---
# <a name="create-educationcategory"></a><span data-ttu-id="e207b-103">Создание educationCategory</span><span class="sxs-lookup"><span data-stu-id="e207b-103">Create educationCategory</span></span>

<span data-ttu-id="e207b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e207b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e207b-105">Создает новое [educationCategory](../resources/educationcategory.md) для [класса educationClass.](../resources/educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="e207b-105">Creates a new [educationCategory](../resources/educationcategory.md) on an [educationClass](../resources/educationclass.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e207b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e207b-106">Permissions</span></span>
<span data-ttu-id="e207b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e207b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e207b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e207b-109">Permission type</span></span>      | <span data-ttu-id="e207b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e207b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e207b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e207b-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="e207b-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e207b-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="e207b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e207b-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e207b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e207b-114">Not supported.</span></span>  |
|<span data-ttu-id="e207b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e207b-115">Application</span></span> | <span data-ttu-id="e207b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e207b-116">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e207b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e207b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignmentCategories

```
## <a name="request-headers"></a><span data-ttu-id="e207b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e207b-118">Request headers</span></span>
| <span data-ttu-id="e207b-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e207b-119">Header</span></span>       | <span data-ttu-id="e207b-120">Значение</span><span class="sxs-lookup"><span data-stu-id="e207b-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e207b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e207b-121">Authorization</span></span>  | <span data-ttu-id="e207b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e207b-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e207b-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e207b-124">Content-Type</span></span>  | <span data-ttu-id="e207b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e207b-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e207b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e207b-126">Request body</span></span>
<span data-ttu-id="e207b-127">В теле запроса поставляют представление JSON объекта [educationCategory.](../resources/educationcategory.md)</span><span class="sxs-lookup"><span data-stu-id="e207b-127">In the request body, supply a JSON representation of an [educationCategory](../resources/educationcategory.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="e207b-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="e207b-128">Response</span></span>
<span data-ttu-id="e207b-129">В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект educationCategory](../resources/educationcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e207b-129">If successful, this method returns a `201 Created` response code and an [educationCategory](../resources/educationcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e207b-130">Пример</span><span class="sxs-lookup"><span data-stu-id="e207b-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e207b-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e207b-131">Request</span></span>
<span data-ttu-id="e207b-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e207b-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["9a5e4047-c1dc-4243-9628-580d3c64b80c"],
  "name": "create_educationcategory_from_educationclass"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/9a5e4047-c1dc-4243-9628-580d3c64b80c/assignmentCategories
Content-type: application/json
Content-length: 33

{ 
  "displayName": "Quizzes"
}
```
<span data-ttu-id="e207b-133">В теле запроса поставляют представление JSON объекта [educationCategory.](../resources/educationcategory.md)</span><span class="sxs-lookup"><span data-stu-id="e207b-133">In the request body, supply a JSON representation of an [educationCategory](../resources/educationcategory.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="e207b-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="e207b-134">Response</span></span>
<span data-ttu-id="e207b-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e207b-135">The following is an example of the response.</span></span> 

><span data-ttu-id="e207b-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e207b-136">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 85

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#education/classes('9a5e4047-c1dc-4243-9628-580d3c64b80c')/assignmentCategories/$entity",
    "displayName": "Quizzes",
    "id": "ec98f158-341d-4fea-9f8c-14a250d489ac"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


