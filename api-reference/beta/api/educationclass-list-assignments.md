---
title: Список назначений
description: Получение списка объектов назначений. Преподаватель может видеть все объекты назначения для класса. Студентов можно видеть только назначения, которые были им назначены.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 2907a0ce34060246bb4254708049501fdef072ee
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935047"
---
# <a name="list-assignments"></a><span data-ttu-id="8b4de-105">Список назначений</span><span class="sxs-lookup"><span data-stu-id="8b4de-105">List assignments</span></span>

> <span data-ttu-id="8b4de-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8b4de-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8b4de-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b4de-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8b4de-108">Получение списка объектов назначений.</span><span class="sxs-lookup"><span data-stu-id="8b4de-108">Retrieve a list of assignment objects.</span></span> <span data-ttu-id="8b4de-109">Преподаватель может видеть все объекты назначения для класса.</span><span class="sxs-lookup"><span data-stu-id="8b4de-109">A teacher is allowed to see all assignment objects for the class.</span></span> <span data-ttu-id="8b4de-110">Студентов можно видеть только назначения, которые были им назначены.</span><span class="sxs-lookup"><span data-stu-id="8b4de-110">Students can only see assignments that are assigned to them.</span></span>

## <a name="permissions"></a><span data-ttu-id="8b4de-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8b4de-111">Permissions</span></span>
<span data-ttu-id="8b4de-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b4de-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b4de-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8b4de-114">Permission type</span></span>      | <span data-ttu-id="8b4de-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8b4de-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b4de-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b4de-116">Delegated (work or school account)</span></span> | <span data-ttu-id="8b4de-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b4de-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="8b4de-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b4de-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="8b4de-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b4de-119">Not supported.</span></span>  |
|<span data-ttu-id="8b4de-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8b4de-120">Application</span></span> | <span data-ttu-id="8b4de-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b4de-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="8b4de-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8b4de-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8b4de-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="8b4de-123">Optional query parameters</span></span>
<span data-ttu-id="8b4de-124">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="8b4de-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8b4de-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8b4de-125">Request headers</span></span>
| <span data-ttu-id="8b4de-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8b4de-126">Header</span></span>       | <span data-ttu-id="8b4de-127">Значение</span><span class="sxs-lookup"><span data-stu-id="8b4de-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8b4de-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8b4de-128">Authorization</span></span>  | <span data-ttu-id="8b4de-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8b4de-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8b4de-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8b4de-131">Request body</span></span>
<span data-ttu-id="8b4de-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8b4de-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="8b4de-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b4de-133">Response</span></span>
<span data-ttu-id="8b4de-134">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [educationAssignment](../resources/educationassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8b4de-134">If successful, this method returns a `200 OK` response code and a collection of [educationAssignment](../resources/educationassignment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8b4de-135">Пример</span><span class="sxs-lookup"><span data-stu-id="8b4de-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8b4de-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b4de-136">Request</span></span>
<span data-ttu-id="8b4de-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8b4de-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_assignments"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/<id>/assignments
```
##### <a name="response"></a><span data-ttu-id="8b4de-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b4de-138">Response</span></span>
<span data-ttu-id="8b4de-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8b4de-139">The following is an example of the response.</span></span> 

><span data-ttu-id="8b4de-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8b4de-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "assignDateTime": "2014-02-01T00:00:00Z",
      "assignTo": {"@odata.type": "microsoft.graph.educationAssignmentRecipient"},
      "assignedDateTime": "2014-02-01T00:00:00Z",
      "classId": "11018",
      "createdBy": {
          "application": null,
          "device": null,
          "user": {
              "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
              "displayName": null
          }
      },
      "createdDateTime": "2014-02-01T00:00:00Z",
      "displayName": "published",
      "dueDateTime": "2014-02-01T00:00:00Z",
      "grading": {
        "@odata.type": "#microsoft.graph.educationAssignmentPointsGradeType",
        "maxPoints": 100
      },
      "instructions": {
        "contentType": "Text",
        "content": "Read chapters 1 through 3"
      },
      "lastModifiedBy": {
          "application": null,
          "device": null,
          "user": {
              "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
              "displayName": null
          }
      },
      "lastModifiedDateTime": "2014-02-01T00:00:00Z",
      "status": "published"
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
