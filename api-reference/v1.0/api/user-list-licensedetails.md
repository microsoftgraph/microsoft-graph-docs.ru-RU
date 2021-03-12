---
title: Перечисление licenseDetails
description: Извлечение списка объектов licenseDetails.
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: c0c4f0cebd430b0087f295a5ae4ecd0b92904512
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50719929"
---
# <a name="list-licensedetails"></a><span data-ttu-id="6a00f-103">Перечисление licenseDetails</span><span class="sxs-lookup"><span data-stu-id="6a00f-103">List licenseDetails</span></span>

<span data-ttu-id="6a00f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a00f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6a00f-105">Извлечение списка **объектов licenseDetails** для корпоративных пользователей.</span><span class="sxs-lookup"><span data-stu-id="6a00f-105">Retrieve a list of **licenseDetails** objects for enterprise users.</span></span>

## <a name="permissions"></a><span data-ttu-id="6a00f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6a00f-106">Permissions</span></span>
<span data-ttu-id="6a00f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a00f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a00f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6a00f-109">Permission type</span></span>      | <span data-ttu-id="6a00f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6a00f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6a00f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6a00f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6a00f-112">User.Read, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6a00f-112">User.Read, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6a00f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6a00f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a00f-114">User.Read</span><span class="sxs-lookup"><span data-stu-id="6a00f-114">User.Read</span></span>    |
|<span data-ttu-id="6a00f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6a00f-115">Application</span></span> | <span data-ttu-id="6a00f-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a00f-116">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6a00f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6a00f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/licenseDetails
GET /users/{id}/licenseDetails
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6a00f-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6a00f-118">Optional query parameters</span></span>
<span data-ttu-id="6a00f-119">Этот метод поддерживает параметр `$select` запроса.</span><span class="sxs-lookup"><span data-stu-id="6a00f-119">This method supports the `$select` query parameter.</span></span> <span data-ttu-id="6a00f-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="6a00f-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6a00f-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6a00f-121">Request headers</span></span>
| <span data-ttu-id="6a00f-122">Имя</span><span class="sxs-lookup"><span data-stu-id="6a00f-122">Name</span></span>      |<span data-ttu-id="6a00f-123">Описание</span><span class="sxs-lookup"><span data-stu-id="6a00f-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6a00f-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6a00f-124">Authorization</span></span>  | <span data-ttu-id="6a00f-125">Код &lt; bearer&gt;</span><span class="sxs-lookup"><span data-stu-id="6a00f-125">Bearer &lt;code&gt;</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a00f-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6a00f-126">Request body</span></span>
<span data-ttu-id="6a00f-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6a00f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a00f-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a00f-128">Response</span></span>

<span data-ttu-id="6a00f-129">В случае успеха этот метод возвращает код отклика и коллекцию `200 OK` [объектов licenseDetails](../resources/licensedetails.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="6a00f-129">If successful, this method returns a `200 OK` response code and collection of [licenseDetails](../resources/licensedetails.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6a00f-130">Пример</span><span class="sxs-lookup"><span data-stu-id="6a00f-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6a00f-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="6a00f-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="6a00f-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="6a00f-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_licensedetails"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/licenseDetails
```
# <a name="c"></a>[<span data-ttu-id="6a00f-133">C#</span><span class="sxs-lookup"><span data-stu-id="6a00f-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-licensedetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6a00f-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6a00f-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-licensedetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6a00f-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6a00f-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-licensedetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6a00f-136">Java</span><span class="sxs-lookup"><span data-stu-id="6a00f-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-licensedetails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6a00f-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a00f-137">Response</span></span>
<span data-ttu-id="6a00f-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6a00f-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

