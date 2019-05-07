---
title: Список объектов contactFolder
description: Получение коллекции папок контактов в папке контактов по умолчанию для вошедшего пользователя.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e36e90aad21ee00aaca57656b716dfc00ae57268
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33602002"
---
# <a name="list-contactfolders"></a><span data-ttu-id="6e3bd-103">Список объектов contactFolder</span><span class="sxs-lookup"><span data-stu-id="6e3bd-103">List contactFolders</span></span>

<span data-ttu-id="6e3bd-104">Получение коллекции папок контактов в папке контактов по умолчанию для вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="6e3bd-104">Get the contact folder collection in the default Contacts folder of the signed-in user.</span></span>
## <a name="permissions"></a><span data-ttu-id="6e3bd-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6e3bd-105">Permissions</span></span>
<span data-ttu-id="6e3bd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6e3bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e3bd-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6e3bd-108">Permission type</span></span>      | <span data-ttu-id="6e3bd-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6e3bd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6e3bd-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6e3bd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6e3bd-111">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6e3bd-111">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="6e3bd-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6e3bd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e3bd-113">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6e3bd-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="6e3bd-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6e3bd-114">Application</span></span> | <span data-ttu-id="6e3bd-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6e3bd-115">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="6e3bd-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6e3bd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders
GET /users/{id | userPrincipalName}/contactFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6e3bd-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6e3bd-117">Optional query parameters</span></span>
<span data-ttu-id="6e3bd-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="6e3bd-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6e3bd-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6e3bd-119">Request headers</span></span>
| <span data-ttu-id="6e3bd-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6e3bd-120">Header</span></span>       | <span data-ttu-id="6e3bd-121">Значение</span><span class="sxs-lookup"><span data-stu-id="6e3bd-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6e3bd-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6e3bd-122">Authorization</span></span>  | <span data-ttu-id="6e3bd-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6e3bd-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6e3bd-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6e3bd-125">Content-Type</span></span>   | <span data-ttu-id="6e3bd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6e3bd-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6e3bd-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6e3bd-127">Request body</span></span>
<span data-ttu-id="6e3bd-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6e3bd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e3bd-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="6e3bd-129">Response</span></span>

<span data-ttu-id="6e3bd-130">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [ContactFolder](../resources/contactfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6e3bd-130">If successful, this method returns a `200 OK` response code and collection of [ContactFolder](../resources/contactfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6e3bd-131">Пример</span><span class="sxs-lookup"><span data-stu-id="6e3bd-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6e3bd-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="6e3bd-132">Request</span></span>
<span data-ttu-id="6e3bd-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6e3bd-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contactfolders"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contactFolders
```
##### <a name="response"></a><span data-ttu-id="6e3bd-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="6e3bd-134">Response</span></span>
<span data-ttu-id="6e3bd-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6e3bd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 145

{
  "value": [
    {
      "parentFolderId": "parentFolderId-value",
      "displayName": "displayName-value",
      "id": "id-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="6e3bd-138">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="6e3bd-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6e3bd-139">Языках</span><span class="sxs-lookup"><span data-stu-id="6e3bd-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_contactfolders-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6e3bd-140">Язык</span><span class="sxs-lookup"><span data-stu-id="6e3bd-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_contactfolders-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List contactFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/user-list-contactfolders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/user-list-contactfolders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
