---
title: Перечисление заданий
description: Получить список объектов назначения. Преподавателю разрешено видеть все объекты заданий для класса. Учащиеся могут видеть только назначения, которые им назначены.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 2667f2248e712cc6f84f6f2214de7006c3b8d3c7
ms.sourcegitcommit: 86d427ac670ebc3fdcf8e06541218bb74d39279d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/15/2020
ms.locfileid: "49675991"
---
# <a name="list-assignments"></a><span data-ttu-id="246e9-105">Перечисление заданий</span><span class="sxs-lookup"><span data-stu-id="246e9-105">List assignments</span></span>

<span data-ttu-id="246e9-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="246e9-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="246e9-107">Получить список объектов назначения.</span><span class="sxs-lookup"><span data-stu-id="246e9-107">Retrieve a list of assignment objects.</span></span> <span data-ttu-id="246e9-108">Преподавателю разрешено видеть все объекты заданий для класса.</span><span class="sxs-lookup"><span data-stu-id="246e9-108">A teacher is allowed to see all assignment objects for the class.</span></span> <span data-ttu-id="246e9-109">Учащиеся могут видеть только назначения, которые им назначены.</span><span class="sxs-lookup"><span data-stu-id="246e9-109">Students can only see assignments that are assigned to them.</span></span>

## <a name="permissions"></a><span data-ttu-id="246e9-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="246e9-110">Permissions</span></span>

<span data-ttu-id="246e9-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="246e9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="246e9-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="246e9-113">Permission type</span></span>                        | <span data-ttu-id="246e9-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="246e9-114">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="246e9-115">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="246e9-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="246e9-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="246e9-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="246e9-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="246e9-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="246e9-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="246e9-118">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="246e9-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="246e9-119">Application</span></span>                            | <span data-ttu-id="246e9-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="246e9-120">Not supported.</span></span>                                                                                         |

## <a name="http-request"></a><span data-ttu-id="246e9-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="246e9-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="246e9-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="246e9-122">Optional query parameters</span></span>
<span data-ttu-id="246e9-123">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="246e9-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="246e9-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="246e9-124">Request headers</span></span>

| <span data-ttu-id="246e9-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="246e9-125">Header</span></span>        | <span data-ttu-id="246e9-126">Значение</span><span class="sxs-lookup"><span data-stu-id="246e9-126">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="246e9-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="246e9-127">Authorization</span></span> | <span data-ttu-id="246e9-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="246e9-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="246e9-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="246e9-130">Request body</span></span>

<span data-ttu-id="246e9-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="246e9-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="246e9-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="246e9-132">Response</span></span>

<span data-ttu-id="246e9-133">В случае успешного выполнения этот метод возвращает код отклика и коллекцию объектов `200 OK` [educationAssignment](../resources/educationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="246e9-133">If successful, this method returns a `200 OK` response code and a collection of [educationAssignment](../resources/educationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="246e9-134">Пример</span><span class="sxs-lookup"><span data-stu-id="246e9-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="246e9-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="246e9-135">Request</span></span>

<span data-ttu-id="246e9-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="246e9-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_assignments"
}-->

```http
GET https://graph.microsoft.com/beta/education/classes/{id}/assignments
```

##### <a name="response"></a><span data-ttu-id="246e9-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="246e9-137">Response</span></span>

<span data-ttu-id="246e9-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="246e9-138">The following is an example of the response.</span></span> 

><span data-ttu-id="246e9-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="246e9-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "addedStudentAction": "String",
      "allowLateSubmissions": true,
      "allowStudentsToAddResourcesToSubmission": true,
      "assignDateTime": "2014-02-01T00:00:00Z",
      "assignTo": {"@odata.type": "microsoft.graph.educationAssignmentRecipient"},
      "assignedDateTime": "2014-02-01T00:00:00Z",
      "classId": "11018",
      "closeDateTime": "2014-02-11T00:00:00Z",
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
      "notificationChannelUrl": "String",
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