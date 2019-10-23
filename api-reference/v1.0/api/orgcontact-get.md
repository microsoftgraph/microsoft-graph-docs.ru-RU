---
title: Получение orgContact
description: Получение свойств объекта orgContact.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3f3ed6d94a51809b9c3838b5e9cb6972f824db5a
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2019
ms.locfileid: "37633981"
---
# <a name="get-orgcontact"></a><span data-ttu-id="4c5ea-103">Получение orgContact</span><span class="sxs-lookup"><span data-stu-id="4c5ea-103">Get orgContact</span></span>

<span data-ttu-id="4c5ea-104">Получение свойств и связей [контакта Организации](../resources/orgcontact.md).</span><span class="sxs-lookup"><span data-stu-id="4c5ea-104">Get the properties and relationships of an [organizational contact](../resources/orgcontact.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4c5ea-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4c5ea-105">Permissions</span></span>
<span data-ttu-id="4c5ea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c5ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c5ea-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c5ea-108">Permission type</span></span>      | <span data-ttu-id="4c5ea-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c5ea-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c5ea-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c5ea-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4c5ea-111">OrgContact. Read. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="4c5ea-111">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4c5ea-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c5ea-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c5ea-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c5ea-113">Not supported.</span></span>    |
|<span data-ttu-id="4c5ea-114">Для приложения</span><span class="sxs-lookup"><span data-stu-id="4c5ea-114">Application</span></span> | <span data-ttu-id="4c5ea-115">OrgContact. Read. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="4c5ea-115">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c5ea-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c5ea-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4c5ea-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4c5ea-117">Optional query parameters</span></span>
<span data-ttu-id="4c5ea-118">Этот метод поддерживает `$select` `$expand` [параметры запросов OData](/graph/query-parameters) и для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="4c5ea-118">This method supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4c5ea-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4c5ea-119">Request headers</span></span>
| <span data-ttu-id="4c5ea-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4c5ea-120">Header</span></span>       | <span data-ttu-id="4c5ea-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4c5ea-121">Value</span></span> |
|:-----------|:----------|
| <span data-ttu-id="4c5ea-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4c5ea-122">Authorization</span></span>  | <span data-ttu-id="4c5ea-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c5ea-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4c5ea-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4c5ea-125">Request body</span></span>
<span data-ttu-id="4c5ea-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4c5ea-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c5ea-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="4c5ea-127">Response</span></span>

<span data-ttu-id="4c5ea-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [orgContact](../resources/orgcontact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4c5ea-128">If successful, this method returns a `200 OK` response code and an [orgContact](../resources/orgcontact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4c5ea-129">Пример</span><span class="sxs-lookup"><span data-stu-id="4c5ea-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4c5ea-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c5ea-130">Request</span></span>
<span data-ttu-id="4c5ea-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c5ea-131">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="4c5ea-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="4c5ea-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_orgcontact"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4c5ea-133">C#</span><span class="sxs-lookup"><span data-stu-id="4c5ea-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4c5ea-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4c5ea-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4c5ea-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4c5ea-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4c5ea-136">Java</span><span class="sxs-lookup"><span data-stu-id="4c5ea-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-orgcontact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4c5ea-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c5ea-137">Response</span></span>
<span data-ttu-id="4c5ea-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4c5ea-138">The following is an example of the response.</span></span>
><span data-ttu-id="4c5ea-139">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4c5ea-139">**Note**: The response object shown here might be shortened for readability.</span></span> 
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
