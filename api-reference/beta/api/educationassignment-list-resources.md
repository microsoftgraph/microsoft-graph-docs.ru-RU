---
title: Список Едукатионассигнментресаурцес
description: Получение всех ресурсов, связанных с этим назначением.
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 2ba4ba24168e6186fd61d58320763f8361d569f0
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324752"
---
# <a name="list-educationassignmentresources"></a><span data-ttu-id="de4a6-103">Список Едукатионассигнментресаурцес</span><span class="sxs-lookup"><span data-stu-id="de4a6-103">List educationAssignmentResources</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de4a6-104">Получение всех ресурсов, связанных с этим назначением.</span><span class="sxs-lookup"><span data-stu-id="de4a6-104">Get all the resources associated with this assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="de4a6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="de4a6-105">Permissions</span></span>
<span data-ttu-id="de4a6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de4a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de4a6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="de4a6-108">Permission type</span></span>      | <span data-ttu-id="de4a6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="de4a6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="de4a6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de4a6-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="de4a6-111">EduAssignments. ReadBasic, EduAssignments. Реадвритебасик, EduAssignments. Read, EduAssignments. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="de4a6-111">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="de4a6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de4a6-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="de4a6-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de4a6-113">Not supported.</span></span>  |
|<span data-ttu-id="de4a6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="de4a6-114">Application</span></span> | <span data-ttu-id="de4a6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de4a6-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="de4a6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="de4a6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/resources
```
## <a name="optional-query-parameters"></a><span data-ttu-id="de4a6-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="de4a6-117">Optional query parameters</span></span>
<span data-ttu-id="de4a6-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="de4a6-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="de4a6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="de4a6-119">Request headers</span></span>
| <span data-ttu-id="de4a6-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="de4a6-120">Header</span></span>       | <span data-ttu-id="de4a6-121">Значение</span><span class="sxs-lookup"><span data-stu-id="de4a6-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="de4a6-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="de4a6-122">Authorization</span></span>  | <span data-ttu-id="de4a6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="de4a6-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="de4a6-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="de4a6-125">Request body</span></span>
<span data-ttu-id="de4a6-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="de4a6-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="de4a6-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="de4a6-127">Response</span></span>
<span data-ttu-id="de4a6-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [едукатионассигнментресаурце](../resources/educationassignmentresource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="de4a6-128">If successful, this method returns a `200 OK` response code and a collection of [educationAssignmentResource](../resources/educationassignmentresource.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="de4a6-129">Пример</span><span class="sxs-lookup"><span data-stu-id="de4a6-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="de4a6-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="de4a6-130">Request</span></span>
<span data-ttu-id="de4a6-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="de4a6-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_resources"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11012/assignments/19002/resources
```
##### <a name="response"></a><span data-ttu-id="de4a6-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="de4a6-132">Response</span></span>
<span data-ttu-id="de4a6-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="de4a6-133">The following is an example of the response.</span></span> 

><span data-ttu-id="de4a6-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="de4a6-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "suppressions": []
}
-->
