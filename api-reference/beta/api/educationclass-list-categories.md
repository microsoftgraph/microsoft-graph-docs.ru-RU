---
title: List educationCategories
description: Извлечение списка объектов категории.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: db34b97be54750fec02568dd83bab1c4f24a9ed1
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52043929"
---
# <a name="list-educationcategories"></a><span data-ttu-id="1390b-103">List educationCategories</span><span class="sxs-lookup"><span data-stu-id="1390b-103">List educationCategories</span></span>

<span data-ttu-id="1390b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1390b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1390b-105">Извлечение списка [объектов educationCategory.](../resources/educationcategory.md)</span><span class="sxs-lookup"><span data-stu-id="1390b-105">Retrieve a list of [educationCategory](../resources/educationcategory.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="1390b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1390b-106">Permissions</span></span>

<span data-ttu-id="1390b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1390b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1390b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1390b-109">Permission type</span></span>                        | <span data-ttu-id="1390b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1390b-110">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="1390b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1390b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1390b-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1390b-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="1390b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1390b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1390b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1390b-114">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="1390b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1390b-115">Application</span></span>                            | <span data-ttu-id="1390b-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1390b-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1390b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1390b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignmentCategories
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1390b-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1390b-118">Optional query parameters</span></span>

<span data-ttu-id="1390b-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="1390b-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1390b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1390b-120">Request headers</span></span>

| <span data-ttu-id="1390b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1390b-121">Header</span></span>        | <span data-ttu-id="1390b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1390b-122">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="1390b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1390b-123">Authorization</span></span> | <span data-ttu-id="1390b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1390b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1390b-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1390b-126">Request body</span></span>

<span data-ttu-id="1390b-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1390b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1390b-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="1390b-128">Response</span></span>

<span data-ttu-id="1390b-129">В случае успешной работы этот метод возвращает код ответа и коллекцию `200 OK` [объектов educationCategory](../resources/educationcategory.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1390b-129">If successful, this method returns a `200 OK` response code and a collection of [educationCategory](../resources/educationcategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1390b-130">Пример</span><span class="sxs-lookup"><span data-stu-id="1390b-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="1390b-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="1390b-131">Request</span></span>

<span data-ttu-id="1390b-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1390b-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_assignments"
}-->

```http
GET https://graph.microsoft.com/beta/education/classes/{id}/assignmentCategories
```

##### <a name="response"></a><span data-ttu-id="1390b-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="1390b-133">Response</span></span>

<span data-ttu-id="1390b-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1390b-134">The following is an example of the response.</span></span> 

><span data-ttu-id="1390b-135">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1390b-135">**Note:** The response object shown here might be shortened for readability.</span></span>

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