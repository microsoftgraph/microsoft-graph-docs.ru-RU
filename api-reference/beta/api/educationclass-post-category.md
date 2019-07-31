---
title: Создание Едукатионкатегори
description: Создает новую категорию.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 16f7f4bf6ea58aa5d29ae63b95f4b104d0dd1d93
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35955371"
---
# <a name="create-educationcategory"></a><span data-ttu-id="d6278-103">Создание Едукатионкатегори</span><span class="sxs-lookup"><span data-stu-id="d6278-103">Create educationCategory</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6278-104">Создает новый [едукатионкатегори](../resources/educationcategory.md) для [educationClass](../resources/educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="d6278-104">Creates a new [educationCategory](../resources/educationcategory.md) on an [educationClass](../resources/educationclass.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d6278-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d6278-105">Permissions</span></span>
<span data-ttu-id="d6278-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6278-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6278-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d6278-108">Permission type</span></span>      | <span data-ttu-id="d6278-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d6278-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6278-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d6278-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="d6278-111">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d6278-111">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="d6278-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d6278-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d6278-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6278-113">Not supported.</span></span>  |
|<span data-ttu-id="d6278-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d6278-114">Application</span></span> | <span data-ttu-id="d6278-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6278-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d6278-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d6278-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignmentCategories

```
## <a name="request-headers"></a><span data-ttu-id="d6278-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d6278-117">Request headers</span></span>
| <span data-ttu-id="d6278-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d6278-118">Header</span></span>       | <span data-ttu-id="d6278-119">Значение</span><span class="sxs-lookup"><span data-stu-id="d6278-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d6278-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d6278-120">Authorization</span></span>  | <span data-ttu-id="d6278-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d6278-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d6278-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d6278-123">Content-Type</span></span>  | <span data-ttu-id="d6278-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d6278-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d6278-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d6278-125">Request body</span></span>
<span data-ttu-id="d6278-126">В тексте запроса добавьте представление объекта [едукатионкатегори](../resources/educationcategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d6278-126">In the request body, supply a JSON representation of an [educationCategory](../resources/educationcategory.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="d6278-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6278-127">Response</span></span>
<span data-ttu-id="d6278-128">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [едукатионкатегори](../resources/educationcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d6278-128">If successful, this method returns a `201 Created` response code and an [educationCategory](../resources/educationcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6278-129">Пример</span><span class="sxs-lookup"><span data-stu-id="d6278-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d6278-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="d6278-130">Request</span></span>
<span data-ttu-id="d6278-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d6278-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "create_educationcategory_from_educationclass"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11019/assignmentCategories
Content-type: application/json
Content-length: 33

{ 
  "displayName": "Quizzes"
}
```
<span data-ttu-id="d6278-132">В тексте запроса добавьте представление объекта [едукатионкатегори](../resources/educationcategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d6278-132">In the request body, supply a JSON representation of an [educationCategory](../resources/educationcategory.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="d6278-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="d6278-133">Response</span></span>
<span data-ttu-id="d6278-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d6278-134">The following is an example of the response.</span></span> 

><span data-ttu-id="d6278-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d6278-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 85

{
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
