---
title: Список memberOf
description: Список групп, в которые входит этот органоайтональный контакт.
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 5eec725428c80c79ef15e195c9d9459a9b97571d
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52039260"
---
# <a name="list-memberof"></a><span data-ttu-id="ee11d-103">Список memberOf</span><span class="sxs-lookup"><span data-stu-id="ee11d-103">List memberOf</span></span>

<span data-ttu-id="ee11d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee11d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ee11d-105">Список групп, в [которые](../resources/orgcontact.md) входит этот организационный контакт.</span><span class="sxs-lookup"><span data-stu-id="ee11d-105">List the groups that this [organizational contact](../resources/orgcontact.md) is a member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="ee11d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ee11d-106">Permissions</span></span>
<span data-ttu-id="ee11d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee11d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee11d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ee11d-109">Permission type</span></span>      | <span data-ttu-id="ee11d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ee11d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee11d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ee11d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ee11d-112">OrgContact.Read.All и Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee11d-112">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span>  |
|<span data-ttu-id="ee11d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ee11d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee11d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ee11d-114">Not supported.</span></span>    |
|<span data-ttu-id="ee11d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ee11d-115">Application</span></span> | <span data-ttu-id="ee11d-116">OrgContact.Read.All и Group.Read.All, Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee11d-116">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="ee11d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ee11d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ee11d-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ee11d-118">Optional query parameters</span></span>
<span data-ttu-id="ee11d-119">Этот метод поддерживает [параметры запроса OData для](/graph/query-parameters) `$select` настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ee11d-119">This method supports the [OData Query Parameters](/graph/query-parameters) `$select` to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ee11d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ee11d-120">Request headers</span></span>
| <span data-ttu-id="ee11d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ee11d-121">Header</span></span>       | <span data-ttu-id="ee11d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ee11d-122">Value</span></span> |
|:-----------|:----------|
| <span data-ttu-id="ee11d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ee11d-123">Authorization</span></span>  | <span data-ttu-id="ee11d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ee11d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ee11d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ee11d-126">Request body</span></span>
<span data-ttu-id="ee11d-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ee11d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee11d-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee11d-128">Response</span></span>

<span data-ttu-id="ee11d-129">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ee11d-129">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ee11d-130">Пример</span><span class="sxs-lookup"><span data-stu-id="ee11d-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ee11d-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="ee11d-131">Request</span></span>
<span data-ttu-id="ee11d-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ee11d-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ee11d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ee11d-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contact_get_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="ee11d-134">C#</span><span class="sxs-lookup"><span data-stu-id="ee11d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contact-get-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ee11d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ee11d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contact-get-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ee11d-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ee11d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contact-get-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ee11d-137">Java</span><span class="sxs-lookup"><span data-stu-id="ee11d-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/contact-get-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ee11d-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="ee11d-138">Response</span></span>
<span data-ttu-id="ee11d-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ee11d-139">The following is an example of the response.</span></span>
><span data-ttu-id="ee11d-140">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ee11d-140">**Note**: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 155

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "024bbfa0-fe5a-4fce-9227-bd6ccf1324bb",
      "createdDateTime": "2018-01-18T18:54:43Z",
      "description": "Best group ever created",
      "displayName": "Best Group",
      "groupTypes": [],
      "isAssignableToRole": null,
      "onPremisesProvisioningErrors": []
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
