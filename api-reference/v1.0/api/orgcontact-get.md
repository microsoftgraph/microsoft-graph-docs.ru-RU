---
title: Get orgContact
description: Извлечение свойств объекта orgContact.
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: f3702f51779bfb42d794aa011bc671b5b7dd99d3
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761655"
---
# <a name="get-orgcontact"></a><span data-ttu-id="9af0a-103">Get orgContact</span><span class="sxs-lookup"><span data-stu-id="9af0a-103">Get orgContact</span></span>

<span data-ttu-id="9af0a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9af0a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9af0a-105">Получите свойства и связи [организационного контакта.](../resources/orgcontact.md)</span><span class="sxs-lookup"><span data-stu-id="9af0a-105">Get the properties and relationships of an [organizational contact](../resources/orgcontact.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9af0a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9af0a-106">Permissions</span></span>
<span data-ttu-id="9af0a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9af0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9af0a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9af0a-109">Permission type</span></span>      | <span data-ttu-id="9af0a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9af0a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9af0a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9af0a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9af0a-112">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9af0a-112">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9af0a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9af0a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9af0a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9af0a-114">Not supported.</span></span>    |
|<span data-ttu-id="9af0a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9af0a-115">Application</span></span> | <span data-ttu-id="9af0a-116">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9af0a-116">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9af0a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9af0a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9af0a-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9af0a-118">Optional query parameters</span></span>
<span data-ttu-id="9af0a-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$select` и `$expand` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="9af0a-119">This method supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9af0a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9af0a-120">Request headers</span></span>
| <span data-ttu-id="9af0a-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9af0a-121">Header</span></span>       | <span data-ttu-id="9af0a-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9af0a-122">Value</span></span> |
|:-----------|:----------|
| <span data-ttu-id="9af0a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9af0a-123">Authorization</span></span>  | <span data-ttu-id="9af0a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9af0a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9af0a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9af0a-126">Request body</span></span>
<span data-ttu-id="9af0a-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9af0a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9af0a-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="9af0a-128">Response</span></span>

<span data-ttu-id="9af0a-129">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект orgContact](../resources/orgcontact.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="9af0a-129">If successful, this method returns a `200 OK` response code and an [orgContact](../resources/orgcontact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9af0a-130">Пример</span><span class="sxs-lookup"><span data-stu-id="9af0a-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9af0a-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="9af0a-131">Request</span></span>
<span data-ttu-id="9af0a-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9af0a-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9af0a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="9af0a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_orgcontact"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts/{id}
```
# <a name="c"></a>[<span data-ttu-id="9af0a-134">C#</span><span class="sxs-lookup"><span data-stu-id="9af0a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9af0a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9af0a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9af0a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9af0a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9af0a-137">Java</span><span class="sxs-lookup"><span data-stu-id="9af0a-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-orgcontact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9af0a-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="9af0a-138">Response</span></span>
<span data-ttu-id="9af0a-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9af0a-139">The following is an example of the response.</span></span>
><span data-ttu-id="9af0a-140">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9af0a-140">**Note**: The response object shown here might be shortened for readability.</span></span> 
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

