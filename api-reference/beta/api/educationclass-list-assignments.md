---
title: Перечисление заданий
description: Получение списка объектов назначений. Преподавателю разрешено просматривать все объекты назначений для этого класса. Студенты могут видеть только назначения, назначенные им.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 71024bec2b359725bda401f20a265cabbfe4ed53
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324782"
---
# <a name="list-assignments"></a><span data-ttu-id="b8ed5-105">Перечисление заданий</span><span class="sxs-lookup"><span data-stu-id="b8ed5-105">List assignments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8ed5-106">Получение списка объектов назначений.</span><span class="sxs-lookup"><span data-stu-id="b8ed5-106">Retrieve a list of assignment objects.</span></span> <span data-ttu-id="b8ed5-107">Преподавателю разрешено просматривать все объекты назначений для этого класса.</span><span class="sxs-lookup"><span data-stu-id="b8ed5-107">A teacher is allowed to see all assignment objects for the class.</span></span> <span data-ttu-id="b8ed5-108">Студенты могут видеть только назначения, назначенные им.</span><span class="sxs-lookup"><span data-stu-id="b8ed5-108">Students can only see assignments that are assigned to them.</span></span>

## <a name="permissions"></a><span data-ttu-id="b8ed5-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b8ed5-109">Permissions</span></span>
<span data-ttu-id="b8ed5-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8ed5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8ed5-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b8ed5-112">Permission type</span></span>      | <span data-ttu-id="b8ed5-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b8ed5-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b8ed5-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b8ed5-114">Delegated (work or school account)</span></span> | <span data-ttu-id="b8ed5-115">EduAssignments. ReadBasic, EduAssignments. Реадвритебасик, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b8ed5-115">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="b8ed5-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b8ed5-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="b8ed5-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8ed5-117">Not supported.</span></span>  |
|<span data-ttu-id="b8ed5-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b8ed5-118">Application</span></span> | <span data-ttu-id="b8ed5-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8ed5-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b8ed5-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b8ed5-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b8ed5-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b8ed5-121">Optional query parameters</span></span>
<span data-ttu-id="b8ed5-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b8ed5-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b8ed5-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b8ed5-123">Request headers</span></span>
| <span data-ttu-id="b8ed5-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b8ed5-124">Header</span></span>       | <span data-ttu-id="b8ed5-125">Значение</span><span class="sxs-lookup"><span data-stu-id="b8ed5-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b8ed5-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b8ed5-126">Authorization</span></span>  | <span data-ttu-id="b8ed5-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b8ed5-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b8ed5-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b8ed5-129">Request body</span></span>
<span data-ttu-id="b8ed5-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b8ed5-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b8ed5-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="b8ed5-131">Response</span></span>
<span data-ttu-id="b8ed5-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [educationAssignment](../resources/educationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b8ed5-132">If successful, this method returns a `200 OK` response code and a collection of [educationAssignment](../resources/educationassignment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b8ed5-133">Пример</span><span class="sxs-lookup"><span data-stu-id="b8ed5-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b8ed5-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="b8ed5-134">Request</span></span>
<span data-ttu-id="b8ed5-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b8ed5-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_assignments"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/<id>/assignments
```
##### <a name="response"></a><span data-ttu-id="b8ed5-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8ed5-136">Response</span></span>
<span data-ttu-id="b8ed5-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b8ed5-137">The following is an example of the response.</span></span> 

><span data-ttu-id="b8ed5-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b8ed5-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
