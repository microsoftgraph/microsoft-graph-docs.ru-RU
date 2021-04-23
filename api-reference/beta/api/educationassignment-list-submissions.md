---
title: Отправки списков
description: Список всех представлений, связанных с этим назначением. Учитель или приложение с разрешениями на приложения могут получать все материалы, в то время как студент может получать только те материалы, с которые они связаны.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: c27472d82521c1972b468ebef7925e194efbae7f
ms.sourcegitcommit: 2006bf01c60793ac6ab1e25fa0526ec5d33c6334
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/23/2021
ms.locfileid: "51961291"
---
# <a name="list-submissions"></a><span data-ttu-id="59ba0-104">Отправки списков</span><span class="sxs-lookup"><span data-stu-id="59ba0-104">List submissions</span></span>

<span data-ttu-id="59ba0-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59ba0-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59ba0-106">Список всех представлений, связанных с этим назначением.</span><span class="sxs-lookup"><span data-stu-id="59ba0-106">List all the submissions associated with this assignment.</span></span> <span data-ttu-id="59ba0-107">Учитель или приложение с разрешениями на приложения могут получать все материалы, в то время как студент может получать только те материалы, с которые они связаны.</span><span class="sxs-lookup"><span data-stu-id="59ba0-107">A teacher or an application with application permissions can get all the submissions while a student can only get submissions that they are associated with.</span></span>

## <a name="permissions"></a><span data-ttu-id="59ba0-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="59ba0-108">Permissions</span></span>
<span data-ttu-id="59ba0-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59ba0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59ba0-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="59ba0-111">Permission type</span></span>      | <span data-ttu-id="59ba0-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="59ba0-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59ba0-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="59ba0-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="59ba0-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59ba0-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="59ba0-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="59ba0-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="59ba0-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="59ba0-116">Not supported.</span></span>  |
|<span data-ttu-id="59ba0-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="59ba0-117">Application</span></span> | <span data-ttu-id="59ba0-118">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59ba0-118">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="59ba0-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="59ba0-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions
```
## <a name="optional-query-parameters"></a><span data-ttu-id="59ba0-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="59ba0-120">Optional query parameters</span></span>
<span data-ttu-id="59ba0-121">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="59ba0-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="59ba0-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="59ba0-122">Request headers</span></span>
| <span data-ttu-id="59ba0-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="59ba0-123">Header</span></span>       | <span data-ttu-id="59ba0-124">Значение</span><span class="sxs-lookup"><span data-stu-id="59ba0-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="59ba0-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="59ba0-125">Authorization</span></span>  | <span data-ttu-id="59ba0-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="59ba0-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="59ba0-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="59ba0-128">Request body</span></span>
<span data-ttu-id="59ba0-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="59ba0-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="59ba0-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="59ba0-130">Response</span></span>
<span data-ttu-id="59ba0-131">В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` объектов [educationSubmission](../resources/educationsubmission.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="59ba0-131">If successful, this method returns a `200 OK` response code and collection of [educationSubmission](../resources/educationsubmission.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="59ba0-132">Пример</span><span class="sxs-lookup"><span data-stu-id="59ba0-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="59ba0-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="59ba0-133">Request</span></span>
<span data-ttu-id="59ba0-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="59ba0-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="59ba0-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="59ba0-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_submissions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions
```
# <a name="c"></a>[<span data-ttu-id="59ba0-136">C#</span><span class="sxs-lookup"><span data-stu-id="59ba0-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-submissions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="59ba0-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="59ba0-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-submissions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="59ba0-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="59ba0-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-submissions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="59ba0-139">Java</span><span class="sxs-lookup"><span data-stu-id="59ba0-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-submissions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="59ba0-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="59ba0-140">Response</span></span>
<span data-ttu-id="59ba0-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="59ba0-141">The following is an example of the response.</span></span> 

><span data-ttu-id="59ba0-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="59ba0-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="59ba0-143">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="59ba0-143">All of the properties will be returned from an actual call.</span></span>

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
            "displayName": "Susana Rocha",
            "id": "14012"
          },
        },
      "releasedDateTime": "2014-01-01T00:00:00Z",
      "resourcesFolderUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeT456457AdW9f/items/017NJZI25NOB5XZNLABF7646XAMDZTQQ6T",
      "status": "working",
      "submittedBy": {
          "user": {
            "displayName": "Susana Rocha",
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
