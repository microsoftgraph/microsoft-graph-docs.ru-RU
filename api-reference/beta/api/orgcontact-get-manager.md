---
title: 'orgContact: получение менеджера'
description: Получение руководителя контакта
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 87880fd90e409a1e79c2755d07fa8229fa8d3a4c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979877"
---
# <a name="orgcontact-get-manager"></a><span data-ttu-id="10165-103">orgContact: получение менеджера</span><span class="sxs-lookup"><span data-stu-id="10165-103">orgContact: Get manager</span></span>

<span data-ttu-id="10165-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10165-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10165-105">Получение руководителя контакта</span><span class="sxs-lookup"><span data-stu-id="10165-105">Get the contact's manager</span></span>

## <a name="permissions"></a><span data-ttu-id="10165-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="10165-106">Permissions</span></span>
<span data-ttu-id="10165-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10165-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10165-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10165-109">Permission type</span></span>      | <span data-ttu-id="10165-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="10165-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="10165-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10165-111">Delegated (work or school account)</span></span> | <span data-ttu-id="10165-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="10165-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="10165-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10165-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10165-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10165-114">Not supported.</span></span>    |
|<span data-ttu-id="10165-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="10165-115">Application</span></span> | <span data-ttu-id="10165-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10165-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="10165-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10165-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /contacts/{id}/manager
```

## <a name="optional-query-parameters"></a><span data-ttu-id="10165-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="10165-118">Optional query parameters</span></span>
<span data-ttu-id="10165-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="10165-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="10165-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10165-120">Request headers</span></span>
| <span data-ttu-id="10165-121">Имя</span><span class="sxs-lookup"><span data-stu-id="10165-121">Name</span></span>       | <span data-ttu-id="10165-122">Тип</span><span class="sxs-lookup"><span data-stu-id="10165-122">Type</span></span> | <span data-ttu-id="10165-123">Описание</span><span class="sxs-lookup"><span data-stu-id="10165-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="10165-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="10165-124">Authorization</span></span>  | <span data-ttu-id="10165-125">string</span><span class="sxs-lookup"><span data-stu-id="10165-125">string</span></span>  | <span data-ttu-id="10165-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10165-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="10165-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="10165-128">Request body</span></span>
<span data-ttu-id="10165-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="10165-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10165-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="10165-130">Response</span></span>

<span data-ttu-id="10165-131">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="10165-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="10165-132">Пример</span><span class="sxs-lookup"><span data-stu-id="10165-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="10165-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="10165-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="10165-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="10165-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_manager"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts/{id}/manager
```
# <a name="c"></a>[<span data-ttu-id="10165-135">C#</span><span class="sxs-lookup"><span data-stu-id="10165-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-manager-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="10165-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="10165-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-manager-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="10165-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="10165-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-manager-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="10165-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="10165-138">Response</span></span>

<span data-ttu-id="10165-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="10165-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": false
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 455

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryObjects/$entity",
    "@odata.type": "#microsoft.graph.user",
    "id": "24fcbca3-c3e2-48bf-9ffc-c7f81b81483d",
    "businessPhones": [
        "+1 205 555 0108"
    ],
    "displayName": "Diego Siciliani",
    "givenName": "Diego",
    "jobTitle": "CVP Finance",
    "mail": "DiegoS@contoso.com",
    "mobilePhone": null,
    "officeLocation": "14/1108",
    "preferredLanguage": "en-US",
    "surname": "Siciliani",
    "userPrincipalName": "DiegoS@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get manager",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


