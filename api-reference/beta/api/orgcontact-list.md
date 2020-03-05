---
title: Список Оргконтактс
description: Получение списка контактов Организации для этой Организации.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 134347a227ba33e1134890496710207c83983d79
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456259"
---
# <a name="list-orgcontacts"></a><span data-ttu-id="ea946-103">Список Оргконтактс</span><span class="sxs-lookup"><span data-stu-id="ea946-103">List orgContacts</span></span>

<span data-ttu-id="ea946-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ea946-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea946-105">Получение списка контактов Организации для этой Организации.</span><span class="sxs-lookup"><span data-stu-id="ea946-105">Get the list of organizational contacts for this organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="ea946-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ea946-106">Permissions</span></span>
<span data-ttu-id="ea946-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea946-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea946-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ea946-109">Permission type</span></span>      | <span data-ttu-id="ea946-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ea946-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ea946-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ea946-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ea946-112">OrgContact. Read. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="ea946-112">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ea946-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ea946-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea946-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea946-114">Not supported.</span></span>    |
|<span data-ttu-id="ea946-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ea946-115">Application</span></span> | <span data-ttu-id="ea946-116">OrgContact. Read. ALL, Directory. Read. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="ea946-116">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ea946-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ea946-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ea946-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ea946-118">Optional query parameters</span></span>
<span data-ttu-id="ea946-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ea946-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ea946-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ea946-120">Request headers</span></span>
| <span data-ttu-id="ea946-121">Имя</span><span class="sxs-lookup"><span data-stu-id="ea946-121">Name</span></span>       | <span data-ttu-id="ea946-122">Тип</span><span class="sxs-lookup"><span data-stu-id="ea946-122">Type</span></span> | <span data-ttu-id="ea946-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ea946-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ea946-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea946-124">Authorization</span></span>  | <span data-ttu-id="ea946-125">string</span><span class="sxs-lookup"><span data-stu-id="ea946-125">string</span></span>  | <span data-ttu-id="ea946-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea946-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ea946-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ea946-128">Request body</span></span>
<span data-ttu-id="ea946-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ea946-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea946-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="ea946-130">Response</span></span>

<span data-ttu-id="ea946-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [orgContact](../resources/orgcontact.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ea946-131">If successful, this method returns a `200 OK` response code and a collection of [orgContact](../resources/orgcontact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ea946-132">Пример</span><span class="sxs-lookup"><span data-stu-id="ea946-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ea946-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="ea946-133">Request</span></span>
<span data-ttu-id="ea946-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ea946-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ea946-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="ea946-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_orgcontact"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts
```
# <a name="c"></a>[<span data-ttu-id="ea946-136">C#</span><span class="sxs-lookup"><span data-stu-id="ea946-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ea946-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ea946-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ea946-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ea946-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ea946-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea946-139">Response</span></span>
<span data-ttu-id="ea946-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ea946-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
