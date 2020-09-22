---
title: Список Транситивемембероф
description: Получение групп, участником которых является контакт органзиатионал. Этот запрос API является транзитивным и также возвращает все группы, в которых пользователь является вложенным.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 780abea12cf61655f8d529dadf2f8c4414401dc2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48032903"
---
# <a name="list-transitivememberof"></a><span data-ttu-id="b094e-104">Список Транситивемембероф</span><span class="sxs-lookup"><span data-stu-id="b094e-104">List transitiveMemberOf</span></span>

<span data-ttu-id="b094e-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b094e-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b094e-106">Получение групп, членом которых является это [организационное Контактное лицо](../resources/orgcontact.md) .</span><span class="sxs-lookup"><span data-stu-id="b094e-106">Get groups that this [organizational contact](../resources/orgcontact.md) is a member of.</span></span> <span data-ttu-id="b094e-107">Запрос API является транзитивным и возвращает все группы. Контактное лицо является вложенным элементом.</span><span class="sxs-lookup"><span data-stu-id="b094e-107">The API request is transitive, and returns all groups the organizational contact is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="b094e-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b094e-108">Permissions</span></span>

<span data-ttu-id="b094e-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b094e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b094e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b094e-111">Permission type</span></span>      | <span data-ttu-id="b094e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b094e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b094e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b094e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b094e-114">OrgContact. Read. ALL и Group. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="b094e-114">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span>  |
|<span data-ttu-id="b094e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b094e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b094e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b094e-116">Not supported.</span></span>    |
|<span data-ttu-id="b094e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b094e-117">Application</span></span> | <span data-ttu-id="b094e-118">OrgContact. Read. ALL и Group. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="b094e-118">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b094e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b094e-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /contacts/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b094e-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b094e-120">Optional query parameters</span></span>

<span data-ttu-id="b094e-121">Этот метод поддерживает `$select` [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="b094e-121">This method supports the `$select` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b094e-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b094e-122">Request headers</span></span>

| <span data-ttu-id="b094e-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b094e-123">Header</span></span>       | <span data-ttu-id="b094e-124">Значение</span><span class="sxs-lookup"><span data-stu-id="b094e-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b094e-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b094e-125">Authorization</span></span>  | <span data-ttu-id="b094e-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b094e-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b094e-128">Accept</span><span class="sxs-lookup"><span data-stu-id="b094e-128">Accept</span></span>  | <span data-ttu-id="b094e-129">application/json</span><span class="sxs-lookup"><span data-stu-id="b094e-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b094e-130">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b094e-130">Request body</span></span>

<span data-ttu-id="b094e-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b094e-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b094e-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="b094e-132">Response</span></span>

<span data-ttu-id="b094e-133">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b094e-133">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b094e-134">Пример</span><span class="sxs-lookup"><span data-stu-id="b094e-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="b094e-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="b094e-135">Request</span></span>

<span data-ttu-id="b094e-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b094e-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b094e-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="b094e-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "orgcontact_list_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="b094e-138">C#</span><span class="sxs-lookup"><span data-stu-id="b094e-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/orgcontact-list-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b094e-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b094e-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/orgcontact-list-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b094e-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b094e-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/orgcontact-list-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b094e-141">Java</span><span class="sxs-lookup"><span data-stu-id="b094e-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/orgcontact-list-transitivememberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b094e-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="b094e-142">Response</span></span>

<span data-ttu-id="b094e-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b094e-143">The following is an example of the response.</span></span>
><span data-ttu-id="b094e-144">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b094e-144">**Note**: The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List orgContact transitiveMemberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

