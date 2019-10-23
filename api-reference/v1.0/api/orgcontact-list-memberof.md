---
title: Список memberOf
description: Список групп, участником которых является этот контакт организаитонал.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6548d78fced9d0869712ea2644e4f05dffcb0e0c
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2019
ms.locfileid: "37633913"
---
# <a name="list-memberof"></a><span data-ttu-id="3c18b-103">Список memberOf</span><span class="sxs-lookup"><span data-stu-id="3c18b-103">List memberOf</span></span>

<span data-ttu-id="3c18b-104">Список групп, участником которых является это [организационное Контактное лицо](../resources/orgcontact.md) .</span><span class="sxs-lookup"><span data-stu-id="3c18b-104">List the groups that this [organizational contact](../resources/orgcontact.md) is a member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="3c18b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3c18b-105">Permissions</span></span>
<span data-ttu-id="3c18b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3c18b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c18b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3c18b-108">Permission type</span></span>      | <span data-ttu-id="3c18b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3c18b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3c18b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3c18b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3c18b-111">OrgContact. Read. ALL и Group. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="3c18b-111">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span>  |
|<span data-ttu-id="3c18b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3c18b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3c18b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c18b-113">Not supported.</span></span>    |
|<span data-ttu-id="3c18b-114">Для приложения</span><span class="sxs-lookup"><span data-stu-id="3c18b-114">Application</span></span> | <span data-ttu-id="3c18b-115">OrgContact. Read. ALL и Group. Read. ALL, Directory. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="3c18b-115">OrgContact.Read.All and Group.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3c18b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3c18b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3c18b-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3c18b-117">Optional query parameters</span></span>
<span data-ttu-id="3c18b-118">Этот метод поддерживает `$select` [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="3c18b-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) `$select` to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3c18b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3c18b-119">Request headers</span></span>
| <span data-ttu-id="3c18b-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3c18b-120">Header</span></span>       | <span data-ttu-id="3c18b-121">Значение</span><span class="sxs-lookup"><span data-stu-id="3c18b-121">Value</span></span> |
|:-----------|:----------|
| <span data-ttu-id="3c18b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3c18b-122">Authorization</span></span>  | <span data-ttu-id="3c18b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3c18b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3c18b-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3c18b-125">Request body</span></span>
<span data-ttu-id="3c18b-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3c18b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c18b-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c18b-127">Response</span></span>

<span data-ttu-id="3c18b-128">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3c18b-128">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3c18b-129">Пример</span><span class="sxs-lookup"><span data-stu-id="3c18b-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3c18b-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="3c18b-130">Request</span></span>
<span data-ttu-id="3c18b-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3c18b-131">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3c18b-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="3c18b-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contact_get_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contacts/{id}/memberOf
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3c18b-133">C#</span><span class="sxs-lookup"><span data-stu-id="3c18b-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contact-get-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3c18b-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3c18b-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contact-get-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3c18b-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3c18b-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contact-get-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3c18b-136">Java</span><span class="sxs-lookup"><span data-stu-id="3c18b-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/contact-get-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3c18b-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c18b-137">Response</span></span>
<span data-ttu-id="3c18b-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3c18b-138">The following is an example of the response.</span></span>
><span data-ttu-id="3c18b-139">**Примечание**. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3c18b-139">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3c18b-140">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3c18b-140">All the properties will be returned from an actual call.</span></span>
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
