---
title: Отправки списков
description: Список всех отправлений, связанных с назначением.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 86647daa0d19555f53c8f0969cdd831ebd9e7e39
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992763"
---
# <a name="list-submissions"></a><span data-ttu-id="1646c-103">Отправки списков</span><span class="sxs-lookup"><span data-stu-id="1646c-103">List submissions</span></span>

<span data-ttu-id="1646c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1646c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1646c-105">Список всех отправлений, связанных с назначением.</span><span class="sxs-lookup"><span data-stu-id="1646c-105">List all the submissions associated with an assignment.</span></span> 

<span data-ttu-id="1646c-106">Учитель или приложение с разрешениями на приложения могут получать все материалы, в то время как студент может получать только те материалы, с которые они связаны.</span><span class="sxs-lookup"><span data-stu-id="1646c-106">A teacher or an application with application permissions can get all the submissions while a student can only get submissions that they are associated with.</span></span>

## <a name="permissions"></a><span data-ttu-id="1646c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1646c-107">Permissions</span></span>
<span data-ttu-id="1646c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1646c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1646c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1646c-110">Permission type</span></span>      | <span data-ttu-id="1646c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1646c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1646c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1646c-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="1646c-113">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1646c-113">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="1646c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1646c-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="1646c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1646c-115">Not supported.</span></span>  |
|<span data-ttu-id="1646c-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="1646c-116">Application</span></span> | <span data-ttu-id="1646c-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1646c-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="1646c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1646c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1646c-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1646c-119">Optional query parameters</span></span>
<span data-ttu-id="1646c-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1646c-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1646c-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1646c-121">Request headers</span></span>
| <span data-ttu-id="1646c-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1646c-122">Header</span></span>       | <span data-ttu-id="1646c-123">Значение</span><span class="sxs-lookup"><span data-stu-id="1646c-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1646c-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1646c-124">Authorization</span></span>  | <span data-ttu-id="1646c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1646c-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1646c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1646c-127">Request body</span></span>
<span data-ttu-id="1646c-128">Не поставляем тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1646c-128">Don't supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="1646c-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="1646c-129">Response</span></span>
<span data-ttu-id="1646c-130">В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` объектов [educationSubmission](../resources/educationsubmission.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1646c-130">If successful, this method returns a `200 OK` response code and collection of [educationSubmission](../resources/educationsubmission.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1646c-131">Пример</span><span class="sxs-lookup"><span data-stu-id="1646c-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="1646c-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="1646c-132">Request</span></span>
<span data-ttu-id="1646c-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1646c-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1646c-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="1646c-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["ad8afb28-c138-4ad7-b7f5-a6986c2655a8"],
  "name": "get_submissions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/submissions
```
# <a name="c"></a>[<span data-ttu-id="1646c-135">C#</span><span class="sxs-lookup"><span data-stu-id="1646c-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-submissions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1646c-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1646c-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-submissions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1646c-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1646c-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-submissions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1646c-138">Java</span><span class="sxs-lookup"><span data-stu-id="1646c-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-submissions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1646c-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="1646c-139">Response</span></span>
<span data-ttu-id="1646c-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1646c-140">The following is an example of the response.</span></span> 

><span data-ttu-id="1646c-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1646c-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmission",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 873

{
  "value": [
    {
      "id": "33223",
      "recipient": {
        "userId": "13015",
        "@Odata.type":"microsoft.graph.educationSubmissionRecipient"
      },
      "releasedBy": {
          "user": {
            "displayName": "Shawn Hughes",
            "id": "14012"
          },
        },
      "releasedDateTime": "2014-01-01T00:00:00Z",
      "resourcesFolderUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeT456457AdW9f/items/017NJZI25NOB5XZNLABF7646XAMDZTQQ6T",
      "status": "working",
      "submittedBy": {
          "user": {
            "displayName": "Shawn Hughes",
            "id": "14012"
          },
        },
      "submittedDateTime": "2014-01-01T00:00:00Z"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List submissions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
