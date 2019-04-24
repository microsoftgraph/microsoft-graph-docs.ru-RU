---
title: Перечисление заданий
description: Возвращает список назначений, назначенных пользователю для всех классов. Это пространство имен служебной программы позволяет вызывающему абоненту находить все назначения учащихся в едином вызове, а не запрашивать назначения из каждого класса. Список назначений содержит сведения, необходимые для получения подробных сведений о назначении в пространстве имен класса. Все остальные операции назначения должны использовать пространство имен класса.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: e2e11eb94c07fc523d6d64143ffc3df401fd9906
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457414"
---
# <a name="list-assignments"></a><span data-ttu-id="d8a0a-106">Перечисление заданий</span><span class="sxs-lookup"><span data-stu-id="d8a0a-106">List assignments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8a0a-107">Возвращает список назначений, назначенных пользователю для всех классов.</span><span class="sxs-lookup"><span data-stu-id="d8a0a-107">Returns a list of assignments assigned to a user for all classes.</span></span> <span data-ttu-id="d8a0a-108">Это пространство имен служебной программы позволяет вызывающему абоненту находить все назначения учащихся в едином вызове, а не запрашивать назначения из каждого класса.</span><span class="sxs-lookup"><span data-stu-id="d8a0a-108">This utility namespace allows a caller to find all a student's assignments in a single call rather than having to request assignments from each class.</span></span> <span data-ttu-id="d8a0a-109">Список назначений содержит сведения, необходимые для получения подробных сведений о назначении в пространстве имен класса.</span><span class="sxs-lookup"><span data-stu-id="d8a0a-109">The assignment list contains what is needed to get the detailed information for the assignment from within the class namespace.</span></span> <span data-ttu-id="d8a0a-110">Все остальные операции назначения должны использовать пространство имен класса.</span><span class="sxs-lookup"><span data-stu-id="d8a0a-110">All other operations on the assignment should use the class namespace.</span></span>

## <a name="permissions"></a><span data-ttu-id="d8a0a-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d8a0a-111">Permissions</span></span>
<span data-ttu-id="d8a0a-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8a0a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8a0a-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d8a0a-114">Permission type</span></span>      | <span data-ttu-id="d8a0a-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d8a0a-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d8a0a-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d8a0a-116">Delegated (work or school account)</span></span> | <span data-ttu-id="d8a0a-117">EduAssignments. ReadBasic, EduAssignments. Реадвритебасик, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d8a0a-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="d8a0a-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d8a0a-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8a0a-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8a0a-119">Not supported.</span></span>   |
|<span data-ttu-id="d8a0a-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d8a0a-120">Application</span></span> | <span data-ttu-id="d8a0a-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8a0a-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d8a0a-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d8a0a-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/assignments/
GET /education/users/{id}/assignments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d8a0a-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d8a0a-123">Optional query parameters</span></span>
<span data-ttu-id="d8a0a-124">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d8a0a-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d8a0a-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d8a0a-125">Request headers</span></span>
| <span data-ttu-id="d8a0a-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d8a0a-126">Header</span></span>       | <span data-ttu-id="d8a0a-127">Значение</span><span class="sxs-lookup"><span data-stu-id="d8a0a-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d8a0a-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d8a0a-128">Authorization</span></span>  | <span data-ttu-id="d8a0a-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d8a0a-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d8a0a-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d8a0a-131">Request body</span></span>
<span data-ttu-id="d8a0a-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d8a0a-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d8a0a-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="d8a0a-133">Response</span></span>
<span data-ttu-id="d8a0a-134">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [educationAssignment](../resources/educationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d8a0a-134">If successful, this method returns a `200 OK` response code and a collection of [educationAssignment](../resources/educationassignment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d8a0a-135">Пример</span><span class="sxs-lookup"><span data-stu-id="d8a0a-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d8a0a-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="d8a0a-136">Request</span></span>
<span data-ttu-id="d8a0a-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d8a0a-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_assignments"
}-->
```http 
GET https://graph.microsoft.com/beta/education/me/assignments
```
##### <a name="response"></a><span data-ttu-id="d8a0a-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8a0a-138">Response</span></span>
<span data-ttu-id="d8a0a-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d8a0a-139">The following is an example of the response.</span></span> 

><span data-ttu-id="d8a0a-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d8a0a-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
