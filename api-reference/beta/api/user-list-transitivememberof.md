---
title: Список транзитивных пользователей memberOf
description: Получение групп, ролей каталогов и административных единиц, участником которых является пользователь. Этот запрос API является транзитивным и также возвращает все группы, в которых пользователь является вложенным.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b61b780a34a00f855f3913c8e2b1382eb65d2e14
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35269547"
---
# <a name="list-user-transitive-memberof"></a><span data-ttu-id="ffb10-104">Список транзитивных пользователей memberOf</span><span class="sxs-lookup"><span data-stu-id="ffb10-104">List user transitive memberOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ffb10-105">Получение групп, ролей каталогов и административных единиц, участником которых является пользователь.</span><span class="sxs-lookup"><span data-stu-id="ffb10-105">Get groups, directory roles and administrative units that the user is a member of.</span></span> <span data-ttu-id="ffb10-106">Этот запрос API является транзитивным и также возвращает все группы, в которых пользователь является вложенным.</span><span class="sxs-lookup"><span data-stu-id="ffb10-106">This API request is transitive, and will also return all groups the user is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="ffb10-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ffb10-107">Permissions</span></span>

<span data-ttu-id="ffb10-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ffb10-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ffb10-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ffb10-110">Permission type</span></span>      | <span data-ttu-id="ffb10-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ffb10-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ffb10-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ffb10-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ffb10-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ffb10-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ffb10-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ffb10-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ffb10-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ffb10-115">Not supported.</span></span>    |
|<span data-ttu-id="ffb10-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ffb10-116">Application</span></span> | <span data-ttu-id="ffb10-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffb10-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ffb10-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ffb10-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id | userPrincipalName}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ffb10-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ffb10-119">Optional query parameters</span></span>

<span data-ttu-id="ffb10-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ffb10-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ffb10-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ffb10-121">Request headers</span></span>

| <span data-ttu-id="ffb10-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ffb10-122">Header</span></span>       | <span data-ttu-id="ffb10-123">Значение</span><span class="sxs-lookup"><span data-stu-id="ffb10-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ffb10-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ffb10-124">Authorization</span></span>  | <span data-ttu-id="ffb10-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ffb10-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ffb10-127">Accept</span><span class="sxs-lookup"><span data-stu-id="ffb10-127">Accept</span></span>  | <span data-ttu-id="ffb10-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ffb10-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ffb10-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ffb10-129">Request body</span></span>

<span data-ttu-id="ffb10-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ffb10-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ffb10-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="ffb10-131">Response</span></span>

<span data-ttu-id="ffb10-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ffb10-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ffb10-133">Пример</span><span class="sxs-lookup"><span data-stu-id="ffb10-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="ffb10-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="ffb10-134">Request</span></span>

<span data-ttu-id="ffb10-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ffb10-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_transitivememberof"
}-->

```http
GET https://graph.microsoft.com/beta/me/transitiveMemberOf
```

### <a name="response"></a><span data-ttu-id="ffb10-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="ffb10-136">Response</span></span>

<span data-ttu-id="ffb10-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ffb10-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="ffb10-140">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="ffb10-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ffb10-141">C#</span><span class="sxs-lookup"><span data-stu-id="ffb10-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_transitivememberof-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ffb10-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="ffb10-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_transitivememberof-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="ffb10-143">Цель — C</span><span class="sxs-lookup"><span data-stu-id="ffb10-143">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_transitivememberof-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/user-list-transitivememberof.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/user-list-transitivememberof.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-list-transitivememberof.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
