---
title: Получение educationSubmittedSubmissionResource
description: Возвращает отправленные ресурсов. Это будет доступно для преподавателей после отправки студента и будет доступен для студента после преподаватель выпуска подачи.  Обратите внимание, что учителя можно оставить заметки в некоторые ресурсы.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: e529231e6503b67390b7248228af84dc59b5f633
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513279"
---
# <a name="get-educationsubmittedsubmissionresource"></a><span data-ttu-id="12fc1-105">Получение educationSubmittedSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="12fc1-105">Get educationSubmittedSubmissionResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12fc1-106">Возвращает отправленные ресурсов.</span><span class="sxs-lookup"><span data-stu-id="12fc1-106">Returns a submitted resource.</span></span> <span data-ttu-id="12fc1-107">Это будет доступно для преподавателей после отправки студента и будет доступен для студента после преподаватель выпуска подачи.</span><span class="sxs-lookup"><span data-stu-id="12fc1-107">This will be available to a teacher after a student has submitted, and will be available to the student after the teacher has released the submission.</span></span>  <span data-ttu-id="12fc1-108">Обратите внимание, что учителя можно оставить заметки в некоторые ресурсы.</span><span class="sxs-lookup"><span data-stu-id="12fc1-108">Note that teachers can leave notes in some resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="12fc1-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="12fc1-109">Permissions</span></span>
<span data-ttu-id="12fc1-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12fc1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12fc1-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="12fc1-112">Permission type</span></span>      | <span data-ttu-id="12fc1-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="12fc1-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="12fc1-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="12fc1-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="12fc1-115">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="12fc1-115">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="12fc1-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="12fc1-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="12fc1-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12fc1-117">Not supported.</span></span>  |
|<span data-ttu-id="12fc1-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="12fc1-118">Application</span></span> | <span data-ttu-id="12fc1-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12fc1-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="12fc1-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="12fc1-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/submittedResources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="12fc1-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="12fc1-121">Optional query parameters</span></span>
<span data-ttu-id="12fc1-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="12fc1-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="12fc1-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="12fc1-123">Request headers</span></span>
| <span data-ttu-id="12fc1-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="12fc1-124">Header</span></span>       | <span data-ttu-id="12fc1-125">Значение</span><span class="sxs-lookup"><span data-stu-id="12fc1-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="12fc1-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="12fc1-126">Authorization</span></span>  | <span data-ttu-id="12fc1-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="12fc1-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="12fc1-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="12fc1-129">Request body</span></span>
<span data-ttu-id="12fc1-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="12fc1-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="12fc1-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="12fc1-131">Response</span></span>
<span data-ttu-id="12fc1-132">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [educationSubmissionResource](../resources/educationsubmissionresource.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="12fc1-132">If successful, this method returns a `200 OK` response code and an [educationSubmissionResource](../resources/educationsubmissionresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="12fc1-133">Пример</span><span class="sxs-lookup"><span data-stu-id="12fc1-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="12fc1-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="12fc1-134">Request</span></span>
<span data-ttu-id="12fc1-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="12fc1-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationsubmittedsubmissionresource"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/submittedResources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
##### <a name="response"></a><span data-ttu-id="12fc1-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="12fc1-136">Response</span></span>
<span data-ttu-id="12fc1-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="12fc1-137">The following is an example of the response.</span></span> 

><span data-ttu-id="12fc1-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="12fc1-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Get educationSubmittedSubmissionResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsubmittedsubmissionresource-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
