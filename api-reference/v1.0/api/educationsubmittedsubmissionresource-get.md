---
title: Get educationSubmittedSubmissionResource
description: Извлечение отправленного ресурса.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 00c9bb49c43dd809945166a6dca4a05a76a87b5f
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912907"
---
# <a name="get-educationsubmittedsubmissionresource"></a><span data-ttu-id="251b5-103">Get educationSubmittedSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="251b5-103">Get educationSubmittedSubmissionResource</span></span>

<span data-ttu-id="251b5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="251b5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="251b5-105">[Извлечение отправленного ресурса.](../resources/educationsubmissionresource.md)</span><span class="sxs-lookup"><span data-stu-id="251b5-105">Retrieve a [submitted resource](../resources/educationsubmissionresource.md).</span></span> 

<span data-ttu-id="251b5-106">Это будет доступно преподавателю или приложению с разрешениями приложения после отправки студента и будет доступно для учащегося после того, как учитель выпустит отправку.</span><span class="sxs-lookup"><span data-stu-id="251b5-106">This will be available to a teacher or an application with application permissions after a student has submitted, and will be available to the student after the teacher has released the submission.</span></span>  <span data-ttu-id="251b5-107">Обратите внимание, что преподаватели могут оставлять заметки в некоторых ресурсах.</span><span class="sxs-lookup"><span data-stu-id="251b5-107">Note that teachers can leave notes in some resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="251b5-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="251b5-108">Permissions</span></span>
<span data-ttu-id="251b5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="251b5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="251b5-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="251b5-111">Permission type</span></span>      | <span data-ttu-id="251b5-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="251b5-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="251b5-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="251b5-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="251b5-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="251b5-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="251b5-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="251b5-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="251b5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="251b5-116">Not supported.</span></span>  |
|<span data-ttu-id="251b5-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="251b5-117">Application</span></span> | <span data-ttu-id="251b5-118">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="251b5-118">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="251b5-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="251b5-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/submittedResources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="251b5-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="251b5-120">Optional query parameters</span></span>
<span data-ttu-id="251b5-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="251b5-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="251b5-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="251b5-122">Request headers</span></span>
| <span data-ttu-id="251b5-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="251b5-123">Header</span></span>       | <span data-ttu-id="251b5-124">Значение</span><span class="sxs-lookup"><span data-stu-id="251b5-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="251b5-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="251b5-125">Authorization</span></span>  | <span data-ttu-id="251b5-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="251b5-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="251b5-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="251b5-128">Request body</span></span>
<span data-ttu-id="251b5-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="251b5-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="251b5-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="251b5-130">Response</span></span>
<span data-ttu-id="251b5-131">В случае успешной работы этот метод возвращает код отклика и `200 OK` объект [educationSubmissionResource](../resources/educationsubmissionresource.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="251b5-131">If successful, this method returns a `200 OK` response code and an [educationSubmissionResource](../resources/educationsubmissionresource.md) object in the response body.</span></span> <span data-ttu-id="251b5-132">В противном случае возвращается `404 Not found` код ответа.</span><span class="sxs-lookup"><span data-stu-id="251b5-132">Otherwise, returns a `404 Not found` response code.</span></span>

## <a name="example"></a><span data-ttu-id="251b5-133">Пример</span><span class="sxs-lookup"><span data-stu-id="251b5-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="251b5-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="251b5-134">Request</span></span>
<span data-ttu-id="251b5-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="251b5-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationsubmittedsubmissionresource"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/classes/f973bc68-2adb-4cf7-8b15-a57a1936b60c/assignments/8b890b42-a1df-478b-bff5-6814afb1afc2/submissions/6d71b348-898a-40cd-8e71-35127eed97f5/submittedResources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
### <a name="response"></a><span data-ttu-id="251b5-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="251b5-136">Response</span></span>
<span data-ttu-id="251b5-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="251b5-137">The following is an example of the response.</span></span> 

><span data-ttu-id="251b5-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="251b5-138">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationResource"
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
