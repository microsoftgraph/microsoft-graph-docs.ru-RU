---
title: Получение educationSubmittedSubmissionResource
description: Возвращает отправленные ресурсов. Это будет доступно для преподавателей после отправки студента и будет доступен для студента после преподаватель выпуска подачи.  Обратите внимание, что учителя можно оставить заметки в некоторые ресурсы.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: bc7b6f9f0a224cf7a9c1e1c069756d8c83e08ba8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926234"
---
# <a name="get-educationsubmittedsubmissionresource"></a><span data-ttu-id="03396-105">Получение educationSubmittedSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="03396-105">Get educationSubmittedSubmissionResource</span></span>

> <span data-ttu-id="03396-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="03396-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="03396-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03396-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="03396-108">Возвращает отправленные ресурсов.</span><span class="sxs-lookup"><span data-stu-id="03396-108">Returns a submitted resource.</span></span> <span data-ttu-id="03396-109">Это будет доступно для преподавателей после отправки студента и будет доступен для студента после преподаватель выпуска подачи.</span><span class="sxs-lookup"><span data-stu-id="03396-109">This will be available to a teacher after a student has submitted, and will be available to the student after the teacher has released the submission.</span></span>  <span data-ttu-id="03396-110">Обратите внимание, что учителя можно оставить заметки в некоторые ресурсы.</span><span class="sxs-lookup"><span data-stu-id="03396-110">Note that teachers can leave notes in some resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="03396-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="03396-111">Permissions</span></span>
<span data-ttu-id="03396-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03396-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03396-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03396-114">Permission type</span></span>      | <span data-ttu-id="03396-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="03396-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="03396-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03396-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="03396-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03396-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="03396-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03396-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="03396-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03396-119">Not supported.</span></span>  |
|<span data-ttu-id="03396-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="03396-120">Application</span></span> | <span data-ttu-id="03396-121">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03396-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="03396-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03396-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/submittedResources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="03396-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="03396-123">Optional query parameters</span></span>
<span data-ttu-id="03396-124">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="03396-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="03396-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="03396-125">Request headers</span></span>
| <span data-ttu-id="03396-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="03396-126">Header</span></span>       | <span data-ttu-id="03396-127">Значение</span><span class="sxs-lookup"><span data-stu-id="03396-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="03396-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="03396-128">Authorization</span></span>  | <span data-ttu-id="03396-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03396-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="03396-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="03396-131">Request body</span></span>
<span data-ttu-id="03396-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="03396-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="03396-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="03396-133">Response</span></span>
<span data-ttu-id="03396-134">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [educationSubmissionResource](../resources/educationsubmissionresource.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="03396-134">If successful, this method returns a `200 OK` response code and an [educationSubmissionResource](../resources/educationsubmissionresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="03396-135">Пример</span><span class="sxs-lookup"><span data-stu-id="03396-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="03396-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="03396-136">Request</span></span>
<span data-ttu-id="03396-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="03396-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationsubmittedsubmissionresource"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/submittedResources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
##### <a name="response"></a><span data-ttu-id="03396-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="03396-138">Response</span></span>
<span data-ttu-id="03396-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="03396-139">The following is an example of the response.</span></span> 

><span data-ttu-id="03396-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="03396-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmittedSubmissionResource"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1152

{
  "assignmentResourceUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeT456457AdW9f/items/017NJZI25NOB5XZNLABF7646XAMDZTQQ6T",
  "id": "f2387c3b-ec39-4bf2-a399-d7242677f024",
  "resource": {
      "@odata.type": "#microsoft.graph.educationWordResource",
      "displayName": "Report.docx",
      "createdDateTime": "2017-10-21T07:52:53.9863696Z",
      "createdBy": {
          "application": null,
          "device": null,
          "user": {
              "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
              "displayName": null
          }
      },
      "lastModifiedDateTime": "2017-10-21T07:52:53.9863696Z",
      "lastModifiedBy": {
          "application": null,
          "device": null,
          "user": {
              "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
              "displayName": null
          }
      },
      "fileUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeTZ_iul5AdW9f/items/017NJZI27BCN2QI2H7HJGLIVPXR6SD2DH6",
      "@odata.type": "microsoft.graph.educationResource"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get educationSubmittedSubmissionResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
