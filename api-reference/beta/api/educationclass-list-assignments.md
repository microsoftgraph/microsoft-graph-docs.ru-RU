---
title: Перечисление заданий
description: Извлечение списка объектов назначения. Преподавателю или приложению, исполняемом с разрешениями приложений, разрешено видеть все объекты назначения для класса. Учащиеся могут видеть только назначения, которые им назначены.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: c88d274a92b0d6b2546fa64e349620af7d7f9353
ms.sourcegitcommit: eb67b0a619a4004c1611304f1252a382264a97f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52061800"
---
# <a name="list-assignments"></a><span data-ttu-id="69fb1-105">Перечисление заданий</span><span class="sxs-lookup"><span data-stu-id="69fb1-105">List assignments</span></span>

<span data-ttu-id="69fb1-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69fb1-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69fb1-107">Извлечение списка объектов назначения.</span><span class="sxs-lookup"><span data-stu-id="69fb1-107">Retrieve a list of assignment objects.</span></span> <span data-ttu-id="69fb1-108">Преподавателю или приложению, исполняемом с разрешениями приложений, разрешено видеть все объекты назначения для класса.</span><span class="sxs-lookup"><span data-stu-id="69fb1-108">A teacher or an application executing with application permissions is allowed to see all assignment objects for the class.</span></span> <span data-ttu-id="69fb1-109">Учащиеся могут видеть только назначения, которые им назначены.</span><span class="sxs-lookup"><span data-stu-id="69fb1-109">Students can only see assignments that are assigned to them.</span></span>

## <a name="permissions"></a><span data-ttu-id="69fb1-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="69fb1-110">Permissions</span></span>

<span data-ttu-id="69fb1-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69fb1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="69fb1-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="69fb1-113">Permission type</span></span>                        | <span data-ttu-id="69fb1-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="69fb1-114">Permissions (from least to most privileged)</span></span>                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="69fb1-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="69fb1-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="69fb1-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="69fb1-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="69fb1-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="69fb1-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69fb1-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="69fb1-118">Not supported.</span></span>                                                                                         |
| <span data-ttu-id="69fb1-119">Приложение\*</span><span class="sxs-lookup"><span data-stu-id="69fb1-119">Application\*</span></span>                           | <span data-ttu-id="69fb1-120">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="69fb1-120">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |

<span data-ttu-id="69fb1-121">\*Разрешения приложения в настоящее время доступны только для частных пользователей предварительного просмотра.</span><span class="sxs-lookup"><span data-stu-id="69fb1-121">\*Application permissions are currently available to private preview customers only.</span></span>

## <a name="http-request"></a><span data-ttu-id="69fb1-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="69fb1-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="69fb1-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="69fb1-123">Optional query parameters</span></span>
<span data-ttu-id="69fb1-124">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="69fb1-124">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="69fb1-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="69fb1-125">Request headers</span></span>

| <span data-ttu-id="69fb1-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="69fb1-126">Header</span></span>        | <span data-ttu-id="69fb1-127">Значение</span><span class="sxs-lookup"><span data-stu-id="69fb1-127">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="69fb1-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="69fb1-128">Authorization</span></span> | <span data-ttu-id="69fb1-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="69fb1-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="69fb1-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="69fb1-131">Request body</span></span>

<span data-ttu-id="69fb1-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="69fb1-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69fb1-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="69fb1-133">Response</span></span>

<span data-ttu-id="69fb1-134">В случае успешного выполнения этот метод возвращает код ответа и коллекцию объектов `200 OK` [educationAssignment](../resources/educationassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="69fb1-134">If successful, this method returns a `200 OK` response code and a collection of [educationAssignment](../resources/educationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69fb1-135">Пример</span><span class="sxs-lookup"><span data-stu-id="69fb1-135">Example</span></span>

##### <a name="request"></a><span data-ttu-id="69fb1-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="69fb1-136">Request</span></span>

<span data-ttu-id="69fb1-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="69fb1-137">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_assignments"
}-->

```http
GET https://graph.microsoft.com/beta/education/classes/{id}/assignments
```

##### <a name="response"></a><span data-ttu-id="69fb1-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="69fb1-138">Response</span></span>

<span data-ttu-id="69fb1-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="69fb1-139">The following is an example of the response.</span></span> 

><span data-ttu-id="69fb1-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="69fb1-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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