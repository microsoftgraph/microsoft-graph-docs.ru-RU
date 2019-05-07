---
title: Перечисление licenseDetails
description: Получение списка объектов licenseDetails.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b51b129977a2923646ec93479c0d8b888db2369e
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33601855"
---
# <a name="list-licensedetails"></a><span data-ttu-id="82846-103">Перечисление licenseDetails</span><span class="sxs-lookup"><span data-stu-id="82846-103">List licenseDetails</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82846-104">Получение списка объектов licenseDetails.</span><span class="sxs-lookup"><span data-stu-id="82846-104">Retrieve a list of licenseDetails objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="82846-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="82846-105">Permissions</span></span>
<span data-ttu-id="82846-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82846-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82846-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="82846-108">Permission type</span></span>      | <span data-ttu-id="82846-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="82846-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="82846-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="82846-110">Delegated (work or school account)</span></span> | <span data-ttu-id="82846-111">User. Read, User. Read. ALL, User. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="82846-111">User.Read, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="82846-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="82846-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82846-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="82846-113">User.Read</span></span>    |
|<span data-ttu-id="82846-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="82846-114">Application</span></span> | <span data-ttu-id="82846-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82846-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="82846-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="82846-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/licenseDetails
GET /users/{id}/licenseDetails
```
## <a name="optional-query-parameters"></a><span data-ttu-id="82846-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="82846-117">Optional query parameters</span></span>
<span data-ttu-id="82846-118">Этот метод **не** поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="82846-118">This method does **not** support [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="82846-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="82846-119">Request headers</span></span>
| <span data-ttu-id="82846-120">Имя</span><span class="sxs-lookup"><span data-stu-id="82846-120">Name</span></span>      |<span data-ttu-id="82846-121">Описание</span><span class="sxs-lookup"><span data-stu-id="82846-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="82846-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="82846-122">Authorization</span></span>  | <span data-ttu-id="82846-123">&lt;Код носителя&gt;</span><span class="sxs-lookup"><span data-stu-id="82846-123">Bearer &lt;code&gt;</span></span>|

## <a name="request-body"></a><span data-ttu-id="82846-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="82846-124">Request body</span></span>
<span data-ttu-id="82846-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="82846-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="82846-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="82846-126">Response</span></span>

<span data-ttu-id="82846-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [licenseDetails](../resources/licensedetails.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="82846-127">If successful, this method returns a `200 OK` response code and collection of [licenseDetails](../resources/licensedetails.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="82846-128">Пример</span><span class="sxs-lookup"><span data-stu-id="82846-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="82846-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="82846-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_licensedetails"
}-->
```http
GET https://graph.microsoft.com/beta/me/licenseDetails
```
##### <a name="response"></a><span data-ttu-id="82846-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="82846-130">Response</span></span>
<span data-ttu-id="82846-p102">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="82846-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="82846-133">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="82846-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="82846-134">Языках</span><span class="sxs-lookup"><span data-stu-id="82846-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_licensedetails-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="82846-135">Язык</span><span class="sxs-lookup"><span data-stu-id="82846-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_licensedetails-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/user-list-licensedetails.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-list-licensedetails.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
