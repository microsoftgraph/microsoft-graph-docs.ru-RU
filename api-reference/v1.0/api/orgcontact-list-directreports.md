---
title: Список directReports
description: Получение подчиненных отчетов о контакте.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 01a46af833b7dc5d827d73f2fd48353e0e2b3622
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2019
ms.locfileid: "37633920"
---
# <a name="list-directreports"></a><span data-ttu-id="60e49-103">Список directReports</span><span class="sxs-lookup"><span data-stu-id="60e49-103">List directReports</span></span>

<span data-ttu-id="60e49-104">Получение подчиненных контактов для этого [организационного контакта](../resources/orgcontact.md).</span><span class="sxs-lookup"><span data-stu-id="60e49-104">Get the direct reports for this [organizational contact](../resources/orgcontact.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="60e49-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="60e49-105">Permissions</span></span>
<span data-ttu-id="60e49-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60e49-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60e49-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="60e49-108">Permission type</span></span>      | <span data-ttu-id="60e49-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="60e49-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="60e49-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="60e49-110">Delegated (work or school account)</span></span> | <span data-ttu-id="60e49-111">OrgContact. Read. ALL и Group. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="60e49-111">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span>  |
|<span data-ttu-id="60e49-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="60e49-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="60e49-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60e49-113">Not supported.</span></span>    |
|<span data-ttu-id="60e49-114">Для приложения</span><span class="sxs-lookup"><span data-stu-id="60e49-114">Application</span></span> | <span data-ttu-id="60e49-115">OrgContact. Read. ALL и Group. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="60e49-115">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="60e49-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="60e49-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts/{id}/directReports
```
## <a name="optional-query-parameters"></a><span data-ttu-id="60e49-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="60e49-117">Optional query parameters</span></span>
<span data-ttu-id="60e49-118">Этот метод поддерживает `$select` [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="60e49-118">This method supports the `$select` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="60e49-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="60e49-119">Request headers</span></span>
| <span data-ttu-id="60e49-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="60e49-120">Header</span></span>       | <span data-ttu-id="60e49-121">Значение</span><span class="sxs-lookup"><span data-stu-id="60e49-121">Value</span></span> |
|:-----------|:----------|
| <span data-ttu-id="60e49-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="60e49-122">Authorization</span></span>  | <span data-ttu-id="60e49-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="60e49-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="60e49-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="60e49-125">Request body</span></span>
<span data-ttu-id="60e49-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="60e49-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60e49-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="60e49-127">Response</span></span>

<span data-ttu-id="60e49-128">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="60e49-128">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="60e49-129">Пример</span><span class="sxs-lookup"><span data-stu-id="60e49-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="60e49-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="60e49-130">Request</span></span>
<span data-ttu-id="60e49-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="60e49-131">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="60e49-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="60e49-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contacts_get_directreports"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts/{id}/directReports
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="60e49-133">C#</span><span class="sxs-lookup"><span data-stu-id="60e49-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contacts-get-directreports-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="60e49-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="60e49-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contacts-get-directreports-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="60e49-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="60e49-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contacts-get-directreports-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="60e49-136">Java</span><span class="sxs-lookup"><span data-stu-id="60e49-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/contacts-get-directreports-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="60e49-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="60e49-137">Response</span></span>
<span data-ttu-id="60e49-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="60e49-138">The following is an example of the response.</span></span>
><span data-ttu-id="60e49-139">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="60e49-139">**Note**: The response object shown here might be shortened for readability.</span></span> 
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
