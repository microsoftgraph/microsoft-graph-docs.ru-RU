---
title: Список educationAssignmentResources
description: Получите все ресурсы, связанные с этим назначением.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 5556210604ce6b0c273a0e4d89e1a792d2639b12
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518571"
---
# <a name="list-educationassignmentresources"></a><span data-ttu-id="9df5a-103">Список educationAssignmentResources</span><span class="sxs-lookup"><span data-stu-id="9df5a-103">List educationAssignmentResources</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9df5a-104">Получите все ресурсы, связанные с этим назначением.</span><span class="sxs-lookup"><span data-stu-id="9df5a-104">Get all the resources associated with this assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="9df5a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9df5a-105">Permissions</span></span>
<span data-ttu-id="9df5a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9df5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9df5a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9df5a-108">Permission type</span></span>      | <span data-ttu-id="9df5a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9df5a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9df5a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9df5a-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="9df5a-111">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9df5a-111">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="9df5a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9df5a-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="9df5a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9df5a-113">Not supported.</span></span>  |
|<span data-ttu-id="9df5a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9df5a-114">Application</span></span> | <span data-ttu-id="9df5a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9df5a-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="9df5a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9df5a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/resources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9df5a-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9df5a-117">Optional query parameters</span></span>
<span data-ttu-id="9df5a-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9df5a-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9df5a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9df5a-119">Request headers</span></span>
| <span data-ttu-id="9df5a-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9df5a-120">Header</span></span>       | <span data-ttu-id="9df5a-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9df5a-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9df5a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9df5a-122">Authorization</span></span>  | <span data-ttu-id="9df5a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9df5a-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9df5a-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9df5a-125">Request body</span></span>
<span data-ttu-id="9df5a-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9df5a-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="9df5a-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="9df5a-127">Response</span></span>
<span data-ttu-id="9df5a-128">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [educationAssignmentResource](../resources/educationassignmentresource.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="9df5a-128">If successful, this method returns a `200 OK` response code and a collection of [educationAssignmentResource](../resources/educationassignmentresource.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9df5a-129">Пример</span><span class="sxs-lookup"><span data-stu-id="9df5a-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9df5a-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="9df5a-130">Request</span></span>
<span data-ttu-id="9df5a-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9df5a-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_resources"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11012/assignments/19002/resources
```
##### <a name="response"></a><span data-ttu-id="9df5a-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="9df5a-132">Response</span></span>
<span data-ttu-id="9df5a-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9df5a-133">The following is an example of the response.</span></span> 

><span data-ttu-id="9df5a-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9df5a-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
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
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignment-list-resources.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
