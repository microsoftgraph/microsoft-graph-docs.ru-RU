---
title: Список транзитивных пользователей memberOf
description: Получение групп, ролей каталогов и административных единиц, участником которых является пользователь. Этот запрос API является транзитивным и также возвращает все группы, в которых пользователь является вложенным.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: afef92aaf8d96abaf6e1fdfe35887d4f14a7ee1a
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870675"
---
# <a name="list-user-transitive-memberof"></a><span data-ttu-id="cd5df-104">Список транзитивных пользователей memberOf</span><span class="sxs-lookup"><span data-stu-id="cd5df-104">List user transitive memberOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd5df-105">Получение групп, ролей каталогов и административных единиц, участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="cd5df-105">Get groups, directory roles and administrative units that the user is a member of.</span></span> <span data-ttu-id="cd5df-106">Этот запрос API является транзитивным и также возвращает все группы, в которых пользователь является вложенным.</span><span class="sxs-lookup"><span data-stu-id="cd5df-106">This API request is transitive, and will also return all groups the user is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="cd5df-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cd5df-107">Permissions</span></span>

<span data-ttu-id="cd5df-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd5df-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd5df-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cd5df-110">Permission type</span></span>      | <span data-ttu-id="cd5df-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cd5df-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cd5df-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cd5df-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cd5df-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cd5df-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cd5df-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cd5df-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd5df-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd5df-115">Not supported.</span></span>    |
|<span data-ttu-id="cd5df-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cd5df-116">Application</span></span> | <span data-ttu-id="cd5df-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd5df-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="cd5df-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cd5df-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id | userPrincipalName}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cd5df-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cd5df-119">Optional query parameters</span></span>

<span data-ttu-id="cd5df-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="cd5df-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cd5df-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cd5df-121">Request headers</span></span>

| <span data-ttu-id="cd5df-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cd5df-122">Header</span></span>       | <span data-ttu-id="cd5df-123">Значение</span><span class="sxs-lookup"><span data-stu-id="cd5df-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cd5df-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cd5df-124">Authorization</span></span>  | <span data-ttu-id="cd5df-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cd5df-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cd5df-127">Accept</span><span class="sxs-lookup"><span data-stu-id="cd5df-127">Accept</span></span>  | <span data-ttu-id="cd5df-128">application/json</span><span class="sxs-lookup"><span data-stu-id="cd5df-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd5df-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cd5df-129">Request body</span></span>

<span data-ttu-id="cd5df-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cd5df-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cd5df-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="cd5df-131">Response</span></span>

<span data-ttu-id="cd5df-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cd5df-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd5df-133">Пример</span><span class="sxs-lookup"><span data-stu-id="cd5df-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="cd5df-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="cd5df-134">Request</span></span>

<span data-ttu-id="cd5df-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cd5df-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="cd5df-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="cd5df-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/transitiveMemberOf
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cd5df-137">C#</span><span class="sxs-lookup"><span data-stu-id="cd5df-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cd5df-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cd5df-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cd5df-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cd5df-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cd5df-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="cd5df-140">Response</span></span>

<span data-ttu-id="cd5df-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cd5df-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "List transitiveMsemberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
