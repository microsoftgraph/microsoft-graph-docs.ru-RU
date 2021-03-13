---
title: Список directReports
description: Получите прямые отчеты контакта.
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 1d294f80b8bf1e55e1575490fb1b888e78afbd47
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761634"
---
# <a name="list-directreports"></a><span data-ttu-id="94ecb-103">Список directReports</span><span class="sxs-lookup"><span data-stu-id="94ecb-103">List directReports</span></span>

<span data-ttu-id="94ecb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94ecb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="94ecb-105">Получите прямые отчеты для этого [организационного контакта.](../resources/orgcontact.md)</span><span class="sxs-lookup"><span data-stu-id="94ecb-105">Get the direct reports for this [organizational contact](../resources/orgcontact.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="94ecb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="94ecb-106">Permissions</span></span>
<span data-ttu-id="94ecb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94ecb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94ecb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="94ecb-109">Permission type</span></span>      | <span data-ttu-id="94ecb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="94ecb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94ecb-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="94ecb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="94ecb-112">OrgContact.Read.All и Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="94ecb-112">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span>  |
|<span data-ttu-id="94ecb-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="94ecb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94ecb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94ecb-114">Not supported.</span></span>    |
|<span data-ttu-id="94ecb-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="94ecb-115">Application</span></span> | <span data-ttu-id="94ecb-116">OrgContact.Read.All и Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="94ecb-116">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="94ecb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="94ecb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts/{id}/directReports
```
## <a name="optional-query-parameters"></a><span data-ttu-id="94ecb-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="94ecb-118">Optional query parameters</span></span>
<span data-ttu-id="94ecb-119">Этот метод поддерживает `$select` [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="94ecb-119">This method supports the `$select` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="94ecb-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="94ecb-120">Request headers</span></span>
| <span data-ttu-id="94ecb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="94ecb-121">Header</span></span>       | <span data-ttu-id="94ecb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="94ecb-122">Value</span></span> |
|:-----------|:----------|
| <span data-ttu-id="94ecb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="94ecb-123">Authorization</span></span>  | <span data-ttu-id="94ecb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="94ecb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="94ecb-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="94ecb-126">Request body</span></span>
<span data-ttu-id="94ecb-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="94ecb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94ecb-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="94ecb-128">Response</span></span>

<span data-ttu-id="94ecb-129">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="94ecb-129">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="94ecb-130">Пример</span><span class="sxs-lookup"><span data-stu-id="94ecb-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="94ecb-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="94ecb-131">Request</span></span>
<span data-ttu-id="94ecb-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="94ecb-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="94ecb-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="94ecb-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contacts_get_directreports"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts/{id}/directReports
```
# <a name="c"></a>[<span data-ttu-id="94ecb-134">C#</span><span class="sxs-lookup"><span data-stu-id="94ecb-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contacts-get-directreports-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="94ecb-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94ecb-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contacts-get-directreports-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="94ecb-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="94ecb-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contacts-get-directreports-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="94ecb-137">Java</span><span class="sxs-lookup"><span data-stu-id="94ecb-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/contacts-get-directreports-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="94ecb-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="94ecb-138">Response</span></span>
<span data-ttu-id="94ecb-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="94ecb-139">The following is an example of the response.</span></span>
><span data-ttu-id="94ecb-140">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="94ecb-140">**Note**: The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 455

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryObjects/$entity",
  "value": [
    {
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

