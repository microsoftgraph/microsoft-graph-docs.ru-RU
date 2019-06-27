---
title: Список участников
description: Получение списка пользователей, которым назначена роль каталога.  Роли каталогов можно назначать только пользователям.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 006335d683ab36ff3607b26a587573b4a412b55f
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35272361"
---
# <a name="list-members"></a><span data-ttu-id="3ac6a-104">Список элементов</span><span class="sxs-lookup"><span data-stu-id="3ac6a-104">List members</span></span>

<span data-ttu-id="3ac6a-105">Получение списка пользователей, которым назначена роль каталога.</span><span class="sxs-lookup"><span data-stu-id="3ac6a-105">Retrieve a list of the users that are assigned to the directory role.</span></span>  <span data-ttu-id="3ac6a-106">Роли каталогов можно назначать только пользователям.</span><span class="sxs-lookup"><span data-stu-id="3ac6a-106">Only users can be assigned to a directory role.</span></span>
## <a name="permissions"></a><span data-ttu-id="3ac6a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3ac6a-107">Permissions</span></span>
<span data-ttu-id="3ac6a-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ac6a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3ac6a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3ac6a-110">Permission type</span></span>      | <span data-ttu-id="3ac6a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3ac6a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3ac6a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3ac6a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3ac6a-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3ac6a-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3ac6a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3ac6a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ac6a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ac6a-115">Not supported.</span></span>    |
|<span data-ttu-id="3ac6a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3ac6a-116">Application</span></span> | <span data-ttu-id="3ac6a-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ac6a-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3ac6a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3ac6a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3ac6a-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3ac6a-119">Optional query parameters</span></span>
<span data-ttu-id="3ac6a-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3ac6a-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3ac6a-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3ac6a-121">Request headers</span></span>
| <span data-ttu-id="3ac6a-122">Имя</span><span class="sxs-lookup"><span data-stu-id="3ac6a-122">Name</span></span>       | <span data-ttu-id="3ac6a-123">Тип</span><span class="sxs-lookup"><span data-stu-id="3ac6a-123">Type</span></span> | <span data-ttu-id="3ac6a-124">Описание</span><span class="sxs-lookup"><span data-stu-id="3ac6a-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3ac6a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ac6a-125">Authorization</span></span>  | <span data-ttu-id="3ac6a-126">string</span><span class="sxs-lookup"><span data-stu-id="3ac6a-126">string</span></span>  | <span data-ttu-id="3ac6a-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3ac6a-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3ac6a-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3ac6a-129">Request body</span></span>
<span data-ttu-id="3ac6a-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3ac6a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ac6a-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="3ac6a-131">Response</span></span>

<span data-ttu-id="3ac6a-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3ac6a-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3ac6a-133">Пример</span><span class="sxs-lookup"><span data-stu-id="3ac6a-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3ac6a-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="3ac6a-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryRoles/{id}/members
```
##### <a name="response"></a><span data-ttu-id="3ac6a-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ac6a-135">Response</span></span>
<span data-ttu-id="3ac6a-p105">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3ac6a-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "businessPhones":["000-000-0000"],
      "displayName":"First Last",
      "givenName":"First",
      "jobTitle":null,
      "mail":"first@example.com",
      "officeLocation":null,
      "preferredLanguage":"en-US",
      "surname":"Last",
      "userPrincipalName":"first@example.com"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="3ac6a-138">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="3ac6a-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3ac6a-139">C#</span><span class="sxs-lookup"><span data-stu-id="3ac6a-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_members-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3ac6a-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="3ac6a-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_members-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3ac6a-141">Цель — C</span><span class="sxs-lookup"><span data-stu-id="3ac6a-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_members-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/directoryrole-list-members.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/directoryrole-list-members.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/directoryrole-list-members.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
