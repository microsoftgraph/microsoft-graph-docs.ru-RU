---
title: Список назначений
description: Возвращает список назначений, назначенных пользователю для всех классов. Это пространство имен служебной программы позволяет вызывающей стороне найти назначений студента в один вызов, вместо того чтобы запросить назначения каждого класса. В списке назначения содержит, необходимые для получения подробных сведений для назначения из в пространстве имен классов. Все операции для назначения следует использовать пространство имен классов.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: e2e11eb94c07fc523d6d64143ffc3df401fd9906
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515981"
---
# <a name="list-assignments"></a><span data-ttu-id="7278f-106">Список назначений</span><span class="sxs-lookup"><span data-stu-id="7278f-106">List assignments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7278f-107">Возвращает список назначений, назначенных пользователю для всех классов.</span><span class="sxs-lookup"><span data-stu-id="7278f-107">Returns a list of assignments assigned to a user for all classes.</span></span> <span data-ttu-id="7278f-108">Это пространство имен служебной программы позволяет вызывающей стороне найти назначений студента в один вызов, вместо того чтобы запросить назначения каждого класса.</span><span class="sxs-lookup"><span data-stu-id="7278f-108">This utility namespace allows a caller to find all a student's assignments in a single call rather than having to request assignments from each class.</span></span> <span data-ttu-id="7278f-109">В списке назначения содержит, необходимые для получения подробных сведений для назначения из в пространстве имен классов.</span><span class="sxs-lookup"><span data-stu-id="7278f-109">The assignment list contains what is needed to get the detailed information for the assignment from within the class namespace.</span></span> <span data-ttu-id="7278f-110">Все операции для назначения следует использовать пространство имен классов.</span><span class="sxs-lookup"><span data-stu-id="7278f-110">All other operations on the assignment should use the class namespace.</span></span>

## <a name="permissions"></a><span data-ttu-id="7278f-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7278f-111">Permissions</span></span>
<span data-ttu-id="7278f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7278f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7278f-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7278f-114">Permission type</span></span>      | <span data-ttu-id="7278f-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7278f-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7278f-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7278f-116">Delegated (work or school account)</span></span> | <span data-ttu-id="7278f-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7278f-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="7278f-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7278f-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7278f-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7278f-119">Not supported.</span></span>   |
|<span data-ttu-id="7278f-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7278f-120">Application</span></span> | <span data-ttu-id="7278f-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7278f-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="7278f-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7278f-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/assignments/
GET /education/users/{id}/assignments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7278f-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7278f-123">Optional query parameters</span></span>
<span data-ttu-id="7278f-124">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="7278f-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7278f-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7278f-125">Request headers</span></span>
| <span data-ttu-id="7278f-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7278f-126">Header</span></span>       | <span data-ttu-id="7278f-127">Значение</span><span class="sxs-lookup"><span data-stu-id="7278f-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7278f-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7278f-128">Authorization</span></span>  | <span data-ttu-id="7278f-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7278f-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7278f-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7278f-131">Request body</span></span>
<span data-ttu-id="7278f-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7278f-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="7278f-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="7278f-133">Response</span></span>
<span data-ttu-id="7278f-134">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [educationAssignment](../resources/educationassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7278f-134">If successful, this method returns a `200 OK` response code and a collection of [educationAssignment](../resources/educationassignment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7278f-135">Пример</span><span class="sxs-lookup"><span data-stu-id="7278f-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7278f-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="7278f-136">Request</span></span>
<span data-ttu-id="7278f-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7278f-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_assignments"
}-->
```http 
GET https://graph.microsoft.com/beta/education/me/assignments
```
##### <a name="response"></a><span data-ttu-id="7278f-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="7278f-138">Response</span></span>
<span data-ttu-id="7278f-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7278f-139">The following is an example of the response.</span></span> 

><span data-ttu-id="7278f-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7278f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/api/educationuser-list-assignments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
