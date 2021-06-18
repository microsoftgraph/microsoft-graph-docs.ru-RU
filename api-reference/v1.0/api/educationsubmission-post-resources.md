---
title: Создание educationSubmissionResource
description: Добавьте ресурс в список ресурсов отправки.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 7d107b7ceff798875244740ebbe8c7e68322480b
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993415"
---
# <a name="create-educationsubmissionresource"></a><span data-ttu-id="e5202-103">Создание educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="e5202-103">Create educationSubmissionResource</span></span>

<span data-ttu-id="e5202-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5202-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e5202-105">Добавьте ресурс в список ресурсов отправки.</span><span class="sxs-lookup"><span data-stu-id="e5202-105">Add a resource to the submission resource list.</span></span> 

<span data-ttu-id="e5202-106">Это действие может быть сделано только студентом, которому назначено это представление.</span><span class="sxs-lookup"><span data-stu-id="e5202-106">This action can only be done by the student to whom this submission is assigned.</span></span> <span data-ttu-id="e5202-107">Это действие не удастся, если **флаг allowStudentsToAddResources** не `true` установлен.</span><span class="sxs-lookup"><span data-stu-id="e5202-107">This action will not succeed if the **allowStudentsToAddResources** flag isn't set to `true`.</span></span> <span data-ttu-id="e5202-108">Если звонячий хочет создать новый ресурс на основе файлов, файл должен быть загружен в папку ресурсов, связанную с отправкой.</span><span class="sxs-lookup"><span data-stu-id="e5202-108">If the caller wants to create a new file-based resource, the file must be uploaded to the resources folder that is associated with the submission.</span></span> <span data-ttu-id="e5202-109">Если файл не существует или отсутствует в этой папке, запрос POST не будет работать.</span><span class="sxs-lookup"><span data-stu-id="e5202-109">If the file does not exist or isn't in that folder, the POST request will fail.</span></span> 

## <a name="permissions"></a><span data-ttu-id="e5202-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e5202-110">Permissions</span></span>
<span data-ttu-id="e5202-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5202-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5202-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e5202-113">Permission type</span></span>      | <span data-ttu-id="e5202-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e5202-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5202-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e5202-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="e5202-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e5202-116">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="e5202-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e5202-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5202-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5202-118">Not supported.</span></span>  |
|<span data-ttu-id="e5202-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e5202-119">Application</span></span> | <span data-ttu-id="e5202-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5202-120">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e5202-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e5202-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/resources
```

## <a name="request-headers"></a><span data-ttu-id="e5202-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e5202-122">Request headers</span></span>
| <span data-ttu-id="e5202-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e5202-123">Header</span></span>       | <span data-ttu-id="e5202-124">Значение</span><span class="sxs-lookup"><span data-stu-id="e5202-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e5202-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e5202-125">Authorization</span></span>  | <span data-ttu-id="e5202-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e5202-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e5202-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e5202-128">Content-Type</span></span>  | <span data-ttu-id="e5202-129">application/json</span><span class="sxs-lookup"><span data-stu-id="e5202-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e5202-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e5202-130">Request body</span></span>
<span data-ttu-id="e5202-131">В теле запроса поставляют представление JSON объекта [educationSubmissionResource.](../resources/educationsubmissionresource.md)</span><span class="sxs-lookup"><span data-stu-id="e5202-131">In the request body, supply a JSON representation of the [educationSubmissionResource](../resources/educationsubmissionresource.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="e5202-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5202-132">Response</span></span>
<span data-ttu-id="e5202-133">В случае успешной работы этот метод возвращает код отклика и `201 Created` объект [educationSubmissionResource](../resources/educationsubmissionresource.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="e5202-133">If successful, this method returns a `201 Created` response code and an [educationSubmissionResource](../resources/educationsubmissionresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5202-134">Пример</span><span class="sxs-lookup"><span data-stu-id="e5202-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="e5202-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5202-135">Request</span></span>
<span data-ttu-id="e5202-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e5202-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e5202-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="e5202-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationsubmissionresource_from_educationsubmission"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/submissions/fbe51c90-78b7-418a-b5f3-871bf8d8d21e/resources
Content-type: application/json
Content-length: 1097

{
  "assignmentResourceUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeT456457AdW9f/items/017NJZI25NOB5XZNLABF7646XAMDZTQQ6T",
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
  },
  "@odata.type": "microsoft.graph.educationResource"
}
```
# <a name="c"></a>[<span data-ttu-id="e5202-138">C#</span><span class="sxs-lookup"><span data-stu-id="e5202-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationsubmissionresource-from-educationsubmission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e5202-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e5202-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationsubmissionresource-from-educationsubmission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e5202-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e5202-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationsubmissionresource-from-educationsubmission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e5202-141">Java</span><span class="sxs-lookup"><span data-stu-id="e5202-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationsubmissionresource-from-educationsubmission-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e5202-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5202-142">Response</span></span>
<span data-ttu-id="e5202-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e5202-143">The following is an example of the response.</span></span> 

><span data-ttu-id="e5202-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e5202-144">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmissionResource"
} -->
```http
HTTP/1.1 201 Created
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
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationSubmissionResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


