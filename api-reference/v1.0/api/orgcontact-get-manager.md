---
title: Получение имени руководителя
description: Получите менеджера этого организационного контакта.
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 0a99bfc16c6380093d8e13930f8b6801ef86ce02
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50943508"
---
# <a name="get-manager"></a><span data-ttu-id="9d7c8-103">Получение имени руководителя</span><span class="sxs-lookup"><span data-stu-id="9d7c8-103">Get manager</span></span>

<span data-ttu-id="9d7c8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d7c8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9d7c8-105">Получите менеджера этого организационного контакта.</span><span class="sxs-lookup"><span data-stu-id="9d7c8-105">Get this organizational contact's manager.</span></span>

## <a name="permissions"></a><span data-ttu-id="9d7c8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9d7c8-106">Permissions</span></span>
<span data-ttu-id="9d7c8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d7c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d7c8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9d7c8-109">Permission type</span></span>      | <span data-ttu-id="9d7c8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9d7c8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d7c8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9d7c8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9d7c8-112">OrgContact.Read.All и Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="9d7c8-112">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span>   |
|<span data-ttu-id="9d7c8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9d7c8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d7c8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d7c8-114">Not supported.</span></span>    |
|<span data-ttu-id="9d7c8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9d7c8-115">Application</span></span> | <span data-ttu-id="9d7c8-116">OrgContact.Read.All и Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="9d7c8-116">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="9d7c8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9d7c8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /contacts/{id}/manager
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9d7c8-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9d7c8-118">Optional query parameters</span></span>
<span data-ttu-id="9d7c8-119">Этот метод поддерживает `$select` [параметры запроса OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9d7c8-119">This method supports the `$select` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9d7c8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9d7c8-120">Request headers</span></span>
| <span data-ttu-id="9d7c8-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9d7c8-121">Header</span></span>       | <span data-ttu-id="9d7c8-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9d7c8-122">Value</span></span> |
|:-----------|:----------|
| <span data-ttu-id="9d7c8-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9d7c8-123">Authorization</span></span>  | <span data-ttu-id="9d7c8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9d7c8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9d7c8-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9d7c8-126">Request body</span></span>
<span data-ttu-id="9d7c8-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9d7c8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9d7c8-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d7c8-128">Response</span></span>

<span data-ttu-id="9d7c8-129">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9d7c8-129">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9d7c8-130">Пример</span><span class="sxs-lookup"><span data-stu-id="9d7c8-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="9d7c8-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="9d7c8-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="9d7c8-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="9d7c8-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_manager_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts/{id}/manager
```
# <a name="c"></a>[<span data-ttu-id="9d7c8-133">C#</span><span class="sxs-lookup"><span data-stu-id="9d7c8-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-manager-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9d7c8-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9d7c8-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-manager-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9d7c8-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9d7c8-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-manager-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9d7c8-136">Java</span><span class="sxs-lookup"><span data-stu-id="9d7c8-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-manager-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9d7c8-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d7c8-137">Response</span></span>
<span data-ttu-id="9d7c8-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9d7c8-138">The following is an example of the response.</span></span>
><span data-ttu-id="9d7c8-139">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9d7c8-139">**Note**: The response object shown here might be shortened for readability.</span></span> 
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

