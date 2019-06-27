---
title: Перечисление пользователей
description: Получение списка объектов user.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 33ba7cced053b6beaa76eb764247ef573d20e6e3
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35269995"
---
# <a name="list-users"></a><span data-ttu-id="23b59-103">Перечисление пользователей</span><span class="sxs-lookup"><span data-stu-id="23b59-103">List users</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23b59-104">Получение списка объектов user.</span><span class="sxs-lookup"><span data-stu-id="23b59-104">Retrieve a list of user objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="23b59-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="23b59-105">Permissions</span></span>

<span data-ttu-id="23b59-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23b59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23b59-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="23b59-108">Permission type</span></span>      | <span data-ttu-id="23b59-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="23b59-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="23b59-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="23b59-110">Delegated (work or school account)</span></span> | <span data-ttu-id="23b59-111">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="23b59-111">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="23b59-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="23b59-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23b59-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23b59-113">Not supported.</span></span>    |
|<span data-ttu-id="23b59-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="23b59-114">Application</span></span> | <span data-ttu-id="23b59-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23b59-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="23b59-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="23b59-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="23b59-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="23b59-117">Optional query parameters</span></span>

<span data-ttu-id="23b59-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="23b59-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="23b59-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="23b59-119">Request headers</span></span>
| <span data-ttu-id="23b59-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="23b59-120">Header</span></span>        | <span data-ttu-id="23b59-121">Значение</span><span class="sxs-lookup"><span data-stu-id="23b59-121">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="23b59-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="23b59-122">Authorization</span></span> | <span data-ttu-id="23b59-123">Bearer {токен} (обязательный)</span><span class="sxs-lookup"><span data-stu-id="23b59-123">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="23b59-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="23b59-124">Content-Type</span></span>  | <span data-ttu-id="23b59-125">application/json</span><span class="sxs-lookup"><span data-stu-id="23b59-125">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="23b59-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="23b59-126">Request body</span></span>

<span data-ttu-id="23b59-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="23b59-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23b59-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="23b59-128">Response</span></span>

<span data-ttu-id="23b59-129">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [user](../resources/user.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="23b59-129">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23b59-130">Пример</span><span class="sxs-lookup"><span data-stu-id="23b59-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="23b59-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="23b59-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/beta/users
```

##### <a name="response"></a><span data-ttu-id="23b59-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="23b59-132">Response</span></span>

<span data-ttu-id="23b59-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="23b59-133">Here is an example of the response.</span></span> <span data-ttu-id="23b59-134">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="23b59-134">Note: The response object shown here may be truncated for brevity.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 608

{
  "value": [
    {
      "businessPhones": [
        "businessPhones-value"
      ],
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "jobTitle": "jobTitle-value",
      "mail": "mail-value",
      "mobilePhone": "mobilePhone-value",
      "officeLocation": "officeLocation-value",
      "preferredLanguage": "preferredLanguage-value",
      "surname": "surname-value",
      "userPrincipalName": "userPrincipalName-value",
      "id": "id-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="23b59-135">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="23b59-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="23b59-136">C#</span><span class="sxs-lookup"><span data-stu-id="23b59-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_users-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="23b59-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="23b59-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_users-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="23b59-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="23b59-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_users-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/user-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
