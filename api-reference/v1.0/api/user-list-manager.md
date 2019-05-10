---
title: Получение руководителя
description: Получение руководителя пользователя. Возвращает пользователя или контакт, назначенный в качестве руководителя пользователя.
localization_priority: Priority
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f877c6f26244c18aba7fbf874ed0a05bda8279e7
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33601792"
---
# <a name="list-manager"></a><span data-ttu-id="01854-104">Получение руководителя</span><span class="sxs-lookup"><span data-stu-id="01854-104">List manager</span></span>

<span data-ttu-id="01854-105">Получение руководителя пользователя.</span><span class="sxs-lookup"><span data-stu-id="01854-105">Get user's manager.</span></span> <span data-ttu-id="01854-106">Возвращает пользователя или контакт, назначенный в качестве руководителя пользователя.</span><span class="sxs-lookup"><span data-stu-id="01854-106">Returns the user or contact assigned as the user's manager.</span></span>
## <a name="permissions"></a><span data-ttu-id="01854-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="01854-107">Permissions</span></span>
<span data-ttu-id="01854-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01854-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01854-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01854-110">Permission type</span></span>      | <span data-ttu-id="01854-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="01854-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01854-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01854-112">Delegated (work or school account)</span></span> | <span data-ttu-id="01854-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="01854-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="01854-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01854-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01854-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01854-115">Not supported.</span></span>    |
|<span data-ttu-id="01854-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="01854-116">Application</span></span> | <span data-ttu-id="01854-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01854-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="01854-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01854-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/manager
GET /users/{id | userPrincipalName}/manager
```
## <a name="optional-query-parameters"></a><span data-ttu-id="01854-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="01854-119">Optional query parameters</span></span>
<span data-ttu-id="01854-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="01854-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="01854-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="01854-121">Request headers</span></span>
| <span data-ttu-id="01854-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="01854-122">Header</span></span>       | <span data-ttu-id="01854-123">Значение</span><span class="sxs-lookup"><span data-stu-id="01854-123">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="01854-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="01854-124">Authorization</span></span>  | <span data-ttu-id="01854-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="01854-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="01854-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="01854-127">Content-Type</span></span>   | <span data-ttu-id="01854-128">application/json</span><span class="sxs-lookup"><span data-stu-id="01854-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="01854-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="01854-129">Request body</span></span>
<span data-ttu-id="01854-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="01854-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01854-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="01854-131">Response</span></span>

<span data-ttu-id="01854-132">В случае успеха этот метод возвращает код отклика `200 OK` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="01854-132">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="01854-133">Пример</span><span class="sxs-lookup"><span data-stu-id="01854-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="01854-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="01854-134">Request</span></span>
<span data-ttu-id="01854-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="01854-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_manager"
}-->
```http
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/manager
```
##### <a name="response"></a><span data-ttu-id="01854-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="01854-136">Response</span></span>
<span data-ttu-id="01854-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="01854-137">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "objectType": "User",
  "id": "111048d2-2761-4347-b978-07354283363b",
  "accountEnabled": true,
  "city": "San Diego",
  "country": "United States",
  "department": "Sales & Marketing",
  "displayName": "Sara Davis",
  "givenName": "Sara",
  "jobTitle": "Finance VP",
  "mail": "SaraD@contoso.onmicrosoft.com",
  "mailNickname": "SaraD",
  "state": "CA",
  "streetAddress": "9256 Towne Center Dr., Suite 400",
  "surname": "Davis",
  "usageLocation": "US",
  "userPrincipalName": "SaraD@contoso.onmicrosoft.com"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="01854-138">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="01854-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="01854-139">C#</span><span class="sxs-lookup"><span data-stu-id="01854-139">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_manager-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="01854-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="01854-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_manager-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/user-list-manager.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/user-list-manager.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
