---
title: Список memberOf
description: Список групп, участником которых является этот контакт организаитонал.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: acab2983a68e5ddfe054b4efefc9308b64eb448d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48077753"
---
# <a name="list-memberof"></a><span data-ttu-id="a14fe-103">Список memberOf</span><span class="sxs-lookup"><span data-stu-id="a14fe-103">List memberOf</span></span>

<span data-ttu-id="a14fe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a14fe-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a14fe-105">Список групп, участником которых является это [организационное Контактное лицо](../resources/orgcontact.md) .</span><span class="sxs-lookup"><span data-stu-id="a14fe-105">List the groups that this [organizational contact](../resources/orgcontact.md) is a member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="a14fe-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a14fe-106">Permissions</span></span>
<span data-ttu-id="a14fe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a14fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a14fe-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a14fe-109">Permission type</span></span>      | <span data-ttu-id="a14fe-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a14fe-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a14fe-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a14fe-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a14fe-112">OrgContact. Read. ALL и Group. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="a14fe-112">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span>  |
|<span data-ttu-id="a14fe-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a14fe-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a14fe-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a14fe-114">Not supported.</span></span>    |
|<span data-ttu-id="a14fe-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="a14fe-115">Application</span></span> | <span data-ttu-id="a14fe-116">OrgContact. Read. ALL и Group. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="a14fe-116">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="a14fe-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a14fe-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a14fe-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a14fe-118">Optional query parameters</span></span>
<span data-ttu-id="a14fe-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) `$select` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="a14fe-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) `$select` to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a14fe-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a14fe-120">Request headers</span></span>
| <span data-ttu-id="a14fe-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a14fe-121">Header</span></span>       | <span data-ttu-id="a14fe-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a14fe-122">Value</span></span> |
|:-----------|:----------|
| <span data-ttu-id="a14fe-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a14fe-123">Authorization</span></span>  | <span data-ttu-id="a14fe-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a14fe-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a14fe-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a14fe-126">Request body</span></span>
<span data-ttu-id="a14fe-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a14fe-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a14fe-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="a14fe-128">Response</span></span>

<span data-ttu-id="a14fe-129">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a14fe-129">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a14fe-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a14fe-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a14fe-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a14fe-131">Request</span></span>
<span data-ttu-id="a14fe-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a14fe-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a14fe-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a14fe-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contact_get_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="a14fe-134">C#</span><span class="sxs-lookup"><span data-stu-id="a14fe-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contact-get-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a14fe-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a14fe-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contact-get-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a14fe-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a14fe-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contact-get-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a14fe-137">Java</span><span class="sxs-lookup"><span data-stu-id="a14fe-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/contact-get-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a14fe-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="a14fe-138">Response</span></span>
<span data-ttu-id="a14fe-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a14fe-139">The following is an example of the response.</span></span>
><span data-ttu-id="a14fe-140">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a14fe-140">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a14fe-141">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a14fe-141">All the properties will be returned from an actual call.</span></span>
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

