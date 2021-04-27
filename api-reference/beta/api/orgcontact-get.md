---
title: Get orgContact
description: Извлечение свойств и связей объекта orgcontact.
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: a75c40ce61224303ee3dd3a3ec3d4b4e6881e627
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055563"
---
# <a name="get-orgcontact"></a><span data-ttu-id="c7703-103">Get orgContact</span><span class="sxs-lookup"><span data-stu-id="c7703-103">Get orgContact</span></span>

<span data-ttu-id="c7703-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7703-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7703-105">Получите свойства и связи объекта контактов организации.</span><span class="sxs-lookup"><span data-stu-id="c7703-105">Get the properties and relationships of an organizational contact object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c7703-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c7703-106">Permissions</span></span>
<span data-ttu-id="c7703-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7703-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7703-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c7703-109">Permission type</span></span>      | <span data-ttu-id="c7703-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c7703-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7703-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c7703-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c7703-112">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c7703-112">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c7703-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c7703-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7703-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7703-114">Not supported.</span></span>    |
|<span data-ttu-id="c7703-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="c7703-115">Application</span></span> | <span data-ttu-id="c7703-116">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7703-116">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c7703-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7703-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c7703-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c7703-118">Optional query parameters</span></span>
<span data-ttu-id="c7703-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c7703-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c7703-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c7703-120">Request headers</span></span>
| <span data-ttu-id="c7703-121">Имя</span><span class="sxs-lookup"><span data-stu-id="c7703-121">Name</span></span>       | <span data-ttu-id="c7703-122">Тип</span><span class="sxs-lookup"><span data-stu-id="c7703-122">Type</span></span> | <span data-ttu-id="c7703-123">Описание</span><span class="sxs-lookup"><span data-stu-id="c7703-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c7703-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7703-124">Authorization</span></span>  | <span data-ttu-id="c7703-125">string</span><span class="sxs-lookup"><span data-stu-id="c7703-125">string</span></span>  | <span data-ttu-id="c7703-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c7703-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c7703-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c7703-128">Request body</span></span>
<span data-ttu-id="c7703-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c7703-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7703-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7703-130">Response</span></span>

<span data-ttu-id="c7703-131">В случае успеха этот метод возвращает код отклика и `200 OK` [объект orgContact](../resources/orgcontact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c7703-131">If successful, this method returns a `200 OK` response code and [orgContact](../resources/orgcontact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c7703-132">Пример</span><span class="sxs-lookup"><span data-stu-id="c7703-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c7703-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7703-133">Request</span></span>
<span data-ttu-id="c7703-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c7703-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c7703-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="c7703-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_orgcontact"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts/{id}
```
# <a name="c"></a>[<span data-ttu-id="c7703-136">C#</span><span class="sxs-lookup"><span data-stu-id="c7703-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c7703-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c7703-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c7703-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c7703-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c7703-139">Java</span><span class="sxs-lookup"><span data-stu-id="c7703-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-orgcontact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c7703-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7703-140">Response</span></span>
<span data-ttu-id="c7703-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c7703-141">Here is an example of the response.</span></span> <span data-ttu-id="c7703-142">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c7703-142">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgContact"
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
