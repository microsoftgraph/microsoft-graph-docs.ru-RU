---
title: Список назначений
description: Возвращает список назначений, назначенных пользователю для всех классов. Это пространство имен служебной программы позволяет вызывающей стороне найти назначений студента в один вызов, вместо того чтобы запросить назначения каждого класса. В списке назначения содержит, необходимые для получения подробных сведений для назначения из в пространстве имен классов. Все операции для назначения следует использовать пространство имен классов.
ms.openlocfilehash: 7c70d6bab1f143caa232e2be89a1f02870d251ac
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075970"
---
# <a name="list-assignments"></a><span data-ttu-id="b1383-106">Список назначений</span><span class="sxs-lookup"><span data-stu-id="b1383-106">List assignments</span></span>

> <span data-ttu-id="b1383-107">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b1383-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b1383-108">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1383-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b1383-109">Возвращает список назначений, назначенных пользователю для всех классов.</span><span class="sxs-lookup"><span data-stu-id="b1383-109">Returns a list of assignments assigned to a user for all classes.</span></span> <span data-ttu-id="b1383-110">Это пространство имен служебной программы позволяет вызывающей стороне найти назначений студента в один вызов, вместо того чтобы запросить назначения каждого класса.</span><span class="sxs-lookup"><span data-stu-id="b1383-110">This utility namespace allows a caller to find all a student's assignments in a single call rather than having to request assignments from each class.</span></span> <span data-ttu-id="b1383-111">В списке назначения содержит, необходимые для получения подробных сведений для назначения из в пространстве имен классов.</span><span class="sxs-lookup"><span data-stu-id="b1383-111">The assignment list contains what is needed to get the detailed information for the assignment from within the class namespace.</span></span> <span data-ttu-id="b1383-112">Все операции для назначения следует использовать пространство имен классов.</span><span class="sxs-lookup"><span data-stu-id="b1383-112">All other operations on the assignment should use the class namespace.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1383-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b1383-113">Permissions</span></span>
<span data-ttu-id="b1383-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1383-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1383-116">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b1383-116">Permission type</span></span>      | <span data-ttu-id="b1383-117">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b1383-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b1383-118">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b1383-118">Delegated (work or school account)</span></span> | <span data-ttu-id="b1383-119">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b1383-119">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="b1383-120">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b1383-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1383-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1383-121">Not supported.</span></span>   |
|<span data-ttu-id="b1383-122">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b1383-122">Application</span></span> | <span data-ttu-id="b1383-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1383-123">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b1383-124">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b1383-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/assignments/
GET /education/users/{id}/assignments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b1383-125">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b1383-125">Optional query parameters</span></span>
<span data-ttu-id="b1383-126">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b1383-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b1383-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b1383-127">Request headers</span></span>
| <span data-ttu-id="b1383-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b1383-128">Header</span></span>       | <span data-ttu-id="b1383-129">Значение</span><span class="sxs-lookup"><span data-stu-id="b1383-129">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b1383-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b1383-130">Authorization</span></span>  | <span data-ttu-id="b1383-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1383-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b1383-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b1383-133">Request body</span></span>
<span data-ttu-id="b1383-134">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b1383-134">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b1383-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="b1383-135">Response</span></span>
<span data-ttu-id="b1383-136">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [educationAssignment](../resources/educationassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b1383-136">If successful, this method returns a `200 OK` response code and a collection of [educationAssignment](../resources/educationassignment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b1383-137">Пример</span><span class="sxs-lookup"><span data-stu-id="b1383-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b1383-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1383-138">Request</span></span>
<span data-ttu-id="b1383-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b1383-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_assignments"
}-->
```http 
GET https://graph.microsoft.com/beta/education/me/assignments
```
##### <a name="response"></a><span data-ttu-id="b1383-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="b1383-140">Response</span></span>
<span data-ttu-id="b1383-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b1383-141">The following is an example of the response.</span></span> 

><span data-ttu-id="b1383-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b1383-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "List assignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->