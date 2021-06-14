---
title: Get educationAssignment
description: Получите свойства и связи назначения.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 4d8eeaa80f94b867f4c0042302681631c343d459
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912786"
---
# <a name="get-educationassignment"></a><span data-ttu-id="2a614-103">Get educationAssignment</span><span class="sxs-lookup"><span data-stu-id="2a614-103">Get educationAssignment</span></span>

<span data-ttu-id="2a614-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a614-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2a614-105">Получите свойства и связи назначения.</span><span class="sxs-lookup"><span data-stu-id="2a614-105">Get the properties and relationships of an assignment.</span></span> 

<span data-ttu-id="2a614-106">Учащиеся могут видеть только назначения, которые им назначены; преподаватели и приложения с разрешениями на приложения могут видеть все назначения в классе.</span><span class="sxs-lookup"><span data-stu-id="2a614-106">Students can only see assignments assigned to them; teachers and applications with application permissions can see all assignments in a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="2a614-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2a614-107">Permissions</span></span>
<span data-ttu-id="2a614-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a614-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2a614-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2a614-110">Permission type</span></span>      | <span data-ttu-id="2a614-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2a614-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2a614-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2a614-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2a614-113">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2a614-113">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="2a614-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2a614-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="2a614-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a614-115">Not supported.</span></span>  |
|<span data-ttu-id="2a614-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="2a614-116">Application</span></span> | <span data-ttu-id="2a614-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2a614-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="2a614-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2a614-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2a614-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2a614-119">Optional query parameters</span></span>
<span data-ttu-id="2a614-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2a614-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2a614-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2a614-121">Request headers</span></span>
| <span data-ttu-id="2a614-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2a614-122">Header</span></span>       | <span data-ttu-id="2a614-123">Значение</span><span class="sxs-lookup"><span data-stu-id="2a614-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2a614-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2a614-124">Authorization</span></span>  | <span data-ttu-id="2a614-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2a614-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2a614-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2a614-127">Request body</span></span>
<span data-ttu-id="2a614-128">Не поставляем тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2a614-128">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a614-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a614-129">Response</span></span>
<span data-ttu-id="2a614-130">В случае успешного выполнения этот метод возвращает код отклика и `200 OK` объект [educationAssignment](../resources/educationassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="2a614-130">If successful, this method returns a `200 OK` response code and an [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a614-131">Пример</span><span class="sxs-lookup"><span data-stu-id="2a614-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="2a614-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="2a614-132">Request</span></span>
<span data-ttu-id="2a614-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2a614-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["1fdf61ee-c129-4960-9b7c-8df159aa64b0"],
  "name": "get_educationassignment"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/5edb6a5f-fc6b-441b-8952-bcbfc33ef0e5/assignments/1fdf61ee-c129-4960-9b7c-8df159aa64b0
```

### <a name="response"></a><span data-ttu-id="2a614-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a614-134">Response</span></span>
<span data-ttu-id="2a614-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2a614-135">The following is an example of the response.</span></span> 

><span data-ttu-id="2a614-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="2a614-136">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 279

{
  "id": "19002",
  "addedStudentAction": "none",
  "allowLateSubmissions": true,
  "allowStudentsToAddResourcesToSubmission": true,
  "assignDateTime": "String (timestamp)",
  "assignTo": {"@odata.type": "microsoft.graph.educationAssignmentRecipient"},
  "assignedDateTime": "2014-01-01T00:00:00Z",
  "classId": "11006",
  "createdBy": {
    "user": {
      "displayName": "Shawn Hughes",
      "id": "14012",
    }
  },
  "closeDateTime": "2014-01-11T00:00:00Z",
  "createdDateTime": "2014-01-01T00:00:00Z",
  "displayName": "Mid term exam",
  "dueDateTime": "2014-01-11T00:00:00Z",
  "resourcesFolderUrl": "https://graph.microsoft.com/v1.0/drives/b!0sGAoOieeE6iSj1WXCV-nYYTuh2luKRDvUVGQBLOmvYpRzc5ARnCRorRht6P3MhU/items/01N74NOEZL7P3VK22SQFDKBZ3PHVPKDVAQ",
  "grading": {
      "@odata.type": "microsoft.graph.educationAssignmentPointsGradeType",
      "maxPoints": 100
  },
  "instructions": {
    "content": "Answer every question correctly",
    "contentType": "Text"
  },
  "lastModifiedBy": {
    "user": {
      "displayName": "Shawn Hughes",
      "id": "14012",
    }
  },
  "lastModifiedDateTime": "2014-01-01T00:00:00Z",
  "notificationChannelUrl": null,
  "status": "assigned"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
