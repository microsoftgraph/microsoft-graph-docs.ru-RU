---
title: Get educationAssignment
description: " преподаватели могут видеть все назначения в классе."
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 28f129d1621be6a54510a8ef1dd4b48e25e2f5ff
ms.sourcegitcommit: eb67b0a619a4004c1611304f1252a382264a97f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52061716"
---
# <a name="get-educationassignment"></a><span data-ttu-id="5c28e-103">Get educationAssignment</span><span class="sxs-lookup"><span data-stu-id="5c28e-103">Get educationAssignment</span></span>

<span data-ttu-id="5c28e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c28e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c28e-105">Получите свойства и связи назначения.</span><span class="sxs-lookup"><span data-stu-id="5c28e-105">Get the properties and relationships of an assignment.</span></span> <span data-ttu-id="5c28e-106">Учащиеся могут видеть только назначения, которые им назначены; преподаватели и приложения с разрешениями на приложения могут видеть все назначения в классе.</span><span class="sxs-lookup"><span data-stu-id="5c28e-106">Students can only see assignments assigned to them; teachers and applications with application permissions can see all assignments in a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="5c28e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5c28e-107">Permissions</span></span>
<span data-ttu-id="5c28e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c28e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5c28e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5c28e-110">Permission type</span></span>      | <span data-ttu-id="5c28e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5c28e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5c28e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5c28e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5c28e-113">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5c28e-113">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="5c28e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5c28e-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="5c28e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5c28e-115">Not supported.</span></span>  |
|<span data-ttu-id="5c28e-116">Приложение\*</span><span class="sxs-lookup"><span data-stu-id="5c28e-116">Application\*</span></span> | <span data-ttu-id="5c28e-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5c28e-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

<span data-ttu-id="5c28e-118">\*Разрешения приложения в настоящее время доступны только для частных пользователей предварительного просмотра.</span><span class="sxs-lookup"><span data-stu-id="5c28e-118">\*Application permissions are currently available to private preview customers only.</span></span>

## <a name="http-request"></a><span data-ttu-id="5c28e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5c28e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5c28e-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5c28e-120">Optional query parameters</span></span>
<span data-ttu-id="5c28e-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5c28e-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5c28e-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5c28e-122">Request headers</span></span>
| <span data-ttu-id="5c28e-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5c28e-123">Header</span></span>       | <span data-ttu-id="5c28e-124">Значение</span><span class="sxs-lookup"><span data-stu-id="5c28e-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5c28e-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5c28e-125">Authorization</span></span>  | <span data-ttu-id="5c28e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5c28e-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5c28e-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5c28e-128">Request body</span></span>
<span data-ttu-id="5c28e-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5c28e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c28e-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c28e-130">Response</span></span>
<span data-ttu-id="5c28e-131">В случае успешного выполнения этот метод возвращает код отклика и `200 OK` объект [educationAssignment](../resources/educationassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="5c28e-131">If successful, this method returns a `200 OK` response code and an [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5c28e-132">Пример</span><span class="sxs-lookup"><span data-stu-id="5c28e-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5c28e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="5c28e-133">Request</span></span>
<span data-ttu-id="5c28e-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5c28e-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5c28e-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="5c28e-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationassignment"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/11014/assignments/19002
```
# <a name="c"></a>[<span data-ttu-id="5c28e-136">C#</span><span class="sxs-lookup"><span data-stu-id="5c28e-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5c28e-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5c28e-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5c28e-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5c28e-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5c28e-139">Java</span><span class="sxs-lookup"><span data-stu-id="5c28e-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5c28e-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="5c28e-140">Response</span></span>
<span data-ttu-id="5c28e-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="5c28e-141">The following is an example of the response.</span></span> 

><span data-ttu-id="5c28e-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5c28e-142">**Note:** The response object shown here might be shortened for readability.</span></span>

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
      "displayName": "Susana Rocha",
      "id": "14012",
    }
  },
  "closeDateTime": "2014-01-11T00:00:00Z",
  "createdDateTime": "2014-01-01T00:00:00Z",
  "displayName": "Mid term exam",
  "dueDateTime": "2014-01-11T00:00:00Z",
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
