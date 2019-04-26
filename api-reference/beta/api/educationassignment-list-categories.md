---
title: Перечисление категорий
description: ПереЧисление всех категорий, связанных с этим назначением.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 3a66e74a0addd6b6064e1e5ad66aba74895f0451
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324742"
---
# <a name="list-categories"></a><span data-ttu-id="4690f-103">Перечисление категорий</span><span class="sxs-lookup"><span data-stu-id="4690f-103">List categories</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4690f-104">ПереЧисление всех категорий, связанных с этим назначением.</span><span class="sxs-lookup"><span data-stu-id="4690f-104">List all the categories associated with this assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="4690f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4690f-105">Permissions</span></span>
<span data-ttu-id="4690f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4690f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4690f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4690f-108">Permission type</span></span>      | <span data-ttu-id="4690f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4690f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4690f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4690f-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="4690f-111">EduAssignments. ReadBasic, EduAssignments. Реадвритебасик, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4690f-111">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="4690f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4690f-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="4690f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4690f-113">Not supported.</span></span>  |
|<span data-ttu-id="4690f-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="4690f-114">Application</span></span> | <span data-ttu-id="4690f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4690f-115">Not Supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="4690f-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4690f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/categories
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4690f-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4690f-117">Optional query parameters</span></span>
<span data-ttu-id="4690f-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="4690f-118">This method supports the [OData query parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4690f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4690f-119">Request headers</span></span>
| <span data-ttu-id="4690f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4690f-120">Header</span></span>       | <span data-ttu-id="4690f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4690f-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4690f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4690f-122">Authorization</span></span>  | <span data-ttu-id="4690f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4690f-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4690f-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4690f-125">Request body</span></span>
<span data-ttu-id="4690f-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4690f-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="4690f-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="4690f-127">Response</span></span>
<span data-ttu-id="4690f-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [едукатионкатегори](../resources/educationcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4690f-128">If successful, this method returns a `200 OK` response code and collection of [educationCategory](../resources/educationcategory.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4690f-129">Пример</span><span class="sxs-lookup"><span data-stu-id="4690f-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4690f-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="4690f-130">Request</span></span>
<span data-ttu-id="4690f-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4690f-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_submissions"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/categories
```
##### <a name="response"></a><span data-ttu-id="4690f-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="4690f-132">Response</span></span>
<span data-ttu-id="4690f-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4690f-133">The following is an example of the response.</span></span> 

><span data-ttu-id="4690f-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4690f-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4690f-135">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4690f-135">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 873

{
    "value": [{
        "displayName": "Quizzes",
        "id": "ec98f158-341d-4fea-9f8c-14a250d489ac"
    }]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List categories added to an assignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
