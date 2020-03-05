---
title: Список Едукатионкатегориес
description: Получение списка объектов Category.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: f647c0b5241dc7ab98d0fda5f3ccce8233a6b557
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42426698"
---
# <a name="list-educationcategories"></a><span data-ttu-id="08cc8-103">Список Едукатионкатегориес</span><span class="sxs-lookup"><span data-stu-id="08cc8-103">List educationCategories</span></span>

<span data-ttu-id="08cc8-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="08cc8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08cc8-105">Получение списка объектов [едукатионкатегори](../resources/educationcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="08cc8-105">Retrieve a list of [educationCategory](../resources/educationcategory.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="08cc8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="08cc8-106">Permissions</span></span>

<span data-ttu-id="08cc8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08cc8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="08cc8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="08cc8-109">Permission type</span></span>                        | <span data-ttu-id="08cc8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="08cc8-110">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="08cc8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="08cc8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="08cc8-112">EduAssignments. ReadBasic, EduAssignments. Реадвритебасик, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="08cc8-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="08cc8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="08cc8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08cc8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08cc8-114">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="08cc8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="08cc8-115">Application</span></span>                            | <span data-ttu-id="08cc8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08cc8-116">Not supported.</span></span>                                                                                         |

## <a name="http-request"></a><span data-ttu-id="08cc8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="08cc8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignmentCategories
```

## <a name="optional-query-parameters"></a><span data-ttu-id="08cc8-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="08cc8-118">Optional query parameters</span></span>

<span data-ttu-id="08cc8-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="08cc8-119">This method supports the [OData query parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="08cc8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="08cc8-120">Request headers</span></span>

| <span data-ttu-id="08cc8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="08cc8-121">Header</span></span>        | <span data-ttu-id="08cc8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="08cc8-122">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="08cc8-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="08cc8-123">Authorization</span></span> | <span data-ttu-id="08cc8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="08cc8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="08cc8-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="08cc8-126">Request body</span></span>

<span data-ttu-id="08cc8-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="08cc8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="08cc8-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="08cc8-128">Response</span></span>

<span data-ttu-id="08cc8-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [едукатионкатегори](../resources/educationcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="08cc8-129">If successful, this method returns a `200 OK` response code and a collection of [educationCategory](../resources/educationcategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08cc8-130">Пример</span><span class="sxs-lookup"><span data-stu-id="08cc8-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="08cc8-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="08cc8-131">Request</span></span>

<span data-ttu-id="08cc8-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="08cc8-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_assignments"
}-->

```http
GET https://graph.microsoft.com/beta/education/classes/{id}/assignmentCategories
```

##### <a name="response"></a><span data-ttu-id="08cc8-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="08cc8-133">Response</span></span>

<span data-ttu-id="08cc8-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="08cc8-134">The following is an example of the response.</span></span> 

><span data-ttu-id="08cc8-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="08cc8-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 218

{
    "value": [{
        "displayName": "Quizzes",
        "id": "ec98f158-341d-4fea-9f8c-14a250d489ac"
    }, {
        "displayName": "Homework",
        "id": "3943e9ea-c69b-4dc9-9674-5f24168cee35"
    }]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List categories",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
