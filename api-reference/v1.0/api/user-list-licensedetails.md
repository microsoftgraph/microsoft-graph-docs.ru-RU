---
title: Перечисление licenseDetails
description: Получение списка объектов licenseDetails.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a2fd268bbc920b3c1a6ef3dc79f5295ff66c2eb1
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36727483"
---
# <a name="list-licensedetails"></a><span data-ttu-id="77ac3-103">Перечисление licenseDetails</span><span class="sxs-lookup"><span data-stu-id="77ac3-103">List licenseDetails</span></span>

<span data-ttu-id="77ac3-104">Получение списка объектов licenseDetails.</span><span class="sxs-lookup"><span data-stu-id="77ac3-104">Retrieve a list of licenseDetails objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="77ac3-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="77ac3-105">Permissions</span></span>
<span data-ttu-id="77ac3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77ac3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77ac3-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="77ac3-108">Permission type</span></span>      | <span data-ttu-id="77ac3-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="77ac3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="77ac3-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="77ac3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="77ac3-111">User. Read, User. Read. ALL, User. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="77ac3-111">User.Read, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="77ac3-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="77ac3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77ac3-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="77ac3-113">User.Read</span></span>    |
|<span data-ttu-id="77ac3-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="77ac3-114">Application</span></span> | <span data-ttu-id="77ac3-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77ac3-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="77ac3-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="77ac3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/licenseDetails
GET /users/{id}/licenseDetails
```
## <a name="optional-query-parameters"></a><span data-ttu-id="77ac3-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="77ac3-117">Optional query parameters</span></span>
<span data-ttu-id="77ac3-118">Этот метод **не** поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="77ac3-118">This method does **not** support [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="77ac3-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="77ac3-119">Request headers</span></span>
| <span data-ttu-id="77ac3-120">Имя</span><span class="sxs-lookup"><span data-stu-id="77ac3-120">Name</span></span>      |<span data-ttu-id="77ac3-121">Описание</span><span class="sxs-lookup"><span data-stu-id="77ac3-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="77ac3-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="77ac3-122">Authorization</span></span>  | <span data-ttu-id="77ac3-123">&lt;Код носителя&gt;</span><span class="sxs-lookup"><span data-stu-id="77ac3-123">Bearer &lt;code&gt;</span></span>|

## <a name="request-body"></a><span data-ttu-id="77ac3-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="77ac3-124">Request body</span></span>
<span data-ttu-id="77ac3-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="77ac3-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77ac3-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="77ac3-126">Response</span></span>

<span data-ttu-id="77ac3-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [licenseDetails](../resources/licensedetails.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="77ac3-127">If successful, this method returns a `200 OK` response code and collection of [licenseDetails](../resources/licensedetails.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="77ac3-128">Пример</span><span class="sxs-lookup"><span data-stu-id="77ac3-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="77ac3-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="77ac3-129">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="77ac3-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="77ac3-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_licensedetails"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/licenseDetails
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="77ac3-131">C#</span><span class="sxs-lookup"><span data-stu-id="77ac3-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-licensedetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="77ac3-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="77ac3-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-licensedetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="77ac3-133">Цель — C</span><span class="sxs-lookup"><span data-stu-id="77ac3-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-licensedetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="77ac3-134">Java</span><span class="sxs-lookup"><span data-stu-id="77ac3-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-licensedetails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="77ac3-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="77ac3-135">Response</span></span>
<span data-ttu-id="77ac3-p102">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="77ac3-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List licenseDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
