---
title: Получение имени руководителя
description: Получите менеджера этого организационного контакта.
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 74bab941c4ab22a626fbd1ed1cc8023768f08ffb
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761669"
---
# <a name="get-manager"></a><span data-ttu-id="c0828-103">Получение имени руководителя</span><span class="sxs-lookup"><span data-stu-id="c0828-103">Get manager</span></span>

<span data-ttu-id="c0828-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0828-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c0828-105">Получите менеджера этого организационного контакта.</span><span class="sxs-lookup"><span data-stu-id="c0828-105">Get this organizational contact's manager.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0828-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c0828-106">Permissions</span></span>
<span data-ttu-id="c0828-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0828-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0828-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c0828-109">Permission type</span></span>      | <span data-ttu-id="c0828-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c0828-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0828-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c0828-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c0828-112">OrgContact.Read.All и Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0828-112">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span>   |
|<span data-ttu-id="c0828-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c0828-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0828-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0828-114">Not supported.</span></span>    |
|<span data-ttu-id="c0828-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c0828-115">Application</span></span> | <span data-ttu-id="c0828-116">OrgContact.Read.All и Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0828-116">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="c0828-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c0828-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /contacts/{id}/manager
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c0828-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c0828-118">Optional query parameters</span></span>
<span data-ttu-id="c0828-119">Этот метод поддерживает `$select` [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="c0828-119">This method supports the `$select` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c0828-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c0828-120">Request headers</span></span>
| <span data-ttu-id="c0828-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c0828-121">Header</span></span>       | <span data-ttu-id="c0828-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c0828-122">Value</span></span> |
|:-----------|:----------|
| <span data-ttu-id="c0828-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c0828-123">Authorization</span></span>  | <span data-ttu-id="c0828-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c0828-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c0828-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c0828-126">Request body</span></span>
<span data-ttu-id="c0828-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c0828-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0828-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0828-128">Response</span></span>

<span data-ttu-id="c0828-129">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c0828-129">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c0828-130">Пример</span><span class="sxs-lookup"><span data-stu-id="c0828-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="c0828-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="c0828-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c0828-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="c0828-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_manager"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts/{id}/manager
```
# <a name="c"></a>[<span data-ttu-id="c0828-133">C#</span><span class="sxs-lookup"><span data-stu-id="c0828-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-manager-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c0828-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c0828-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-manager-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c0828-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c0828-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-manager-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c0828-136">Java</span><span class="sxs-lookup"><span data-stu-id="c0828-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-manager-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c0828-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="c0828-137">Response</span></span>
<span data-ttu-id="c0828-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c0828-138">The following is an example of the response.</span></span>
><span data-ttu-id="c0828-139">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c0828-139">**Note**: The response object shown here might be shortened for readability.</span></span> 
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

