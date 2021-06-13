---
title: Get educationAssignment
description: Получите свойства и связи данного назначения. Обратите внимание, что преподаватели и приложения могут видеть все назначения в классе.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 39daae36befe6a9a3496863d82b1d15bf2e695c3
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911947"
---
# <a name="get-educationassignment"></a><span data-ttu-id="47651-104">Get educationAssignment</span><span class="sxs-lookup"><span data-stu-id="47651-104">Get educationAssignment</span></span>

<span data-ttu-id="47651-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47651-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47651-106">Получите свойства и связи назначения.</span><span class="sxs-lookup"><span data-stu-id="47651-106">Get the properties and relationships of an assignment.</span></span> 

<span data-ttu-id="47651-107">Учащиеся могут видеть только назначения, которые им назначены; преподаватели и приложения с разрешениями на приложения могут видеть все назначения в классе.</span><span class="sxs-lookup"><span data-stu-id="47651-107">Students can only see assignments assigned to them; teachers and applications with application permissions can see all assignments in a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="47651-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="47651-108">Permissions</span></span>
<span data-ttu-id="47651-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47651-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="47651-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47651-111">Permission type</span></span>      | <span data-ttu-id="47651-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="47651-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="47651-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47651-113">Delegated (work or school account)</span></span> | <span data-ttu-id="47651-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="47651-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="47651-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47651-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="47651-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47651-116">Not supported.</span></span>  |
|<span data-ttu-id="47651-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="47651-117">Application</span></span> | <span data-ttu-id="47651-118">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="47651-118">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="47651-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47651-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="47651-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="47651-120">Optional query parameters</span></span>
<span data-ttu-id="47651-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="47651-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="47651-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="47651-122">Request headers</span></span>
| <span data-ttu-id="47651-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="47651-123">Header</span></span>       | <span data-ttu-id="47651-124">Значение</span><span class="sxs-lookup"><span data-stu-id="47651-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="47651-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="47651-125">Authorization</span></span>  | <span data-ttu-id="47651-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="47651-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="47651-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="47651-128">Request body</span></span>
<span data-ttu-id="47651-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="47651-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47651-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="47651-130">Response</span></span>
<span data-ttu-id="47651-131">В случае успешного выполнения этот метод возвращает код отклика и `200 OK` объект [educationAssignment](../resources/educationassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="47651-131">If successful, this method returns a `200 OK` response code and an [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47651-132">Пример</span><span class="sxs-lookup"><span data-stu-id="47651-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="47651-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="47651-133">Request</span></span>
<span data-ttu-id="47651-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47651-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="47651-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="47651-135">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_educationassignment"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/11014/assignments/19002
```
# <a name="c"></a>[<span data-ttu-id="47651-136">C#</span><span class="sxs-lookup"><span data-stu-id="47651-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="47651-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="47651-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="47651-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="47651-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="47651-139">Java</span><span class="sxs-lookup"><span data-stu-id="47651-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="47651-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="47651-140">Response</span></span>
<span data-ttu-id="47651-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="47651-141">The following is an example of the response.</span></span> 

><span data-ttu-id="47651-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="47651-142">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "addToCalendarAction": "studentsAndPublisher",
  "allowLateSubmissions": true,
  "allowStudentsToAddResourcesToSubmission": true,
  "assignDateTime": "String (timestamp)",
  "assignTo": {"@odata.type": "microsoft.graph.educationAssignmentRecipient"},
  "assignedDateTime": "2014-01-01T00:00:00Z",
  "classId": "11006",
  "createdBy": {
    "user": {
      "displayName": "Susana Rocha",
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
      "displayName": "Susana Rocha",
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
