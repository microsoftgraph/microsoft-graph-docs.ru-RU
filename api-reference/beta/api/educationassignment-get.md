---
title: Get educationAssignment
description: " преподаватели могут видеть все задания в классе."
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 17cc7921c451fae534cd2bbe278ed89ce5e523af
ms.sourcegitcommit: 86d427ac670ebc3fdcf8e06541218bb74d39279d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/15/2020
ms.locfileid: "49675865"
---
# <a name="get-educationassignment"></a><span data-ttu-id="fd701-103">Get educationAssignment</span><span class="sxs-lookup"><span data-stu-id="fd701-103">Get educationAssignment</span></span>

<span data-ttu-id="fd701-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd701-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd701-105">Получите свойства и связи назначения.</span><span class="sxs-lookup"><span data-stu-id="fd701-105">Get the properties and relationships of an assignment.</span></span> <span data-ttu-id="fd701-106">Учащиеся могут видеть только назначения, которые им назначены; преподаватели могут видеть все задания в классе.</span><span class="sxs-lookup"><span data-stu-id="fd701-106">Students can only see assignments assigned to them; teachers can see all assignments in a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="fd701-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fd701-107">Permissions</span></span>
<span data-ttu-id="fd701-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd701-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="fd701-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fd701-110">Permission type</span></span>      | <span data-ttu-id="fd701-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fd701-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd701-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fd701-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fd701-113">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fd701-113">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> |
|<span data-ttu-id="fd701-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fd701-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="fd701-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd701-115">Not supported.</span></span>  |
|<span data-ttu-id="fd701-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fd701-116">Application</span></span> | <span data-ttu-id="fd701-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fd701-117">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="fd701-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fd701-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fd701-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fd701-119">Optional query parameters</span></span>
<span data-ttu-id="fd701-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="fd701-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fd701-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fd701-121">Request headers</span></span>
| <span data-ttu-id="fd701-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fd701-122">Header</span></span>       | <span data-ttu-id="fd701-123">Значение</span><span class="sxs-lookup"><span data-stu-id="fd701-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fd701-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fd701-124">Authorization</span></span>  | <span data-ttu-id="fd701-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fd701-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fd701-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fd701-127">Request body</span></span>
<span data-ttu-id="fd701-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fd701-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fd701-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd701-129">Response</span></span>
<span data-ttu-id="fd701-130">В случае успешного выполнения этот метод возвращает код отклика и объект `200 OK` [educationAssignment](../resources/educationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fd701-130">If successful, this method returns a `200 OK` response code and an [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fd701-131">Пример</span><span class="sxs-lookup"><span data-stu-id="fd701-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fd701-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="fd701-132">Request</span></span>
<span data-ttu-id="fd701-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fd701-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationassignment"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11014/assignments/19002
```
##### <a name="response"></a><span data-ttu-id="fd701-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd701-134">Response</span></span>
<span data-ttu-id="fd701-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fd701-135">The following is an example of the response.</span></span> 

><span data-ttu-id="fd701-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fd701-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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