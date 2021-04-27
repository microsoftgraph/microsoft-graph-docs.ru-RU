---
title: Перечисление заданий
description: Извлечение списка объектов назначения. Преподавателю или приложению, исполняемом с разрешениями приложений, разрешено видеть все объекты назначения для класса. Учащиеся могут видеть только назначения, которые им назначены.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: a301303904cb042cf2dd87f7bb51b04957cd34bc
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52043978"
---
# <a name="list-assignments"></a><span data-ttu-id="e1cb6-105">Перечисление заданий</span><span class="sxs-lookup"><span data-stu-id="e1cb6-105">List assignments</span></span>

<span data-ttu-id="e1cb6-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1cb6-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1cb6-107">Извлечение списка объектов назначения.</span><span class="sxs-lookup"><span data-stu-id="e1cb6-107">Retrieve a list of assignment objects.</span></span> <span data-ttu-id="e1cb6-108">Преподавателю или приложению, исполняемом с разрешениями приложений, разрешено видеть все объекты назначения для класса.</span><span class="sxs-lookup"><span data-stu-id="e1cb6-108">A teacher or an application executing with application permissions is allowed to see all assignment objects for the class.</span></span> <span data-ttu-id="e1cb6-109">Учащиеся могут видеть только назначения, которые им назначены.</span><span class="sxs-lookup"><span data-stu-id="e1cb6-109">Students can only see assignments that are assigned to them.</span></span>

## <a name="permissions"></a><span data-ttu-id="e1cb6-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e1cb6-110">Permissions</span></span>

<span data-ttu-id="e1cb6-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1cb6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e1cb6-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e1cb6-113">Permission type</span></span>                        | <span data-ttu-id="e1cb6-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e1cb6-114">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="e1cb6-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e1cb6-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="e1cb6-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1cb6-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="e1cb6-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e1cb6-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1cb6-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1cb6-118">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="e1cb6-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e1cb6-119">Application</span></span>                            | <span data-ttu-id="e1cb6-120">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e1cb6-120">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1cb6-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e1cb6-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e1cb6-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e1cb6-122">Optional query parameters</span></span>
<span data-ttu-id="e1cb6-123">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e1cb6-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e1cb6-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e1cb6-124">Request headers</span></span>

| <span data-ttu-id="e1cb6-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e1cb6-125">Header</span></span>        | <span data-ttu-id="e1cb6-126">Значение</span><span class="sxs-lookup"><span data-stu-id="e1cb6-126">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="e1cb6-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e1cb6-127">Authorization</span></span> | <span data-ttu-id="e1cb6-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e1cb6-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e1cb6-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e1cb6-130">Request body</span></span>

<span data-ttu-id="e1cb6-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e1cb6-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1cb6-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1cb6-132">Response</span></span>

<span data-ttu-id="e1cb6-133">В случае успешного выполнения этот метод возвращает код ответа и коллекцию объектов `200 OK` [educationAssignment](../resources/educationassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e1cb6-133">If successful, this method returns a `200 OK` response code and a collection of [educationAssignment](../resources/educationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1cb6-134">Пример</span><span class="sxs-lookup"><span data-stu-id="e1cb6-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e1cb6-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="e1cb6-135">Request</span></span>

<span data-ttu-id="e1cb6-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e1cb6-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_assignments"
}-->

```http
GET https://graph.microsoft.com/beta/education/classes/{id}/assignments
```

##### <a name="response"></a><span data-ttu-id="e1cb6-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1cb6-137">Response</span></span>

<span data-ttu-id="e1cb6-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e1cb6-138">The following is an example of the response.</span></span> 

><span data-ttu-id="e1cb6-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e1cb6-139">**Note:** The response object shown here might be shortened for readability.</span></span>

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
      "addedStudentAction": "none",
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
      "notificationChannelUrl": null,
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