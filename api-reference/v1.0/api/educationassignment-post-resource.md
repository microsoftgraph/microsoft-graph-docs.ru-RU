---
title: Создание educationAssignmentResource
description: Создание ресурса назначения образования.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 2febd840a6ba93f28f38d66d94a2e8f69a526ca2
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992797"
---
# <a name="create-educationassignmentresource"></a><span data-ttu-id="553b9-103">Создание educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="553b9-103">Create educationAssignmentResource</span></span>

<span data-ttu-id="553b9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="553b9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="553b9-105">Создание ресурса [назначения.](../resources/educationassignmentresource.md)</span><span class="sxs-lookup"><span data-stu-id="553b9-105">Create an [assignment resource](../resources/educationassignmentresource.md).</span></span> 

<span data-ttu-id="553b9-106">Каждый ресурс имеет свойство @odata.type, чтобы указать, какой тип ресурса создается.</span><span class="sxs-lookup"><span data-stu-id="553b9-106">Every resource has an @odata.type property to indicate which type of resource is being created.</span></span> 

[!IMPORTANT] 
<span data-ttu-id="553b9-107">Upload файлообъемный ресурс для назначений `resourcesFolder` перед созданием ресурса.</span><span class="sxs-lookup"><span data-stu-id="553b9-107">Upload file-based resource to the assignments `resourcesFolder` before creating the resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="553b9-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="553b9-108">Permissions</span></span>
<span data-ttu-id="553b9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="553b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="553b9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="553b9-111">Permission type</span></span>      | <span data-ttu-id="553b9-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="553b9-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="553b9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="553b9-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="553b9-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="553b9-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="553b9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="553b9-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="553b9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="553b9-116">Not supported.</span></span>  |
|<span data-ttu-id="553b9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="553b9-117">Application</span></span> | <span data-ttu-id="553b9-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="553b9-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="553b9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="553b9-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/resources
```
## <a name="request-headers"></a><span data-ttu-id="553b9-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="553b9-120">Request headers</span></span>
| <span data-ttu-id="553b9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="553b9-121">Header</span></span>       | <span data-ttu-id="553b9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="553b9-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="553b9-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="553b9-123">Authorization</span></span>  | <span data-ttu-id="553b9-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="553b9-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="553b9-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="553b9-126">Content-Type</span></span>  | <span data-ttu-id="553b9-127">application/json</span><span class="sxs-lookup"><span data-stu-id="553b9-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="553b9-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="553b9-128">Request body</span></span>
<span data-ttu-id="553b9-129">В теле запроса поставляют представление JSON объекта [educationAssignmentResource.](../resources/educationassignmentresource.md)</span><span class="sxs-lookup"><span data-stu-id="553b9-129">In the request body, supply a JSON representation of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="553b9-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="553b9-130">Response</span></span>
<span data-ttu-id="553b9-131">В случае успешного выполнения этот метод возвращает код ответа и `201 Created` объект [educationAssignmentResource](../resources/educationassignmentresource.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="553b9-131">If successful, this method returns a `201 Created` response code and an [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="553b9-132">Пример</span><span class="sxs-lookup"><span data-stu-id="553b9-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="553b9-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="553b9-133">Request</span></span>
<span data-ttu-id="553b9-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="553b9-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="553b9-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="553b9-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["ad8afb28-c138-4ad7-b7f5-a6986c2655a8"],
  "name": "create_educationassignmentresource_from_educationassignment"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/resources
Content-type: application/json
Content-length: 212

{
  "distributeForStudentWork": "false",
  "resource": {
    "displayName": "Bing",
    "link": "https://www.bing.com",
    "@odata.type": "educationLinkResource"
  }
}

```
# <a name="c"></a>[<span data-ttu-id="553b9-136">C#</span><span class="sxs-lookup"><span data-stu-id="553b9-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationassignmentresource-from-educationassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="553b9-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="553b9-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationassignmentresource-from-educationassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="553b9-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="553b9-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationassignmentresource-from-educationassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="553b9-139">Java</span><span class="sxs-lookup"><span data-stu-id="553b9-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationassignmentresource-from-educationassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="553b9-140">В теле запроса поставляют представление JSON объекта [educationAssignmentResource.](../resources/educationassignmentresource.md)</span><span class="sxs-lookup"><span data-stu-id="553b9-140">In the request body, supply a JSON representation of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="553b9-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="553b9-141">Response</span></span>
<span data-ttu-id="553b9-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="553b9-142">The following is an example of the response.</span></span> 

><span data-ttu-id="553b9-143">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="553b9-143">**Note:** The response object shown here might be shortened for readability.</span></span>


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentResource"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 229

{
  "id": "122333",
  "distributeForStudentWork": false,
  "resource": {
    "displayName": "Bing",
    "link": "https://www.bing.com",
    "@odata.type": "#microsoft.education.assignments.api.educationLinkResource"
  }
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationAssignmentResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


