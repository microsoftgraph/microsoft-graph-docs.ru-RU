---
title: Создание Едукатионкатегори
description: Создает новую категорию.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 555abb13f9f8910101a8b3d634c56babb6dc0f21
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48007618"
---
# <a name="create-educationcategory"></a><span data-ttu-id="34532-103">Создание Едукатионкатегори</span><span class="sxs-lookup"><span data-stu-id="34532-103">Create educationCategory</span></span>

<span data-ttu-id="34532-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34532-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="34532-105">Создает новый [едукатионкатегори](../resources/educationcategory.md) для [educationClass](../resources/educationclass.md).</span><span class="sxs-lookup"><span data-stu-id="34532-105">Creates a new [educationCategory](../resources/educationcategory.md) on an [educationClass](../resources/educationclass.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="34532-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="34532-106">Permissions</span></span>
<span data-ttu-id="34532-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34532-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34532-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="34532-109">Permission type</span></span>      | <span data-ttu-id="34532-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="34532-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="34532-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="34532-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="34532-112">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="34532-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="34532-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="34532-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="34532-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34532-114">Not supported.</span></span>  |
|<span data-ttu-id="34532-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="34532-115">Application</span></span> | <span data-ttu-id="34532-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34532-116">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="34532-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="34532-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignmentCategories

```
## <a name="request-headers"></a><span data-ttu-id="34532-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="34532-118">Request headers</span></span>
| <span data-ttu-id="34532-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="34532-119">Header</span></span>       | <span data-ttu-id="34532-120">Значение</span><span class="sxs-lookup"><span data-stu-id="34532-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="34532-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="34532-121">Authorization</span></span>  | <span data-ttu-id="34532-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="34532-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="34532-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="34532-124">Content-Type</span></span>  | <span data-ttu-id="34532-125">application/json</span><span class="sxs-lookup"><span data-stu-id="34532-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="34532-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="34532-126">Request body</span></span>
<span data-ttu-id="34532-127">В тексте запроса добавьте представление объекта [едукатионкатегори](../resources/educationcategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="34532-127">In the request body, supply a JSON representation of an [educationCategory](../resources/educationcategory.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="34532-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="34532-128">Response</span></span>
<span data-ttu-id="34532-129">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [едукатионкатегори](../resources/educationcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="34532-129">If successful, this method returns a `201 Created` response code and an [educationCategory](../resources/educationcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34532-130">Пример</span><span class="sxs-lookup"><span data-stu-id="34532-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="34532-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="34532-131">Request</span></span>
<span data-ttu-id="34532-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="34532-132">The following is an example of the request.</span></span>
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
<span data-ttu-id="34532-133">В тексте запроса добавьте представление объекта [едукатионкатегори](../resources/educationcategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="34532-133">In the request body, supply a JSON representation of an [educationCategory](../resources/educationcategory.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="34532-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="34532-134">Response</span></span>
<span data-ttu-id="34532-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="34532-135">The following is an example of the response.</span></span> 

><span data-ttu-id="34532-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="34532-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


