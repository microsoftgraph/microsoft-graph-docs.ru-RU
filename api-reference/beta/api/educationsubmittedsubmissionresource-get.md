---
title: Получение Едукатионсубмиттедсубмиссионресаурце
description: Возвращает отправленный ресурс. Это будет доступно для преподавателя после того, как ученик отправил, и будет доступен студенту после того, как преподаватель выпустит отправку.  Обратите внимание, что преподаватели могут оставлять заметок в некоторых ресурсах.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 0e670022a2d8eb87313952e2429b720bd4a535cf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42424640"
---
# <a name="get-educationsubmittedsubmissionresource"></a><span data-ttu-id="d28fb-105">Получение Едукатионсубмиттедсубмиссионресаурце</span><span class="sxs-lookup"><span data-stu-id="d28fb-105">Get educationSubmittedSubmissionResource</span></span>

<span data-ttu-id="d28fb-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d28fb-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d28fb-107">Возвращает отправленный ресурс.</span><span class="sxs-lookup"><span data-stu-id="d28fb-107">Returns a submitted resource.</span></span> <span data-ttu-id="d28fb-108">Это будет доступно для преподавателя после того, как ученик отправил, и будет доступен студенту после того, как преподаватель выпустит отправку.</span><span class="sxs-lookup"><span data-stu-id="d28fb-108">This will be available to a teacher after a student has submitted, and will be available to the student after the teacher has released the submission.</span></span>  <span data-ttu-id="d28fb-109">Обратите внимание, что преподаватели могут оставлять заметок в некоторых ресурсах.</span><span class="sxs-lookup"><span data-stu-id="d28fb-109">Note that teachers can leave notes in some resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="d28fb-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d28fb-110">Permissions</span></span>
<span data-ttu-id="d28fb-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d28fb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d28fb-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d28fb-113">Permission type</span></span>      | <span data-ttu-id="d28fb-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d28fb-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d28fb-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d28fb-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="d28fb-116">EduAssignments. ReadBasic, EduAssignments. Реадвритебасик, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d28fb-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="d28fb-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d28fb-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d28fb-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d28fb-118">Not supported.</span></span>  |
|<span data-ttu-id="d28fb-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d28fb-119">Application</span></span> | <span data-ttu-id="d28fb-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d28fb-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="d28fb-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d28fb-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/submittedResources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d28fb-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d28fb-122">Optional query parameters</span></span>
<span data-ttu-id="d28fb-123">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d28fb-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d28fb-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d28fb-124">Request headers</span></span>
| <span data-ttu-id="d28fb-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d28fb-125">Header</span></span>       | <span data-ttu-id="d28fb-126">Значение</span><span class="sxs-lookup"><span data-stu-id="d28fb-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d28fb-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d28fb-127">Authorization</span></span>  | <span data-ttu-id="d28fb-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d28fb-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d28fb-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d28fb-130">Request body</span></span>
<span data-ttu-id="d28fb-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d28fb-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d28fb-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="d28fb-132">Response</span></span>
<span data-ttu-id="d28fb-133">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [едукатионсубмиссионресаурце](../resources/educationsubmissionresource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d28fb-133">If successful, this method returns a `200 OK` response code and an [educationSubmissionResource](../resources/educationsubmissionresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d28fb-134">Пример</span><span class="sxs-lookup"><span data-stu-id="d28fb-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d28fb-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="d28fb-135">Request</span></span>
<span data-ttu-id="d28fb-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d28fb-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationsubmittedsubmissionresource"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/submittedResources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
##### <a name="response"></a><span data-ttu-id="d28fb-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="d28fb-137">Response</span></span>
<span data-ttu-id="d28fb-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d28fb-138">The following is an example of the response.</span></span> 

><span data-ttu-id="d28fb-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d28fb-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
