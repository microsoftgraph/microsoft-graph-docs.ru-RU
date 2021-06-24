---
title: 'educationAssignment: setUpResourcesFolder'
description: Создайте SharePoint папку для отправки файлов для данного образованияAssignment.
localization_priority: Normal
author: sharmas
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 5ca3d7d267551bdeebb7a34a1624a4f1a4caea3f
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53107622"
---
# <a name="educationassignment-setupresourcesfolder"></a><span data-ttu-id="1517d-103">educationAssignment: setUpResourcesFolder</span><span class="sxs-lookup"><span data-stu-id="1517d-103">educationAssignment: setUpResourcesFolder</span></span>

<span data-ttu-id="1517d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1517d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1517d-105">Создайте SharePoint папку для отправки файлов для данного [образованияAssignment](../resources/educationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="1517d-105">Create a SharePoint folder to upload files for a given [educationAssignment](../resources/educationassignment.md).</span></span> 

<span data-ttu-id="1517d-106">Учитель определяет ресурсы для отправки в папку назначения.</span><span class="sxs-lookup"><span data-stu-id="1517d-106">The teacher determines the resources to upload in the assignment's folder.</span></span> 

## <a name="permissions"></a><span data-ttu-id="1517d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1517d-107">Permissions</span></span>
<span data-ttu-id="1517d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1517d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1517d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1517d-110">Permission type</span></span>      | <span data-ttu-id="1517d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1517d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1517d-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1517d-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="1517d-113">EduAssignments.ReadBasic, EduAssignments.Read</span><span class="sxs-lookup"><span data-stu-id="1517d-113">EduAssignments.ReadBasic, EduAssignments.Read</span></span>  |
|<span data-ttu-id="1517d-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1517d-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="1517d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1517d-115">Not supported.</span></span>  |
|<span data-ttu-id="1517d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1517d-116">Application</span></span> | <span data-ttu-id="1517d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1517d-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="1517d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1517d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/setUpResourcesFolder
```
## <a name="request-headers"></a><span data-ttu-id="1517d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1517d-119">Request headers</span></span>
| <span data-ttu-id="1517d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1517d-120">Header</span></span>       | <span data-ttu-id="1517d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="1517d-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1517d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1517d-122">Authorization</span></span>  | <span data-ttu-id="1517d-p102">Bearer `{token}`. Обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="1517d-p102">Bearer `{token}`. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1517d-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1517d-125">Request body</span></span>
<span data-ttu-id="1517d-126">Необходимо предоставить пустой json в качестве `{}` тела запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1517d-126">You need to provide an empty json `{}` as request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="1517d-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="1517d-127">Response</span></span>
<span data-ttu-id="1517d-128">В случае успешного выполнения этот метод возвращает код ответа 200 Ok и [объект educationAssignment](/graph/api/resources/educationAssignment?view=graph-rest-beta&preserve-view=true) в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="1517d-128">If successful, this method returns a 200 Ok response code and [educationAssignment](/graph/api/resources/educationAssignment?view=graph-rest-beta&preserve-view=true) object in the request body.</span></span>

## <a name="example"></a><span data-ttu-id="1517d-129">Пример</span><span class="sxs-lookup"><span data-stu-id="1517d-129">Example</span></span>
<span data-ttu-id="1517d-130">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="1517d-130">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="1517d-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="1517d-131">Request</span></span>
<span data-ttu-id="1517d-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1517d-132">The following is an example of a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1517d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="1517d-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationassignment_setupresourcesfolder"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/beta/education/classes/11012/assignments/19002/setUpResourcesFolder
Content-type: application/json

{
}
```
# <a name="c"></a>[<span data-ttu-id="1517d-134">C#</span><span class="sxs-lookup"><span data-stu-id="1517d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationassignment-setupresourcesfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1517d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1517d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationassignment-setupresourcesfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1517d-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1517d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationassignment-setupresourcesfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1517d-137">Java</span><span class="sxs-lookup"><span data-stu-id="1517d-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationassignment-setupresourcesfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---
### <a name="response"></a><span data-ttu-id="1517d-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="1517d-138">Response</span></span>
<span data-ttu-id="1517d-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1517d-139">The following is an example of a response.</span></span> 

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/classes('955e0bd5-52c2-41ad-b7e8-5b33a18c5e78')/assignments/$entity",
    "classId": "955e0bd5-52c2-41ad-b7e8-5b33a18c5e78",
    "displayName": "Unit 3 Essay",
    "closeDateTime": "2021-04-06T00:00:00Z",
    "dueDateTime": "2021-04-05T00:00:00Z",
    "assignDateTime": "2021-04-01T00:00:00Z",
    "assignedDateTime": null,
    "allowLateSubmissions": true,
    "createdDateTime": "2021-03-04T00:02:31.9834674Z",
    "lastModifiedDateTime": "2021-03-04T00:02:32.0954032Z",
    "allowStudentsToAddResourcesToSubmission": true,
    "status": "draft",
    "notificationChannelUrl": null,
    "addedStudentAction": "assignIfOpen",
    "addToCalendarAction": "studentsAndTeamOwners",
    "id": "18d17255-3278-49fb-8da7-d095b7f610c4",
    "instructions": {
        "content": "Upload a 500 word essay about the theme of nature in a Shakespearean sonnet.",
        "contentType": "text"
    },
    "grading": {
        "@odata.type": "#microsoft.graph.educationAssignmentPointsGradeType",
        "maxPoints": 100
    },
    "assignTo": {
        "@odata.type": "#microsoft.graph.educationAssignmentIndividualRecipient",
        "recipients": [
            "42ff222c-571f-497c-a9d3-f77ea9ece327"
        ]
    },
    "resourcesFolderUrl": "https://graph.microsoft.com/v1.0/drives/b!H0Unq6KJREmMLHgbJXfKw4YTuh2luKRDvUVGQBLOmvaRxxvbedZKT4LKslSIjT9a/items/01SMYGQ3IUCDNLBJ4XCFE3AQMQHTLSLVYX",
    "createdBy": {
        "application": null,
        "device": null,
        "user": {
            "id": "42ff222c-571f-497c-a9d3-f77ea9ece327",
            "displayName": null
        }
    },
    "lastModifiedBy": {
        "application": null,
        "device": null,
        "user": {
            "id": "42ff222c-571f-497c-a9d3-f77ea9ece327",
            "displayName": null
        }
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignment: publish",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

