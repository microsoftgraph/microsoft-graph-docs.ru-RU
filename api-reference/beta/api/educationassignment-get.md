---
title: Получение educationAssignment
description: " учителя могут видеть все назначения в классе."
ms.openlocfilehash: 9819576d7194a15d47f4ecc2a1bda5fbf7d61751
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074680"
---
# <a name="get-educationassignment"></a><span data-ttu-id="b1378-103">Получение educationAssignment</span><span class="sxs-lookup"><span data-stu-id="b1378-103">Get educationAssignment</span></span>

> <span data-ttu-id="b1378-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b1378-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b1378-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1378-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b1378-106">Получите свойства и связи назначения.</span><span class="sxs-lookup"><span data-stu-id="b1378-106">Get the properties and relationships of an assignment.</span></span> <span data-ttu-id="b1378-107">Студентов доступны только назначения назначенные им; учителя могут видеть все назначения в классе.</span><span class="sxs-lookup"><span data-stu-id="b1378-107">Students can only see assignments assigned to them; teachers can see all assignments in a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1378-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b1378-108">Permissions</span></span>
<span data-ttu-id="b1378-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1378-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b1378-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b1378-111">Permission type</span></span>      | <span data-ttu-id="b1378-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b1378-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b1378-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b1378-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b1378-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b1378-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="b1378-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b1378-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="b1378-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1378-116">Not supported.</span></span>  |
|<span data-ttu-id="b1378-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b1378-117">Application</span></span> | <span data-ttu-id="b1378-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1378-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="b1378-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b1378-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b1378-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b1378-120">Optional query parameters</span></span>
<span data-ttu-id="b1378-121">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="b1378-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b1378-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b1378-122">Request headers</span></span>
| <span data-ttu-id="b1378-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b1378-123">Header</span></span>       | <span data-ttu-id="b1378-124">Значение</span><span class="sxs-lookup"><span data-stu-id="b1378-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b1378-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b1378-125">Authorization</span></span>  | <span data-ttu-id="b1378-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1378-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b1378-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b1378-128">Request body</span></span>
<span data-ttu-id="b1378-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b1378-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b1378-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="b1378-130">Response</span></span>
<span data-ttu-id="b1378-131">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [educationAssignment](../resources/educationassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b1378-131">If successful, this method returns a `200 OK` response code and an [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b1378-132">Пример</span><span class="sxs-lookup"><span data-stu-id="b1378-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b1378-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b1378-133">Request</span></span>
<span data-ttu-id="b1378-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b1378-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationassignment"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11014/assignments/19002
```
##### <a name="response"></a><span data-ttu-id="b1378-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="b1378-135">Response</span></span>
<span data-ttu-id="b1378-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b1378-136">The following is an example of the response.</span></span> 

><span data-ttu-id="b1378-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b1378-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 279

{
  "id": "19002",
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
  "status": "assigned"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->