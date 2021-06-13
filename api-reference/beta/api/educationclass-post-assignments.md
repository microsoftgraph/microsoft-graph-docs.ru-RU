---
title: Создание educationAssignment
description: Создайте новое назначение.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: c15bca046a08b62ff9a3d6cc75631e6a9110ef34
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911783"
---
# <a name="create-educationassignment"></a><span data-ttu-id="f227c-103">Создание educationAssignment</span><span class="sxs-lookup"><span data-stu-id="f227c-103">Create educationAssignment</span></span>

<span data-ttu-id="f227c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f227c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f227c-105">Создайте новое назначение.</span><span class="sxs-lookup"><span data-stu-id="f227c-105">Create a new assignment.</span></span> 

<span data-ttu-id="f227c-106">Только преподаватели в классе могут создать назначение.</span><span class="sxs-lookup"><span data-stu-id="f227c-106">Only teachers in a class can create an assignment.</span></span> <span data-ttu-id="f227c-107">Назначения начинаются в состоянии Draft, что означает, что учащиеся не будут видеть назначение до публикации.</span><span class="sxs-lookup"><span data-stu-id="f227c-107">Assignments start in the Draft state, which means that students will not see the assignment until publication.</span></span>

## <a name="permissions"></a><span data-ttu-id="f227c-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f227c-108">Permissions</span></span>
<span data-ttu-id="f227c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f227c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f227c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f227c-111">Permission type</span></span>      | <span data-ttu-id="f227c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f227c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f227c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f227c-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="f227c-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f227c-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="f227c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f227c-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f227c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f227c-116">Not supported.</span></span>  |
|<span data-ttu-id="f227c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f227c-117">Application</span></span> | <span data-ttu-id="f227c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f227c-118">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f227c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f227c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments
```
## <a name="request-headers"></a><span data-ttu-id="f227c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f227c-120">Request headers</span></span>
| <span data-ttu-id="f227c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f227c-121">Header</span></span>       | <span data-ttu-id="f227c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f227c-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f227c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f227c-123">Authorization</span></span>  | <span data-ttu-id="f227c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f227c-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f227c-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f227c-126">Content-Type</span></span>  | <span data-ttu-id="f227c-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f227c-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f227c-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f227c-128">Request body</span></span>
<span data-ttu-id="f227c-129">В теле запроса поставляют представление JSON объекта [educationAssignment.](../resources/educationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="f227c-129">In the request body, supply a JSON representation of an [educationAssignment](../resources/educationassignment.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="f227c-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="f227c-130">Response</span></span>
<span data-ttu-id="f227c-131">В случае успешного выполнения этот метод возвращает код отклика и `201 Created` объект [educationAssignment](../resources/educationassignment.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f227c-131">If successful, this method returns a `201 Created` response code and an [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f227c-132">Пример</span><span class="sxs-lookup"><span data-stu-id="f227c-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f227c-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="f227c-133">Request</span></span>
<span data-ttu-id="f227c-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f227c-134">The following is an example of the request.</span></span>
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
<span data-ttu-id="f227c-135">В теле запроса поставляют представление JSON объекта [educationAssignment.](../resources/educationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="f227c-135">In the request body, supply a JSON representation of an [educationAssignment](../resources/educationassignment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="f227c-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="f227c-136">Response</span></span>
<span data-ttu-id="f227c-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f227c-137">The following is an example of the response.</span></span> 

><span data-ttu-id="f227c-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f227c-138">**Note:** The response object shown here might be shortened for readability.</span></span>

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


