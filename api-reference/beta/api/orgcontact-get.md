---
title: Получение orgContact
description: Получение свойств и связей объекта orgcontact.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9bf4704135dcc66cb38281f131abbe9bbc51110c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35877945"
---
# <a name="get-orgcontact"></a><span data-ttu-id="66b07-103">Получение orgContact</span><span class="sxs-lookup"><span data-stu-id="66b07-103">Get orgContact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66b07-104">Получение свойств и связей объекта orgcontact.</span><span class="sxs-lookup"><span data-stu-id="66b07-104">Retrieve the properties and relationships of orgcontact object.</span></span>
## <a name="permissions"></a><span data-ttu-id="66b07-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="66b07-105">Permissions</span></span>
<span data-ttu-id="66b07-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66b07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66b07-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="66b07-108">Permission type</span></span>      | <span data-ttu-id="66b07-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="66b07-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66b07-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="66b07-110">Delegated (work or school account)</span></span> | <span data-ttu-id="66b07-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="66b07-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="66b07-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="66b07-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66b07-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66b07-113">Not supported.</span></span>    |
|<span data-ttu-id="66b07-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="66b07-114">Application</span></span> | <span data-ttu-id="66b07-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66b07-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="66b07-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="66b07-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="66b07-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="66b07-117">Optional query parameters</span></span>
<span data-ttu-id="66b07-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="66b07-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="66b07-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="66b07-119">Request headers</span></span>
| <span data-ttu-id="66b07-120">Имя</span><span class="sxs-lookup"><span data-stu-id="66b07-120">Name</span></span>       | <span data-ttu-id="66b07-121">Тип</span><span class="sxs-lookup"><span data-stu-id="66b07-121">Type</span></span> | <span data-ttu-id="66b07-122">Описание</span><span class="sxs-lookup"><span data-stu-id="66b07-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="66b07-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="66b07-123">Authorization</span></span>  | <span data-ttu-id="66b07-124">string</span><span class="sxs-lookup"><span data-stu-id="66b07-124">string</span></span>  | <span data-ttu-id="66b07-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="66b07-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="66b07-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="66b07-127">Request body</span></span>
<span data-ttu-id="66b07-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="66b07-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66b07-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="66b07-129">Response</span></span>

<span data-ttu-id="66b07-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [orgContact](../resources/orgcontact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="66b07-130">If successful, this method returns a `200 OK` response code and [orgContact](../resources/orgcontact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="66b07-131">Пример</span><span class="sxs-lookup"><span data-stu-id="66b07-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="66b07-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="66b07-132">Request</span></span>
<span data-ttu-id="66b07-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="66b07-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="66b07-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="66b07-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_orgcontact"
}-->
```http
GET https://graph.microsoft.com/beta/contacts/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="66b07-135">C#</span><span class="sxs-lookup"><span data-stu-id="66b07-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="66b07-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="66b07-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="66b07-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="66b07-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="66b07-138">Java</span><span class="sxs-lookup"><span data-stu-id="66b07-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-orgcontact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="66b07-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="66b07-139">Response</span></span>
<span data-ttu-id="66b07-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="66b07-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 222

{
  "addresses":[
      {
        "city": "string",
        "countryOrRegion": "string",
        "officeLocation": "string",
        "postalCode": "string",
        "state": "string",
        "street": "string"
      }
  ],
  "companyName": "companyName-value",
  "department": "department-value",
  "displayName": "displayName-value",
  "phones":[
      {
        "type": "string",
        "number": "string"
      }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get orgContact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
