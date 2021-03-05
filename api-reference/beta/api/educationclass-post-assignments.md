---
title: Создание educationAssignment
description: 'Создает новое назначение. Только преподаватели в классе могут создать назначение. Назначения начинаются в состоянии Draft, что означает, что учащиеся не будут видеть назначение до тех пор, пока не будет вызвана публикация.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 399f97fc7e93657f7c3eefb039f5a410121e7a65
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470235"
---
# <a name="create-educationassignment"></a><span data-ttu-id="c9af9-105">Создание educationAssignment</span><span class="sxs-lookup"><span data-stu-id="c9af9-105">Create educationAssignment</span></span>

<span data-ttu-id="c9af9-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9af9-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9af9-107">Создает новое назначение.</span><span class="sxs-lookup"><span data-stu-id="c9af9-107">Creates a new assignment.</span></span> <span data-ttu-id="c9af9-108">Только преподаватели в классе могут создать назначение.</span><span class="sxs-lookup"><span data-stu-id="c9af9-108">Only teachers in a class can create an assignment.</span></span> <span data-ttu-id="c9af9-109">Назначения начинаются в состоянии Draft, что означает, что учащиеся не будут видеть назначение до тех пор, пока не будет вызвана публикация.</span><span class="sxs-lookup"><span data-stu-id="c9af9-109">Assignments start in the Draft state, which means that students will not see the assignment until publish is called.</span></span>  

## <a name="permissions"></a><span data-ttu-id="c9af9-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c9af9-110">Permissions</span></span>
<span data-ttu-id="c9af9-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9af9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9af9-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c9af9-113">Permission type</span></span>      | <span data-ttu-id="c9af9-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c9af9-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c9af9-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c9af9-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="c9af9-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c9af9-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="c9af9-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c9af9-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c9af9-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9af9-118">Not supported.</span></span>  |
|<span data-ttu-id="c9af9-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c9af9-119">Application</span></span> | <span data-ttu-id="c9af9-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9af9-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c9af9-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c9af9-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments
```
## <a name="request-headers"></a><span data-ttu-id="c9af9-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c9af9-122">Request headers</span></span>
| <span data-ttu-id="c9af9-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c9af9-123">Header</span></span>       | <span data-ttu-id="c9af9-124">Значение</span><span class="sxs-lookup"><span data-stu-id="c9af9-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c9af9-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c9af9-125">Authorization</span></span>  | <span data-ttu-id="c9af9-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c9af9-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c9af9-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c9af9-128">Content-Type</span></span>  | <span data-ttu-id="c9af9-129">application/json</span><span class="sxs-lookup"><span data-stu-id="c9af9-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c9af9-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c9af9-130">Request body</span></span>
<span data-ttu-id="c9af9-131">В теле запроса поставляют представление JSON объекта [educationAssignment.](../resources/educationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c9af9-131">In the request body, supply a JSON representation of an [educationAssignment](../resources/educationassignment.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="c9af9-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9af9-132">Response</span></span>
<span data-ttu-id="c9af9-133">В случае успешного выполнения этот метод возвращает код отклика и `201 Created` объект [educationAssignment](../resources/educationassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c9af9-133">If successful, this method returns a `201 Created` response code and an [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9af9-134">Пример</span><span class="sxs-lookup"><span data-stu-id="c9af9-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c9af9-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="c9af9-135">Request</span></span>
<span data-ttu-id="c9af9-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c9af9-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "create_educationassignment_from_educationclass"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11019/assignments
Content-type: application/json
Content-length: 279

{ 
  "dueDateTime": "2014-02-01T00:00:00Z",
  "displayName": "Midterm 1",
    "instructions":  {
      "contentType": "text",
      "content": "Read chapters 1 through 3"
    },
      "grading": {
        "@odata.type": "#microsoft.education.assignments.api.educationAssignmentPointsGradeType",
        "maxPoints": 100
      },
      "assignTo": {
        "@odata.type": "#microsoft.education.assignments.api.educationAssignmentClassRecipient"
      },
      "status":"draft",
      "allowStudentsToAddResourcesToSubmission": true
}
```
<span data-ttu-id="c9af9-137">В теле запроса поставляют представление JSON объекта [educationAssignment.](../resources/educationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c9af9-137">In the request body, supply a JSON representation of an [educationAssignment](../resources/educationassignment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="c9af9-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="c9af9-138">Response</span></span>
<span data-ttu-id="c9af9-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c9af9-139">The following is an example of the response.</span></span> 

><span data-ttu-id="c9af9-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c9af9-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 279

{
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
    "contentType": "text",
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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


