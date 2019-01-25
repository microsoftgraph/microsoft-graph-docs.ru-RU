---
title: Получение educationAssignmentResource
description: 'Получение свойств определенного ресурса по назначению.  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 76d9ed55c4e914385ad6282e3bed6025ef5c6036
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526195"
---
# <a name="get-educationassignmentresource"></a><span data-ttu-id="c1068-103">Получение educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="c1068-103">Get educationAssignmentResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1068-104">Получение свойств определенного ресурса по назначению.</span><span class="sxs-lookup"><span data-stu-id="c1068-104">Get the properties of a specific resource on an assignment.</span></span>  
## <a name="permissions"></a><span data-ttu-id="c1068-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c1068-105">Permissions</span></span>
<span data-ttu-id="c1068-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c1068-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1068-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c1068-108">Permission type</span></span>      | <span data-ttu-id="c1068-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c1068-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c1068-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c1068-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c1068-111">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c1068-111">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="c1068-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c1068-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c1068-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1068-113">Not supported.</span></span>  |
|<span data-ttu-id="c1068-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c1068-114">Application</span></span> |  <span data-ttu-id="c1068-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1068-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c1068-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c1068-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/resources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c1068-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c1068-117">Optional query parameters</span></span>
<span data-ttu-id="c1068-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c1068-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c1068-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c1068-119">Request headers</span></span>
| <span data-ttu-id="c1068-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c1068-120">Header</span></span>       | <span data-ttu-id="c1068-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c1068-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c1068-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c1068-122">Authorization</span></span>  | <span data-ttu-id="c1068-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c1068-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c1068-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c1068-125">Request body</span></span>
<span data-ttu-id="c1068-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c1068-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c1068-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="c1068-127">Response</span></span>
<span data-ttu-id="c1068-128">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [educationAssignmentResource](../resources/educationassignmentresource.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c1068-128">If successful, this method returns a `200 OK` response code and an [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c1068-129">Пример</span><span class="sxs-lookup"><span data-stu-id="c1068-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c1068-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="c1068-130">Request</span></span>
<span data-ttu-id="c1068-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c1068-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationassignmentresource"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources/22002
```
##### <a name="response"></a><span data-ttu-id="c1068-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="c1068-132">Response</span></span>
<span data-ttu-id="c1068-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c1068-133">The following is an example of the response.</span></span> 

><span data-ttu-id="c1068-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c1068-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c1068-135">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c1068-135">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentResource"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 842

{
  "distributeForStudentWork": true,
  "id": "22002",
  "resource": {
    "createdBy": {
      "user": {
        "displayName": "Susana Rocha",
        "id": "14012"
      },
    },
    "createdDateTime": "2014-01-01T00:00:00Z",
    "displayName": "Excel workbook 1",
    "lastModifiedBy": {
      "user": {
        "displayName": "Susana Rocha",
        "id": "14012"
      },
    },
    "lastModifiedDateTime": "2014-01-01T00:00:00Z"
  }
}
    
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get educationAssignmentResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignmentresource-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
