---
title: Список educationAssignmentResources
description: Получите все ресурсы, связанные с этим назначением.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: d770d17644462db110be021a541a0dfc28eacf9b
ms.sourcegitcommit: 2006bf01c60793ac6ab1e25fa0526ec5d33c6334
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/23/2021
ms.locfileid: "51961312"
---
# <a name="list-educationassignmentresources"></a><span data-ttu-id="889d8-103">Список educationAssignmentResources</span><span class="sxs-lookup"><span data-stu-id="889d8-103">List educationAssignmentResources</span></span>

<span data-ttu-id="889d8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="889d8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="889d8-105">Получите все ресурсы, связанные с этим назначением.</span><span class="sxs-lookup"><span data-stu-id="889d8-105">Get all the resources associated with this assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="889d8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="889d8-106">Permissions</span></span>
<span data-ttu-id="889d8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="889d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="889d8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="889d8-109">Permission type</span></span>      | <span data-ttu-id="889d8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="889d8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="889d8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="889d8-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="889d8-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="889d8-112">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="889d8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="889d8-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="889d8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="889d8-114">Not supported.</span></span>  |
|<span data-ttu-id="889d8-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="889d8-115">Application</span></span> | <span data-ttu-id="889d8-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="889d8-116">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="889d8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="889d8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/resources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="889d8-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="889d8-118">Optional query parameters</span></span>
<span data-ttu-id="889d8-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="889d8-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="889d8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="889d8-120">Request headers</span></span>
| <span data-ttu-id="889d8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="889d8-121">Header</span></span>       | <span data-ttu-id="889d8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="889d8-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="889d8-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="889d8-123">Authorization</span></span>  | <span data-ttu-id="889d8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="889d8-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="889d8-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="889d8-126">Request body</span></span>
<span data-ttu-id="889d8-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="889d8-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="889d8-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="889d8-128">Response</span></span>
<span data-ttu-id="889d8-129">В случае успешного выполнения этот метод возвращает код ответа и коллекцию объектов `200 OK` [educationAssignmentResource](../resources/educationassignmentresource.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="889d8-129">If successful, this method returns a `200 OK` response code and a collection of [educationAssignmentResource](../resources/educationassignmentresource.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="889d8-130">Пример</span><span class="sxs-lookup"><span data-stu-id="889d8-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="889d8-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="889d8-131">Request</span></span>
<span data-ttu-id="889d8-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="889d8-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="889d8-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="889d8-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_resources_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/11012/assignments/19002/resources
```
# <a name="c"></a>[<span data-ttu-id="889d8-134">C#</span><span class="sxs-lookup"><span data-stu-id="889d8-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-resources-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="889d8-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="889d8-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-resources-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="889d8-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="889d8-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-resources-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="889d8-137">Java</span><span class="sxs-lookup"><span data-stu-id="889d8-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-resources-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="889d8-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="889d8-138">Response</span></span>
<span data-ttu-id="889d8-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="889d8-139">The following is an example of the response.</span></span> 

><span data-ttu-id="889d8-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="889d8-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
