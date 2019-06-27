---
title: Перечисление удаленных элементов
description: Получение списка недавно удаленных элементов.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 31a5336ec1a01b61b522e826daa28efcde9bf9c9
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260874"
---
# <a name="list-deleted-items"></a><span data-ttu-id="38856-103">Перечисление удаленных элементов</span><span class="sxs-lookup"><span data-stu-id="38856-103">List deleted items</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38856-104">Получение списка недавно [удаленных элементов](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="38856-104">Retrieve a list of recently deleted items from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="38856-105">В настоящее время хранение удаленных элементов поддерживается только для ресурсов [group](../resources/group.md) и [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="38856-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="38856-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="38856-106">Permissions</span></span>
<span data-ttu-id="38856-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38856-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="38856-109">Для пользователей: User. Read. ALL, Directory. Read. ALL, User. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="38856-109">For users: User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.AccessAsUser.All</span></span>
* <span data-ttu-id="38856-110">Для групп: Group. Read. ALL, Directory. Read. ALL, Group. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="38856-110">For groups: Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="38856-111">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="38856-111">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http 
GET /directory/deleteditems/microsoft.graph.group
GET /directory/deletedItems/microsoft.graph.user
```

<span data-ttu-id="38856-112">В настоящее время этот API поддерживает получение групп (microsoft.graph.group) и пользователей (microsoft.graph.user) из удаленных элементов.</span><span class="sxs-lookup"><span data-stu-id="38856-112">This API currently supports retrieving object types of groups (microsoft.graph.group) or users (microsoft.graph.user) from deleted items.</span></span> <span data-ttu-id="38856-113">Тип является обязательной частью URI.</span><span class="sxs-lookup"><span data-stu-id="38856-113">The type is specified as a required part of the URI.</span></span> <span data-ttu-id="38856-114">Вызов GET /directory/deleteditems без типа не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38856-114">Calling GET /directory/deleteditems without a type is not supported.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="38856-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="38856-115">Optional query parameters</span></span>
<span data-ttu-id="38856-116">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="38856-116">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="38856-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="38856-117">Request headers</span></span>
| <span data-ttu-id="38856-118">Имя</span><span class="sxs-lookup"><span data-stu-id="38856-118">Name</span></span>      |<span data-ttu-id="38856-119">Описание</span><span class="sxs-lookup"><span data-stu-id="38856-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="38856-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="38856-120">Authorization</span></span>  | <span data-ttu-id="38856-121">Bearer &lt;code&gt; *Обязательный*.</span><span class="sxs-lookup"><span data-stu-id="38856-121">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="38856-122">Accept</span><span class="sxs-lookup"><span data-stu-id="38856-122">Accept</span></span>  | <span data-ttu-id="38856-123">application/json</span><span class="sxs-lookup"><span data-stu-id="38856-123">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="38856-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="38856-124">Request body</span></span>
<span data-ttu-id="38856-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="38856-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38856-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="38856-126">Response</span></span>

<span data-ttu-id="38856-127">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="38856-127">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="38856-128">Пример</span><span class="sxs-lookup"><span data-stu-id="38856-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="38856-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="38856-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_deleteditems"
}-->
```http
GET https://graph.microsoft.com/beta/directory/deleteditems/microsoft.graph.group
```
##### <a name="response"></a><span data-ttu-id="38856-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="38856-130">Response</span></span>
<span data-ttu-id="38856-p103">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="38856-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
  "value": [
    {
      "id":"46cc6179-19d0-473e-97ad-6ff84347bbbb",
      "displayName":"SampleGroup",
      "groupTypes":["Unified"],
      "mail":"example@contoso.com",
      "mailEnabled":true,
      "mailNickname":"Example",
      "securityEnabled":false,
      "visibility":"Public"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="38856-133">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="38856-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="38856-134">C#</span><span class="sxs-lookup"><span data-stu-id="38856-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_deleteditems-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="38856-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="38856-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_deleteditems-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="38856-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="38856-136">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_deleteditems-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List deleteditems",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directory-deleteditems-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/directory-deleteditems-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/directory-deleteditems-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
