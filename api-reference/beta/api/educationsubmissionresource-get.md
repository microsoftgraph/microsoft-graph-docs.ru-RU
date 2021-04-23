---
title: Get educationSubmissionResource
description: Извлекает свойства определенного ресурса, связанного с отправкой. Этот ресурс находится в "рабочем" списке ресурсов и должен рассматриваться студентом в процессе работы. Этот ресурс завернут с помощью возможного указателя обратно в ресурс назначения, если он был скопирован из назначения.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 66342daf0483087d29dd508905a6440cf5a77bd3
ms.sourcegitcommit: 2006bf01c60793ac6ab1e25fa0526ec5d33c6334
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/23/2021
ms.locfileid: "51961151"
---
# <a name="get-educationsubmissionresource"></a><span data-ttu-id="895ff-105">Get educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="895ff-105">Get educationSubmissionResource</span></span>

<span data-ttu-id="895ff-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="895ff-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="895ff-107">Извлекает свойства определенного ресурса, связанного с отправкой.</span><span class="sxs-lookup"><span data-stu-id="895ff-107">Retrieves the properties of a specific resource associated with the submission.</span></span> <span data-ttu-id="895ff-108">Этот ресурс находится в "рабочем" списке ресурсов и должен рассматриваться студентом в процессе работы.</span><span class="sxs-lookup"><span data-stu-id="895ff-108">This resource is in the "working" resource list and should be considered work in process by a student.</span></span> <span data-ttu-id="895ff-109">Этот ресурс завернут с помощью возможного указателя обратно в ресурс назначения, если он был скопирован из назначения.</span><span class="sxs-lookup"><span data-stu-id="895ff-109">This resource is wrapped with a possible pointer back to the assignment resource if it was copied from the assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="895ff-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="895ff-110">Permissions</span></span>
<span data-ttu-id="895ff-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="895ff-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="895ff-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="895ff-113">Permission type</span></span>      | <span data-ttu-id="895ff-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="895ff-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="895ff-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="895ff-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="895ff-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="895ff-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="895ff-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="895ff-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="895ff-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="895ff-118">Not supported.</span></span>  |
|<span data-ttu-id="895ff-119">Приложение</span><span class="sxs-lookup"><span data-stu-id="895ff-119">Application</span></span> | <span data-ttu-id="895ff-120">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="895ff-120">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="895ff-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="895ff-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/resources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="895ff-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="895ff-122">Optional query parameters</span></span>
<span data-ttu-id="895ff-123">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="895ff-123">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="895ff-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="895ff-124">Request headers</span></span>
| <span data-ttu-id="895ff-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="895ff-125">Header</span></span>       | <span data-ttu-id="895ff-126">Значение</span><span class="sxs-lookup"><span data-stu-id="895ff-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="895ff-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="895ff-127">Authorization</span></span>  | <span data-ttu-id="895ff-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="895ff-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="895ff-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="895ff-130">Request body</span></span>
<span data-ttu-id="895ff-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="895ff-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="895ff-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="895ff-132">Response</span></span>
<span data-ttu-id="895ff-133">В случае успешной работы этот метод возвращает код отклика и `200 OK` объект [educationSubmissionResource](../resources/educationsubmissionresource.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="895ff-133">If successful, this method returns a `200 OK` response code and an [educationSubmissionResource](../resources/educationsubmissionresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="895ff-134">Пример</span><span class="sxs-lookup"><span data-stu-id="895ff-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="895ff-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="895ff-135">Request</span></span>
<span data-ttu-id="895ff-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="895ff-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="895ff-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="895ff-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationsubmissionresource"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
# <a name="c"></a>[<span data-ttu-id="895ff-138">C#</span><span class="sxs-lookup"><span data-stu-id="895ff-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationsubmissionresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="895ff-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="895ff-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationsubmissionresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="895ff-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="895ff-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationsubmissionresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="895ff-141">Java</span><span class="sxs-lookup"><span data-stu-id="895ff-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationsubmissionresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="895ff-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="895ff-142">Response</span></span>
<span data-ttu-id="895ff-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="895ff-143">The following is an example of the response.</span></span> 

><span data-ttu-id="895ff-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="895ff-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmissionResource"
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
      "fileUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeTZ_iul5AdW9f/items/017NJZI27BCN2QI2H7HJGLIVPXR6SD2DH6"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get educationSubmissionResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
