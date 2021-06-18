---
title: Перечисление ресурсов задания
description: Получите все ресурсы, связанные с этим назначением.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: f94f1bb5f0aec7a55685a42296f0d5184c58cd1a
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992174"
---
# <a name="list-assignment-resources"></a><span data-ttu-id="cb1bf-103">Перечисление ресурсов задания</span><span class="sxs-lookup"><span data-stu-id="cb1bf-103">List assignment resources</span></span>

<span data-ttu-id="cb1bf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb1bf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cb1bf-105">Получите все ресурсы, связанные с [назначением.](../resources/educationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="cb1bf-105">Get all the resources associated with an [assignment](../resources/educationassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cb1bf-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cb1bf-106">Permissions</span></span>
<span data-ttu-id="cb1bf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb1bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb1bf-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cb1bf-109">Permission type</span></span>      | <span data-ttu-id="cb1bf-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cb1bf-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cb1bf-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cb1bf-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="cb1bf-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cb1bf-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="cb1bf-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cb1bf-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="cb1bf-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb1bf-114">Not supported.</span></span>  |
|<span data-ttu-id="cb1bf-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="cb1bf-115">Application</span></span> | <span data-ttu-id="cb1bf-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cb1bf-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="cb1bf-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cb1bf-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/resources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cb1bf-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cb1bf-118">Optional query parameters</span></span>
<span data-ttu-id="cb1bf-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="cb1bf-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cb1bf-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cb1bf-120">Request headers</span></span>
| <span data-ttu-id="cb1bf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cb1bf-121">Header</span></span>       | <span data-ttu-id="cb1bf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cb1bf-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cb1bf-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cb1bf-123">Authorization</span></span>  | <span data-ttu-id="cb1bf-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cb1bf-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cb1bf-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cb1bf-126">Request body</span></span>
<span data-ttu-id="cb1bf-127">Не поставляем тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cb1bf-127">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb1bf-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb1bf-128">Response</span></span>
<span data-ttu-id="cb1bf-129">В случае успешного выполнения этот метод возвращает код ответа и коллекцию объектов `200 OK` [educationAssignmentResource](../resources/educationassignmentresource.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="cb1bf-129">If successful, this method returns a `200 OK` response code and a collection of [educationAssignmentResource](../resources/educationassignmentresource.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb1bf-130">Пример</span><span class="sxs-lookup"><span data-stu-id="cb1bf-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="cb1bf-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="cb1bf-131">Request</span></span>
<span data-ttu-id="cb1bf-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cb1bf-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="cb1bf-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="cb1bf-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["ad8afb28-c138-4ad7-b7f5-a6986c2655a8"],
  "name": "get_resources_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/d38ffdea-da93-46ac-90ba-d568c6073075/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/resources
```
# <a name="c"></a>[<span data-ttu-id="cb1bf-134">C#</span><span class="sxs-lookup"><span data-stu-id="cb1bf-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-resources-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cb1bf-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cb1bf-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-resources-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cb1bf-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cb1bf-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-resources-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cb1bf-137">Java</span><span class="sxs-lookup"><span data-stu-id="cb1bf-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-resources-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cb1bf-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb1bf-138">Response</span></span>
<span data-ttu-id="cb1bf-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="cb1bf-139">The following is an example of the response.</span></span> 

><span data-ttu-id="cb1bf-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="cb1bf-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentResource",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1011

{
  "value": [
    {
      "distributeForStudentWork": false,
      "resource": {
          "@odata.type": "#microsoft.graph.educationLinkResource",
          "displayName": "Microsoft Homepage",
          "createdDateTime": "2017-10-21T07:52:45.5675913Z",
          "createdBy": {
              "application": null,
              "device": null,
              "user": {
                  "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
                  "displayName": null
              }
          },
          "lastModifiedDateTime": "2017-10-21T07:52:45.5675913Z",
          "lastModifiedBy": {
              "application": null,
              "device": null,
              "user": {
                  "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
                  "displayName": null
              }
          },
          "link": "https://www.microsoft.com"
      },
      "id": "850f51b7-1df9-4ec0-bd62-64a0214b9cbf"
    },
    {
      "distributeForStudentWork": true,
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
      "id": "f2387c3b-ec39-4bf2-a399-d7242677f024"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List resources",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
