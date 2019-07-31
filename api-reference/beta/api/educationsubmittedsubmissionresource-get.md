---
title: Получение Едукатионсубмиттедсубмиссионресаурце
description: Возвращает отправленный ресурс. Это будет доступно для преподавателя после того, как ученик отправил, и будет доступен студенту после того, как преподаватель выпустит отправку.  Обратите внимание, что преподаватели могут оставлять заметок в некоторых ресурсах.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: f3703de6176af8cc475e83408d77d4880e2ef77b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35954923"
---
# <a name="get-educationsubmittedsubmissionresource"></a><span data-ttu-id="f6366-105">Получение Едукатионсубмиттедсубмиссионресаурце</span><span class="sxs-lookup"><span data-stu-id="f6366-105">Get educationSubmittedSubmissionResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6366-106">Возвращает отправленный ресурс.</span><span class="sxs-lookup"><span data-stu-id="f6366-106">Returns a submitted resource.</span></span> <span data-ttu-id="f6366-107">Это будет доступно для преподавателя после того, как ученик отправил, и будет доступен студенту после того, как преподаватель выпустит отправку.</span><span class="sxs-lookup"><span data-stu-id="f6366-107">This will be available to a teacher after a student has submitted, and will be available to the student after the teacher has released the submission.</span></span>  <span data-ttu-id="f6366-108">Обратите внимание, что преподаватели могут оставлять заметок в некоторых ресурсах.</span><span class="sxs-lookup"><span data-stu-id="f6366-108">Note that teachers can leave notes in some resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="f6366-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f6366-109">Permissions</span></span>
<span data-ttu-id="f6366-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6366-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6366-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f6366-112">Permission type</span></span>      | <span data-ttu-id="f6366-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f6366-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f6366-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f6366-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="f6366-115">EduAssignments. ReadBasic, EduAssignments. Реадвритебасик, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f6366-115">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="f6366-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f6366-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f6366-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6366-117">Not supported.</span></span>  |
|<span data-ttu-id="f6366-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f6366-118">Application</span></span> | <span data-ttu-id="f6366-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f6366-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f6366-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f6366-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/submittedResources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f6366-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="f6366-121">Optional query parameters</span></span>
<span data-ttu-id="f6366-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="f6366-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f6366-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f6366-123">Request headers</span></span>
| <span data-ttu-id="f6366-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f6366-124">Header</span></span>       | <span data-ttu-id="f6366-125">Значение</span><span class="sxs-lookup"><span data-stu-id="f6366-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f6366-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f6366-126">Authorization</span></span>  | <span data-ttu-id="f6366-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f6366-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f6366-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f6366-129">Request body</span></span>
<span data-ttu-id="f6366-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f6366-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f6366-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="f6366-131">Response</span></span>
<span data-ttu-id="f6366-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [едукатионсубмиссионресаурце](../resources/educationsubmissionresource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f6366-132">If successful, this method returns a `200 OK` response code and an [educationSubmissionResource](../resources/educationsubmissionresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f6366-133">Пример</span><span class="sxs-lookup"><span data-stu-id="f6366-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f6366-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="f6366-134">Request</span></span>
<span data-ttu-id="f6366-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f6366-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationsubmittedsubmissionresource"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/submittedResources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
##### <a name="response"></a><span data-ttu-id="f6366-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="f6366-136">Response</span></span>
<span data-ttu-id="f6366-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f6366-137">The following is an example of the response.</span></span> 

><span data-ttu-id="f6366-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f6366-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
