---
title: Назначение спискаCategories
description: Извлечение списка объектов категории.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 5e07a33e8dd3d3e55fc894e58049a301b1b7a756
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912888"
---
# <a name="list-assignmentcategories"></a><span data-ttu-id="8c9f0-103">Назначение спискаCategories</span><span class="sxs-lookup"><span data-stu-id="8c9f0-103">List assignmentCategories</span></span>

<span data-ttu-id="8c9f0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c9f0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8c9f0-105">Извлечение списка [объектов educationCategory.](../resources/educationcategory.md)</span><span class="sxs-lookup"><span data-stu-id="8c9f0-105">Retrieve a list of [educationCategory](../resources/educationcategory.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="8c9f0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8c9f0-106">Permissions</span></span>

<span data-ttu-id="8c9f0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c9f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8c9f0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c9f0-109">Permission type</span></span>                        | <span data-ttu-id="8c9f0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8c9f0-110">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="8c9f0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c9f0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8c9f0-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c9f0-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="8c9f0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c9f0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c9f0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c9f0-114">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="8c9f0-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="8c9f0-115">Application</span></span>                            | <span data-ttu-id="8c9f0-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c9f0-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c9f0-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c9f0-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignmentCategories
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8c9f0-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8c9f0-118">Optional query parameters</span></span>

<span data-ttu-id="8c9f0-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="8c9f0-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8c9f0-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8c9f0-120">Request headers</span></span>

| <span data-ttu-id="8c9f0-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8c9f0-121">Header</span></span>        | <span data-ttu-id="8c9f0-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8c9f0-122">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="8c9f0-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8c9f0-123">Authorization</span></span> | <span data-ttu-id="8c9f0-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c9f0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8c9f0-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8c9f0-126">Request body</span></span>

<span data-ttu-id="8c9f0-127">Не поставляем тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8c9f0-127">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c9f0-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c9f0-128">Response</span></span>

<span data-ttu-id="8c9f0-129">В случае успешной работы этот метод возвращает код ответа и коллекцию `200 OK` [объектов educationCategory](../resources/educationcategory.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="8c9f0-129">If successful, this method returns a `200 OK` response code and a collection of [educationCategory](../resources/educationcategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c9f0-130">Пример</span><span class="sxs-lookup"><span data-stu-id="8c9f0-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="8c9f0-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c9f0-131">Request</span></span>

<span data-ttu-id="8c9f0-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8c9f0-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["acdefc6b-2dc6-4e71-b1e9-6d9810ab1793"],
  "name": "get_class_categories"
}-->

```http
GET https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentCategories
```

### <a name="response"></a><span data-ttu-id="8c9f0-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c9f0-133">Response</span></span>

<span data-ttu-id="8c9f0-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="8c9f0-134">The following is an example of the response.</span></span> 

><span data-ttu-id="8c9f0-135">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="8c9f0-135">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 218

{
    "@odata.context": "https://graph.microsoft.com/v1.0/education/classes('acdefc6b-2dc6-4e71-b1e9-6d9810ab1793')/assignmentCategories",
    "value": [
      {
          "displayName": "Quizzes",
          "id": "f997a279-6bcf-429e-b1d0-d2320c4b84ab"
      },
      {
          "displayName": "Homework",
          "id": "9b8f8f88-ddfc-4aad-9fe9-280513fffc74"
      }
    ]
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
