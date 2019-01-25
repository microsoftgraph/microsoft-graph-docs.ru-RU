---
title: Перечисление licenseDetails
description: Получение списка объектов licenseDetails.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7dae02120f17dfbd329758734ba5fb912adfe0e6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515946"
---
# <a name="list-licensedetails"></a><span data-ttu-id="fd019-103">Перечисление licenseDetails</span><span class="sxs-lookup"><span data-stu-id="fd019-103">List licenseDetails</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd019-104">Получение списка объектов licenseDetails.</span><span class="sxs-lookup"><span data-stu-id="fd019-104">Retrieve a list of licenseDetails objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="fd019-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fd019-105">Permissions</span></span>
<span data-ttu-id="fd019-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd019-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd019-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fd019-108">Permission type</span></span>      | <span data-ttu-id="fd019-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fd019-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd019-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fd019-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fd019-111">User.Read, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fd019-111">User.Read, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fd019-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fd019-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd019-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="fd019-113">User.Read</span></span>    |
|<span data-ttu-id="fd019-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fd019-114">Application</span></span> | <span data-ttu-id="fd019-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd019-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fd019-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fd019-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/licenseDetails
GET /users/{id}/licenseDetails
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fd019-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="fd019-117">Optional query parameters</span></span>
<span data-ttu-id="fd019-118">Этот метод **не** поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="fd019-118">This method does **not** support [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="fd019-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fd019-119">Request headers</span></span>
| <span data-ttu-id="fd019-120">Имя</span><span class="sxs-lookup"><span data-stu-id="fd019-120">Name</span></span>      |<span data-ttu-id="fd019-121">Описание</span><span class="sxs-lookup"><span data-stu-id="fd019-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fd019-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd019-122">Authorization</span></span>  | <span data-ttu-id="fd019-123">Bearer &lt;code&gt;</span><span class="sxs-lookup"><span data-stu-id="fd019-123">Bearer &lt;code&gt;</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd019-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fd019-124">Request body</span></span>
<span data-ttu-id="fd019-125">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fd019-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fd019-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd019-126">Response</span></span>

<span data-ttu-id="fd019-127">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [licenseDetails](../resources/licensedetails.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fd019-127">If successful, this method returns a `200 OK` response code and collection of [licenseDetails](../resources/licensedetails.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fd019-128">Пример</span><span class="sxs-lookup"><span data-stu-id="fd019-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fd019-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="fd019-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_licensedetails"
}-->
```http
GET https://graph.microsoft.com/beta/me/licenseDetails
```
##### <a name="response"></a><span data-ttu-id="fd019-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="fd019-130">Response</span></span>
<span data-ttu-id="fd019-p102">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fd019-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.licenseDetails",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 389

{
  "value": [
    {
      "servicePlans": [
        {
          "servicePlanId": "servicePlanId-value",
          "servicePlanName": "servicePlanName-value",
          "provisioningStatus": "provisioningStatus-value",
          "appliesTo": "appliesTo-value"
        }
      ],
      "skuId": "skuId-value",
      "skuPartNumber": "skuPartNumber-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List licenseDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-licensedetails.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
