---
title: Перечисление orgContacts
description: Получение списка контактов Организации для этой Организации.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f7c356f2247e3d5a4b4c2939b6a97faf4ae2c2c7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48079405"
---
# <a name="list-orgcontacts"></a><span data-ttu-id="e74ec-103">Перечисление orgContacts</span><span class="sxs-lookup"><span data-stu-id="e74ec-103">List orgContacts</span></span>

<span data-ttu-id="e74ec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e74ec-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e74ec-105">Получение списка [контактов](../resources/orgcontact.md) Организации для этой Организации.</span><span class="sxs-lookup"><span data-stu-id="e74ec-105">Get the list of [organizational contacts](../resources/orgcontact.md) for this organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="e74ec-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e74ec-106">Permissions</span></span>
<span data-ttu-id="e74ec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e74ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e74ec-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e74ec-109">Permission type</span></span>      | <span data-ttu-id="e74ec-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e74ec-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e74ec-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e74ec-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e74ec-112">OrgContact. Read. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="e74ec-112">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e74ec-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e74ec-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e74ec-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e74ec-114">Not supported.</span></span>    |
|<span data-ttu-id="e74ec-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="e74ec-115">Application</span></span> | <span data-ttu-id="e74ec-116">OrgContact. Read. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="e74ec-116">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e74ec-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e74ec-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e74ec-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e74ec-118">Optional query parameters</span></span>
<span data-ttu-id="e74ec-119">Этот метод поддерживает `$expand` `$filter` `$select` параметры запросов,, и `$top` [OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="e74ec-119">This method supports the `$expand`, `$filter`, `$select`, and `$top` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e74ec-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e74ec-120">Request headers</span></span>
| <span data-ttu-id="e74ec-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e74ec-121">Header</span></span>       | <span data-ttu-id="e74ec-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e74ec-122">Value</span></span> |
|:-----------|:----------|
| <span data-ttu-id="e74ec-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e74ec-123">Authorization</span></span>  |<span data-ttu-id="e74ec-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e74ec-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e74ec-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e74ec-126">Request body</span></span>
<span data-ttu-id="e74ec-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e74ec-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e74ec-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="e74ec-128">Response</span></span>

<span data-ttu-id="e74ec-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [orgContact](../resources/orgcontact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e74ec-129">If successful, this method returns a `200 OK` response code and a collection of [orgContact](../resources/orgcontact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e74ec-130">Пример</span><span class="sxs-lookup"><span data-stu-id="e74ec-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e74ec-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e74ec-131">Request</span></span>
<span data-ttu-id="e74ec-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e74ec-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e74ec-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="e74ec-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_orgcontact"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts
```
# <a name="c"></a>[<span data-ttu-id="e74ec-134">C#</span><span class="sxs-lookup"><span data-stu-id="e74ec-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e74ec-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e74ec-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e74ec-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e74ec-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e74ec-137">Java</span><span class="sxs-lookup"><span data-stu-id="e74ec-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-orgcontact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e74ec-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="e74ec-138">Response</span></span>
<span data-ttu-id="e74ec-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e74ec-139">The following is an example of the response.</span></span>
><span data-ttu-id="e74ec-140">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e74ec-140">**Note**: The response object shown here might be shortened for readability.</span></span> 
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

