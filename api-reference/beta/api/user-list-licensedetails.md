---
title: Перечисление licenseDetails
description: Получение списка объектов licenseDetails.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 48c2a6ce218b5e71fc58d5529f9301ba18265797
ms.sourcegitcommit: 3834b7b0287ee71668c52c42d3465ca19366e678
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2020
ms.locfileid: "43082415"
---
# <a name="list-licensedetails"></a><span data-ttu-id="1b99c-103">Перечисление licenseDetails</span><span class="sxs-lookup"><span data-stu-id="1b99c-103">List licenseDetails</span></span>

<span data-ttu-id="1b99c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b99c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b99c-105">Получение списка объектов **licenseDetails** для корпоративных пользователей.</span><span class="sxs-lookup"><span data-stu-id="1b99c-105">Retrieve a list of **licenseDetails** objects for enterprise users.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b99c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1b99c-106">Permissions</span></span>
<span data-ttu-id="1b99c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b99c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b99c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1b99c-109">Permission type</span></span>      | <span data-ttu-id="1b99c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1b99c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b99c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1b99c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1b99c-112">User. Read, User. Read. ALL, User. ReadWrite. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="1b99c-112">User.Read, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1b99c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1b99c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b99c-114">User.Read</span><span class="sxs-lookup"><span data-stu-id="1b99c-114">User.Read</span></span>    |
|<span data-ttu-id="1b99c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1b99c-115">Application</span></span> | <span data-ttu-id="1b99c-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b99c-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1b99c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1b99c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/licenseDetails
GET /users/{id}/licenseDetails
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1b99c-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1b99c-118">Optional query parameters</span></span>
<span data-ttu-id="1b99c-119">Этот метод **не** поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters).</span><span class="sxs-lookup"><span data-stu-id="1b99c-119">This method does **not** support [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1b99c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1b99c-120">Request headers</span></span>
| <span data-ttu-id="1b99c-121">Имя</span><span class="sxs-lookup"><span data-stu-id="1b99c-121">Name</span></span>      |<span data-ttu-id="1b99c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="1b99c-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1b99c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1b99c-123">Authorization</span></span>  | <span data-ttu-id="1b99c-124">&lt;Код носителя&gt;</span><span class="sxs-lookup"><span data-stu-id="1b99c-124">Bearer &lt;code&gt;</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b99c-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1b99c-125">Request body</span></span>
<span data-ttu-id="1b99c-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1b99c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1b99c-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="1b99c-127">Response</span></span>

<span data-ttu-id="1b99c-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [licenseDetails](../resources/licensedetails.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1b99c-128">If successful, this method returns a `200 OK` response code and collection of [licenseDetails](../resources/licensedetails.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1b99c-129">Пример</span><span class="sxs-lookup"><span data-stu-id="1b99c-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1b99c-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="1b99c-130">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="1b99c-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="1b99c-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_licensedetails"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/licenseDetails
```
# <a name="c"></a>[<span data-ttu-id="1b99c-132">C#</span><span class="sxs-lookup"><span data-stu-id="1b99c-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-licensedetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1b99c-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1b99c-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-licensedetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1b99c-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1b99c-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-licensedetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1b99c-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b99c-135">Response</span></span>
<span data-ttu-id="1b99c-p102">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1b99c-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
