---
title: Создание educationAssignment
description: 'Создание нового назначения. Учителя только в классе можно создать назначение. Запустите назначений в черновом варианте, что означает, что студентов не будут отображаться назначения, пока не будет вызван опубликовать.  '
ms.openlocfilehash: 9a6af2a0c0689ca2118ce4d06a55d7b27a70a4ff
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076985"
---
# <a name="create-educationassignment"></a><span data-ttu-id="5e346-105">Создание educationAssignment</span><span class="sxs-lookup"><span data-stu-id="5e346-105">Create educationAssignment</span></span>

> <span data-ttu-id="5e346-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5e346-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5e346-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e346-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5e346-108">Создание нового назначения.</span><span class="sxs-lookup"><span data-stu-id="5e346-108">Creates a new assignment.</span></span> <span data-ttu-id="5e346-109">Учителя только в классе можно создать назначение.</span><span class="sxs-lookup"><span data-stu-id="5e346-109">Only teachers in a class can create an assignment.</span></span> <span data-ttu-id="5e346-110">Запустите назначений в черновом варианте, что означает, что студентов не будут отображаться назначения, пока не будет вызван опубликовать.</span><span class="sxs-lookup"><span data-stu-id="5e346-110">Assignments start in the Draft state, which means that students will not see the assignment until publish is called.</span></span>  

## <a name="permissions"></a><span data-ttu-id="5e346-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5e346-111">Permissions</span></span>
<span data-ttu-id="5e346-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e346-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e346-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5e346-114">Permission type</span></span>      | <span data-ttu-id="5e346-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5e346-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5e346-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5e346-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="5e346-117">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5e346-117">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="5e346-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5e346-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="5e346-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e346-119">Not supported.</span></span>  |
|<span data-ttu-id="5e346-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5e346-120">Application</span></span> | <span data-ttu-id="5e346-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e346-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="5e346-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5e346-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments

```
## <a name="request-headers"></a><span data-ttu-id="5e346-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5e346-123">Request headers</span></span>
| <span data-ttu-id="5e346-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5e346-124">Header</span></span>       | <span data-ttu-id="5e346-125">Значение</span><span class="sxs-lookup"><span data-stu-id="5e346-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5e346-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5e346-126">Authorization</span></span>  | <span data-ttu-id="5e346-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5e346-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5e346-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5e346-129">Content-Type</span></span>  | <span data-ttu-id="5e346-130">application/json</span><span class="sxs-lookup"><span data-stu-id="5e346-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5e346-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5e346-131">Request body</span></span>
<span data-ttu-id="5e346-132">В тексте запроса укажите представление JSON объекта [educationAssignment](../resources/educationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="5e346-132">In the request body, supply a JSON representation of an [educationAssignment](../resources/educationassignment.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="5e346-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="5e346-133">Response</span></span>
<span data-ttu-id="5e346-134">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [educationAssignment](../resources/educationassignment.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5e346-134">If successful, this method returns a `201 Created` response code and an [educationAssignment](../resources/educationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e346-135">Пример</span><span class="sxs-lookup"><span data-stu-id="5e346-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5e346-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="5e346-136">Request</span></span>
<span data-ttu-id="5e346-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5e346-137">The following is an example of the request.</span></span>
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
      "contentType": "Text",
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
<span data-ttu-id="5e346-138">В тексте запроса укажите представление JSON объекта [educationAssignment](../resources/educationassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="5e346-138">In the request body, supply a JSON representation of an [educationAssignment](../resources/educationassignment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="5e346-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="5e346-139">Response</span></span>
<span data-ttu-id="5e346-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5e346-140">The following is an example of the response.</span></span> 

><span data-ttu-id="5e346-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5e346-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "status": "published"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->