---
title: Создание educationAssignment
description: 'Создает новое назначение. Только преподаватели в классе могут создавать назначения. Назначения начинаются в состоянии черновика, что означает, что студенты не увидят назначение, пока не будет вызвана публикация.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: fcaeb3234562479b25eef28d9798187d087ea0ee
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42426467"
---
# <a name="create-educationassignment"></a><span data-ttu-id="bd62a-105">Создание educationAssignment</span><span class="sxs-lookup"><span data-stu-id="bd62a-105">Create educationAssignment</span></span>

<span data-ttu-id="bd62a-106">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="bd62a-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd62a-107">Создает новое назначение.</span><span class="sxs-lookup"><span data-stu-id="bd62a-107">Creates a new assignment.</span></span> <span data-ttu-id="bd62a-108">Только преподаватели в классе могут создавать назначения.</span><span class="sxs-lookup"><span data-stu-id="bd62a-108">Only teachers in a class can create an assignment.</span></span> <span data-ttu-id="bd62a-109">Назначения начинаются в состоянии черновика, что означает, что студенты не увидят назначение, пока не будет вызвана публикация.</span><span class="sxs-lookup"><span data-stu-id="bd62a-109">Assignments start in the Draft state, which means that students will not see the assignment until publish is called.</span></span>  

## <a name="permissions"></a><span data-ttu-id="bd62a-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bd62a-110">Permissions</span></span>
<span data-ttu-id="bd62a-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd62a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd62a-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bd62a-113">Permission type</span></span>      | <span data-ttu-id="bd62a-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bd62a-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bd62a-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bd62a-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="bd62a-116">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bd62a-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="bd62a-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bd62a-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="bd62a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd62a-118">Not supported.</span></span>  |
|<span data-ttu-id="bd62a-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bd62a-119">Application</span></span> | <span data-ttu-id="bd62a-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd62a-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="bd62a-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bd62a-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments

```
## <a name="request-headers"></a><span data-ttu-id="bd62a-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bd62a-122">Request headers</span></span>
| <span data-ttu-id="bd62a-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bd62a-123">Header</span></span>       | <span data-ttu-id="bd62a-124">Значение</span><span class="sxs-lookup"><span data-stu-id="bd62a-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bd62a-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bd62a-125">Authorization</span></span>  | <span data-ttu-id="bd62a-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bd62a-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bd62a-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bd62a-128">Content-Type</span></span>  | <span data-ttu-id="bd62a-129">application/json</span><span class="sxs-lookup"><span data-stu-id="bd62a-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bd62a-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bd62a-130">Request body</span></span>
<span data-ttu-id="bd62a-131">В тексте запроса добавьте представление объекта [educationAssignment](../resources/educationassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bd62a-131">In the request body, supply a JSON representation of an [educationAssignment](../resources/educationassignment.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="bd62a-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd62a-132">Response</span></span>
<span data-ttu-id="bd62a-133">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [educationAssignment](../resources/educationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bd62a-133">If successful, this method returns a `201 Created` response code and an [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd62a-134">Пример</span><span class="sxs-lookup"><span data-stu-id="bd62a-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bd62a-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="bd62a-135">Request</span></span>
<span data-ttu-id="bd62a-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bd62a-136">The following is an example of the request.</span></span>
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
<span data-ttu-id="bd62a-137">В тексте запроса добавьте представление объекта [educationAssignment](../resources/educationassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bd62a-137">In the request body, supply a JSON representation of an [educationAssignment](../resources/educationassignment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="bd62a-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd62a-138">Response</span></span>
<span data-ttu-id="bd62a-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bd62a-139">The following is an example of the response.</span></span> 

><span data-ttu-id="bd62a-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bd62a-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 279

{
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
