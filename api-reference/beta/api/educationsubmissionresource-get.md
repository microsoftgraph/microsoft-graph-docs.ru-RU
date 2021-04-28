---
title: Get educationSubmissionResource
description: Извлекает свойства определенного ресурса, связанного с отправкой. Этот ресурс находится в "рабочем" списке ресурсов и должен рассматриваться студентом в процессе работы. Этот ресурс завернут с помощью возможного указателя обратно в ресурс назначения, если он был скопирован из назначения.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 31df23948009f8724b1bf08a8608fc9ae0b316be
ms.sourcegitcommit: eb67b0a619a4004c1611304f1252a382264a97f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52061863"
---
# <a name="get-educationsubmissionresource"></a><span data-ttu-id="da149-105">Get educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="da149-105">Get educationSubmissionResource</span></span>

<span data-ttu-id="da149-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da149-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da149-107">Извлекает свойства определенного ресурса, связанного с отправкой.</span><span class="sxs-lookup"><span data-stu-id="da149-107">Retrieves the properties of a specific resource associated with the submission.</span></span> <span data-ttu-id="da149-108">Этот ресурс находится в "рабочем" списке ресурсов и должен рассматриваться студентом в процессе работы.</span><span class="sxs-lookup"><span data-stu-id="da149-108">This resource is in the "working" resource list and should be considered work in process by a student.</span></span> <span data-ttu-id="da149-109">Этот ресурс завернут с помощью возможного указателя обратно в ресурс назначения, если он был скопирован из назначения.</span><span class="sxs-lookup"><span data-stu-id="da149-109">This resource is wrapped with a possible pointer back to the assignment resource if it was copied from the assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="da149-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="da149-110">Permissions</span></span>
<span data-ttu-id="da149-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da149-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da149-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="da149-113">Permission type</span></span>      | <span data-ttu-id="da149-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="da149-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da149-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="da149-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="da149-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="da149-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="da149-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="da149-117">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="da149-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da149-118">Not supported.</span></span>  |
|<span data-ttu-id="da149-119">Приложение\*</span><span class="sxs-lookup"><span data-stu-id="da149-119">Application\*</span></span> | <span data-ttu-id="da149-120">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="da149-120">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

<span data-ttu-id="da149-121">\*Разрешения приложения в настоящее время доступны только для частных пользователей предварительного просмотра.</span><span class="sxs-lookup"><span data-stu-id="da149-121">\*Application permissions are currently available to private preview customers only.</span></span>

## <a name="http-request"></a><span data-ttu-id="da149-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="da149-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/resources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="da149-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="da149-123">Optional query parameters</span></span>
<span data-ttu-id="da149-124">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="da149-124">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="da149-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="da149-125">Request headers</span></span>
| <span data-ttu-id="da149-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="da149-126">Header</span></span>       | <span data-ttu-id="da149-127">Значение</span><span class="sxs-lookup"><span data-stu-id="da149-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="da149-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="da149-128">Authorization</span></span>  | <span data-ttu-id="da149-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="da149-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="da149-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="da149-131">Request body</span></span>
<span data-ttu-id="da149-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="da149-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="da149-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="da149-133">Response</span></span>
<span data-ttu-id="da149-134">В случае успешной работы этот метод возвращает код отклика и `200 OK` объект [educationSubmissionResource](../resources/educationsubmissionresource.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="da149-134">If successful, this method returns a `200 OK` response code and an [educationSubmissionResource](../resources/educationsubmissionresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="da149-135">Пример</span><span class="sxs-lookup"><span data-stu-id="da149-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="da149-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="da149-136">Request</span></span>
<span data-ttu-id="da149-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="da149-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="da149-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="da149-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationsubmissionresource"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
# <a name="c"></a>[<span data-ttu-id="da149-139">C#</span><span class="sxs-lookup"><span data-stu-id="da149-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationsubmissionresource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="da149-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="da149-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationsubmissionresource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="da149-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="da149-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationsubmissionresource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="da149-142">Java</span><span class="sxs-lookup"><span data-stu-id="da149-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationsubmissionresource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="da149-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="da149-143">Response</span></span>
<span data-ttu-id="da149-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="da149-144">The following is an example of the response.</span></span> 

><span data-ttu-id="da149-145">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="da149-145">**Note:** The response object shown here might be shortened for readability.</span></span>

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
