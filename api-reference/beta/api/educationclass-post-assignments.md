---
title: Создание educationAssignment
description: 'Создает новое назначение. Только преподаватели в классе могут создавать назначения. Назначения начинаются в состоянии черновика, что означает, что студенты не увидят назначение, пока не будет вызвана публикация.  '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 2fe916bf7b37e7c7ee2e0487185b585075fd32cc
ms.sourcegitcommit: f23cc661a0e30d01a6b59cfdae90768c55b80ae2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/08/2019
ms.locfileid: "37418232"
---
# <a name="create-educationassignment"></a><span data-ttu-id="df042-105">Создание educationAssignment</span><span class="sxs-lookup"><span data-stu-id="df042-105">Create educationAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df042-106">Создает новое назначение.</span><span class="sxs-lookup"><span data-stu-id="df042-106">Creates a new assignment.</span></span> <span data-ttu-id="df042-107">Только преподаватели в классе могут создавать назначения.</span><span class="sxs-lookup"><span data-stu-id="df042-107">Only teachers in a class can create an assignment.</span></span> <span data-ttu-id="df042-108">Назначения начинаются в состоянии черновика, что означает, что студенты не увидят назначение, пока не будет вызвана публикация.</span><span class="sxs-lookup"><span data-stu-id="df042-108">Assignments start in the Draft state, which means that students will not see the assignment until publish is called.</span></span>  

## <a name="permissions"></a><span data-ttu-id="df042-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="df042-109">Permissions</span></span>
<span data-ttu-id="df042-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df042-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df042-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="df042-112">Permission type</span></span>      | <span data-ttu-id="df042-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="df042-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="df042-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="df042-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="df042-115">EduAssignments. Реадвритебасик, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="df042-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="df042-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="df042-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="df042-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df042-117">Not supported.</span></span>  |
|<span data-ttu-id="df042-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="df042-118">Application</span></span> | <span data-ttu-id="df042-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df042-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="df042-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="df042-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments

```
## <a name="request-headers"></a><span data-ttu-id="df042-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="df042-121">Request headers</span></span>
| <span data-ttu-id="df042-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="df042-122">Header</span></span>       | <span data-ttu-id="df042-123">Значение</span><span class="sxs-lookup"><span data-stu-id="df042-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="df042-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="df042-124">Authorization</span></span>  | <span data-ttu-id="df042-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="df042-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="df042-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="df042-127">Content-Type</span></span>  | <span data-ttu-id="df042-128">application/json</span><span class="sxs-lookup"><span data-stu-id="df042-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="df042-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="df042-129">Request body</span></span>
<span data-ttu-id="df042-130">В тексте запроса добавьте представление объекта [educationAssignment](../resources/educationassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="df042-130">In the request body, supply a JSON representation of an [educationAssignment](../resources/educationassignment.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="df042-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="df042-131">Response</span></span>
<span data-ttu-id="df042-132">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [educationAssignment](../resources/educationassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="df042-132">If successful, this method returns a `201 Created` response code and an [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df042-133">Пример</span><span class="sxs-lookup"><span data-stu-id="df042-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="df042-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="df042-134">Request</span></span>
<span data-ttu-id="df042-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="df042-135">The following is an example of the request.</span></span>
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
<span data-ttu-id="df042-136">В тексте запроса добавьте представление объекта [educationAssignment](../resources/educationassignment.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="df042-136">In the request body, supply a JSON representation of an [educationAssignment](../resources/educationassignment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="df042-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="df042-137">Response</span></span>
<span data-ttu-id="df042-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="df042-138">The following is an example of the response.</span></span> 

><span data-ttu-id="df042-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="df042-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
