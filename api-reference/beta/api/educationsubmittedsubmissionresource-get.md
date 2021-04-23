---
title: Get educationSubmittedSubmissionResource
description: Возвращает отправленный ресурс. Это будет доступно преподавателю или приложению с разрешениями приложения после отправки студента и будет доступно для учащегося после того, как учитель выпустит отправку.  Обратите внимание, что преподаватели могут оставлять заметки в некоторых ресурсах.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 3a7db3962a2dbc7e012c1e89080008efcd228e52
ms.sourcegitcommit: 2006bf01c60793ac6ab1e25fa0526ec5d33c6334
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/23/2021
ms.locfileid: "51961116"
---
# <a name="get-educationsubmittedsubmissionresource"></a><span data-ttu-id="89780-105">Get educationSubmittedSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="89780-105">Get educationSubmittedSubmissionResource</span></span>

<span data-ttu-id="89780-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89780-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89780-107">Возвращает отправленный ресурс.</span><span class="sxs-lookup"><span data-stu-id="89780-107">Returns a submitted resource.</span></span> <span data-ttu-id="89780-108">Это будет доступно преподавателю или приложению с разрешениями приложения после отправки студента и будет доступно для учащегося после того, как учитель выпустит отправку.</span><span class="sxs-lookup"><span data-stu-id="89780-108">This will be available to a teacher or an application with application permissions after a student has submitted, and will be available to the student after the teacher has released the submission.</span></span>  <span data-ttu-id="89780-109">Обратите внимание, что преподаватели могут оставлять заметки в некоторых ресурсах.</span><span class="sxs-lookup"><span data-stu-id="89780-109">Note that teachers can leave notes in some resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="89780-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="89780-110">Permissions</span></span>
<span data-ttu-id="89780-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89780-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89780-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="89780-113">Permission type</span></span>      | <span data-ttu-id="89780-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="89780-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="89780-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="89780-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="89780-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="89780-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="89780-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="89780-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="89780-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89780-118">Not supported.</span></span>  |
|<span data-ttu-id="89780-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="89780-119">Application</span></span> | <span data-ttu-id="89780-120">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="89780-120">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="89780-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="89780-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/submittedResources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="89780-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="89780-122">Optional query parameters</span></span>
<span data-ttu-id="89780-123">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="89780-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="89780-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="89780-124">Request headers</span></span>
| <span data-ttu-id="89780-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="89780-125">Header</span></span>       | <span data-ttu-id="89780-126">Значение</span><span class="sxs-lookup"><span data-stu-id="89780-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="89780-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="89780-127">Authorization</span></span>  | <span data-ttu-id="89780-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="89780-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="89780-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="89780-130">Request body</span></span>
<span data-ttu-id="89780-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="89780-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="89780-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="89780-132">Response</span></span>
<span data-ttu-id="89780-133">В случае успешной работы этот метод возвращает код отклика и `200 OK` объект [educationSubmissionResource](../resources/educationsubmissionresource.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="89780-133">If successful, this method returns a `200 OK` response code and an [educationSubmissionResource](../resources/educationsubmissionresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="89780-134">Пример</span><span class="sxs-lookup"><span data-stu-id="89780-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="89780-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="89780-135">Request</span></span>
<span data-ttu-id="89780-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="89780-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationsubmittedsubmissionresource"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/submittedResources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
##### <a name="response"></a><span data-ttu-id="89780-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="89780-137">Response</span></span>
<span data-ttu-id="89780-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="89780-138">The following is an example of the response.</span></span> 

><span data-ttu-id="89780-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="89780-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "suppressions": []
}
-->