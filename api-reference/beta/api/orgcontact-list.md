---
title: Список Оргконтактс
description: Получение списка контактов Организации для этой Организации.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 21902b537ff14be15b469da124a47c1a5f0b1eb7
ms.sourcegitcommit: 23aa2941cfb8bd744d8d59e8bba9d2c5f57f8e29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/29/2019
ms.locfileid: "36667528"
---
# <a name="list-orgcontacts"></a><span data-ttu-id="c794a-103">Список Оргконтактс</span><span class="sxs-lookup"><span data-stu-id="c794a-103">List orgContacts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c794a-104">Получение списка контактов Организации для этой Организации.</span><span class="sxs-lookup"><span data-stu-id="c794a-104">Get the list of organizational contacts for this organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="c794a-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c794a-105">Permissions</span></span>
<span data-ttu-id="c794a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c794a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c794a-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c794a-108">Permission type</span></span>      | <span data-ttu-id="c794a-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c794a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c794a-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c794a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c794a-111">OrgContact. Read. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="c794a-111">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c794a-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c794a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c794a-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c794a-113">Not supported.</span></span>    |
|<span data-ttu-id="c794a-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c794a-114">Application</span></span> | <span data-ttu-id="c794a-115">OrgContact. Read. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c794a-115">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c794a-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c794a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c794a-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c794a-117">Optional query parameters</span></span>
<span data-ttu-id="c794a-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c794a-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c794a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c794a-119">Request headers</span></span>
| <span data-ttu-id="c794a-120">Имя</span><span class="sxs-lookup"><span data-stu-id="c794a-120">Name</span></span>       | <span data-ttu-id="c794a-121">Тип</span><span class="sxs-lookup"><span data-stu-id="c794a-121">Type</span></span> | <span data-ttu-id="c794a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c794a-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c794a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c794a-123">Authorization</span></span>  | <span data-ttu-id="c794a-124">string</span><span class="sxs-lookup"><span data-stu-id="c794a-124">string</span></span>  | <span data-ttu-id="c794a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c794a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c794a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c794a-127">Request body</span></span>
<span data-ttu-id="c794a-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c794a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c794a-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="c794a-129">Response</span></span>

<span data-ttu-id="c794a-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [orgContact](../resources/orgcontact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c794a-130">If successful, this method returns a `200 OK` response code and a collection of [orgContact](../resources/orgcontact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c794a-131">Пример</span><span class="sxs-lookup"><span data-stu-id="c794a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c794a-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="c794a-132">Request</span></span>
<span data-ttu-id="c794a-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c794a-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c794a-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="c794a-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_orgcontact"
}-->
```http
GET https://graph.microsoft.com/beta/contacts
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c794a-135">C#</span><span class="sxs-lookup"><span data-stu-id="c794a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c794a-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c794a-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c794a-137">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c794a-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c794a-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="c794a-138">Response</span></span>
<span data-ttu-id="c794a-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c794a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 222

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List orgContact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
