---
title: Перечисление заданий
description: Возвращает список назначений, назначенных пользователю для всех классов. Это пространство имен служебной программы позволяет вызывающему абоненту находить все назначения учащихся в едином вызове, а не запрашивать назначения из каждого класса. Список назначений содержит сведения, необходимые для получения подробных сведений о назначении в пространстве имен класса. Все остальные операции назначения должны использовать пространство имен класса.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 566eaa526981a14ab4ce622fbad9b858f5b40ef9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33321965"
---
# <a name="list-assignments"></a><span data-ttu-id="68c3c-106">Перечисление заданий</span><span class="sxs-lookup"><span data-stu-id="68c3c-106">List assignments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68c3c-107">Возвращает список назначений, назначенных пользователю для всех классов.</span><span class="sxs-lookup"><span data-stu-id="68c3c-107">Returns a list of assignments assigned to a user for all classes.</span></span> <span data-ttu-id="68c3c-108">Это пространство имен служебной программы позволяет вызывающему абоненту находить все назначения учащихся в едином вызове, а не запрашивать назначения из каждого класса.</span><span class="sxs-lookup"><span data-stu-id="68c3c-108">This utility namespace allows a caller to find all a student's assignments in a single call rather than having to request assignments from each class.</span></span> <span data-ttu-id="68c3c-109">Список назначений содержит сведения, необходимые для получения подробных сведений о назначении в пространстве имен класса.</span><span class="sxs-lookup"><span data-stu-id="68c3c-109">The assignment list contains what is needed to get the detailed information for the assignment from within the class namespace.</span></span> <span data-ttu-id="68c3c-110">Все остальные операции назначения должны использовать пространство имен класса.</span><span class="sxs-lookup"><span data-stu-id="68c3c-110">All other operations on the assignment should use the class namespace.</span></span>

## <a name="permissions"></a><span data-ttu-id="68c3c-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="68c3c-111">Permissions</span></span>
<span data-ttu-id="68c3c-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68c3c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68c3c-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="68c3c-114">Permission type</span></span>      | <span data-ttu-id="68c3c-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="68c3c-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="68c3c-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="68c3c-116">Delegated (work or school account)</span></span> | <span data-ttu-id="68c3c-117">EduAssignments. ReadBasic, EduAssignments. Реадвритебасик, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="68c3c-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="68c3c-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="68c3c-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68c3c-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68c3c-119">Not supported.</span></span>   |
|<span data-ttu-id="68c3c-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="68c3c-120">Application</span></span> | <span data-ttu-id="68c3c-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68c3c-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="68c3c-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="68c3c-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/assignments/
GET /education/users/{id}/assignments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="68c3c-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="68c3c-123">Optional query parameters</span></span>
<span data-ttu-id="68c3c-124">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="68c3c-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="68c3c-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="68c3c-125">Request headers</span></span>
| <span data-ttu-id="68c3c-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="68c3c-126">Header</span></span>       | <span data-ttu-id="68c3c-127">Значение</span><span class="sxs-lookup"><span data-stu-id="68c3c-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="68c3c-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="68c3c-128">Authorization</span></span>  | <span data-ttu-id="68c3c-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="68c3c-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="68c3c-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="68c3c-131">Request body</span></span>
<span data-ttu-id="68c3c-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="68c3c-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="68c3c-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="68c3c-133">Response</span></span>
<span data-ttu-id="68c3c-134">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [educationAssignment](../resources/educationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="68c3c-134">If successful, this method returns a `200 OK` response code and a collection of [educationAssignment](../resources/educationassignment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="68c3c-135">Пример</span><span class="sxs-lookup"><span data-stu-id="68c3c-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="68c3c-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="68c3c-136">Request</span></span>
<span data-ttu-id="68c3c-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="68c3c-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_assignments"
}-->
```http 
GET https://graph.microsoft.com/beta/education/me/assignments
```
##### <a name="response"></a><span data-ttu-id="68c3c-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="68c3c-138">Response</span></span>
<span data-ttu-id="68c3c-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="68c3c-139">The following is an example of the response.</span></span> 

><span data-ttu-id="68c3c-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="68c3c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 344

{
  "value": [
    {
      "id": "19002",
      "allowLateSubmissions": true,
      "allowStudentsToAddResourcesToSubmission": true,
      "assignDateTime": "2014-01-01T00:00:00Z",
      "assignTo": {"@odata.type": "microsoft.graph.educationAssignmentRecipient"},
      "assignedDateTime": "2014-01-01T00:00:00Z",
      "classId": "11010",
      "createdBy": {
        "user": {
            "displayName": "Susana Rocha",
            "id": "14012"
          }
      },
      "createdDateTime": "2014-01-01T00:00:00Z",
      "displayName": "Assignment 1",
      "dueDateTime": "2014-01-01T00:00:00Z",
      "grading": {
        "@odata.type": "#microsoft.graph.educationAssignmentPointsGradeType",
        "maxPoints": 100
      },
      "instructions": {
        "content": "Answer every question correctly",
        "contentType": "Text"
      },
      "lastModifiedBy": {
        "user": {
            "displayName": "Susana Rocha",
            "id": "14012"
          }
      },
      "lastModifiedDateTime": "2014-01-01T00:00:00Z",
      "status": "assigned"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List assignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
