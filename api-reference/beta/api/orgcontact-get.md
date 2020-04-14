---
title: Получение orgContact
description: Получение свойств и связей объекта orgcontact.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 50cb6d85b7bda47a14cbbb58439881c1126e15fc
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43467011"
---
# <a name="get-orgcontact"></a><span data-ttu-id="d80fd-103">Получение orgContact</span><span class="sxs-lookup"><span data-stu-id="d80fd-103">Get orgContact</span></span>

<span data-ttu-id="d80fd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d80fd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d80fd-105">Получение свойств и связей объекта контакта в Организации.</span><span class="sxs-lookup"><span data-stu-id="d80fd-105">Get the properties and relationships of an organizational contact object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d80fd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d80fd-106">Permissions</span></span>
<span data-ttu-id="d80fd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d80fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d80fd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d80fd-109">Permission type</span></span>      | <span data-ttu-id="d80fd-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d80fd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d80fd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d80fd-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d80fd-112">OrgContact. Read. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="d80fd-112">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d80fd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d80fd-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d80fd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d80fd-114">Not supported.</span></span>    |
|<span data-ttu-id="d80fd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d80fd-115">Application</span></span> | <span data-ttu-id="d80fd-116">OrgContact. Read. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="d80fd-116">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d80fd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d80fd-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d80fd-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d80fd-118">Optional query parameters</span></span>
<span data-ttu-id="d80fd-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="d80fd-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d80fd-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d80fd-120">Request headers</span></span>
| <span data-ttu-id="d80fd-121">Имя</span><span class="sxs-lookup"><span data-stu-id="d80fd-121">Name</span></span>       | <span data-ttu-id="d80fd-122">Тип</span><span class="sxs-lookup"><span data-stu-id="d80fd-122">Type</span></span> | <span data-ttu-id="d80fd-123">Описание</span><span class="sxs-lookup"><span data-stu-id="d80fd-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d80fd-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d80fd-124">Authorization</span></span>  | <span data-ttu-id="d80fd-125">string</span><span class="sxs-lookup"><span data-stu-id="d80fd-125">string</span></span>  | <span data-ttu-id="d80fd-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d80fd-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d80fd-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d80fd-128">Request body</span></span>
<span data-ttu-id="d80fd-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d80fd-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d80fd-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="d80fd-130">Response</span></span>

<span data-ttu-id="d80fd-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [orgContact](../resources/orgcontact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d80fd-131">If successful, this method returns a `200 OK` response code and [orgContact](../resources/orgcontact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d80fd-132">Пример</span><span class="sxs-lookup"><span data-stu-id="d80fd-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d80fd-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="d80fd-133">Request</span></span>
<span data-ttu-id="d80fd-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d80fd-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d80fd-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="d80fd-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_orgcontact"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts/{id}
```
# <a name="c"></a>[<span data-ttu-id="d80fd-136">C#</span><span class="sxs-lookup"><span data-stu-id="d80fd-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d80fd-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d80fd-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d80fd-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d80fd-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d80fd-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="d80fd-139">Response</span></span>
<span data-ttu-id="d80fd-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d80fd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
