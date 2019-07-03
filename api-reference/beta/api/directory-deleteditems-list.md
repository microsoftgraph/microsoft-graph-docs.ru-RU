---
title: Перечисление удаленных элементов
description: Получение списка недавно удаленных элементов.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 80a719b2212dc06fcb1351b61b8e3338b8d8eec9
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35437119"
---
# <a name="list-deleted-items"></a><span data-ttu-id="959ee-103">Перечисление удаленных элементов</span><span class="sxs-lookup"><span data-stu-id="959ee-103">List deleted items</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="959ee-104">Получение списка недавно [удаленных элементов](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="959ee-104">Retrieve a list of recently deleted items from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="959ee-105">В настоящее время хранение удаленных элементов поддерживается только для ресурсов [group](../resources/group.md) и [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="959ee-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="959ee-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="959ee-106">Permissions</span></span>
<span data-ttu-id="959ee-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="959ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="959ee-109">Для пользователей: User. Read. ALL, Directory. Read. ALL, User. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="959ee-109">For users: User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.AccessAsUser.All</span></span>
* <span data-ttu-id="959ee-110">Для групп: Group. Read. ALL, Directory. Read. ALL, Group. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="959ee-110">For groups: Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="959ee-111">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="959ee-111">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http 
GET /directory/deleteditems/microsoft.graph.group
GET /directory/deletedItems/microsoft.graph.user
```

<span data-ttu-id="959ee-112">В настоящее время этот API поддерживает получение групп (microsoft.graph.group) и пользователей (microsoft.graph.user) из удаленных элементов.</span><span class="sxs-lookup"><span data-stu-id="959ee-112">This API currently supports retrieving object types of groups (microsoft.graph.group) or users (microsoft.graph.user) from deleted items.</span></span> <span data-ttu-id="959ee-113">Тип является обязательной частью URI.</span><span class="sxs-lookup"><span data-stu-id="959ee-113">The type is specified as a required part of the URI.</span></span> <span data-ttu-id="959ee-114">Вызов GET /directory/deleteditems без типа не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="959ee-114">Calling GET /directory/deleteditems without a type is not supported.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="959ee-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="959ee-115">Optional query parameters</span></span>
<span data-ttu-id="959ee-116">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="959ee-116">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="959ee-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="959ee-117">Request headers</span></span>
| <span data-ttu-id="959ee-118">Имя</span><span class="sxs-lookup"><span data-stu-id="959ee-118">Name</span></span>      |<span data-ttu-id="959ee-119">Описание</span><span class="sxs-lookup"><span data-stu-id="959ee-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="959ee-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="959ee-120">Authorization</span></span>  | <span data-ttu-id="959ee-121">Bearer &lt;code&gt; *Обязательный*.</span><span class="sxs-lookup"><span data-stu-id="959ee-121">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="959ee-122">Accept</span><span class="sxs-lookup"><span data-stu-id="959ee-122">Accept</span></span>  | <span data-ttu-id="959ee-123">application/json</span><span class="sxs-lookup"><span data-stu-id="959ee-123">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="959ee-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="959ee-124">Request body</span></span>
<span data-ttu-id="959ee-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="959ee-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="959ee-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="959ee-126">Response</span></span>

<span data-ttu-id="959ee-127">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="959ee-127">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="959ee-128">Пример</span><span class="sxs-lookup"><span data-stu-id="959ee-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="959ee-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="959ee-129">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="959ee-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="959ee-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_deleteditems"
}-->
```http
GET https://graph.microsoft.com/beta/directory/deleteditems/microsoft.graph.group
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="959ee-131">C#</span><span class="sxs-lookup"><span data-stu-id="959ee-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-deleteditems-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="959ee-132">Javascript</span><span class="sxs-lookup"><span data-stu-id="959ee-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-deleteditems-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="959ee-133">Цель — C</span><span class="sxs-lookup"><span data-stu-id="959ee-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-deleteditems-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="959ee-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="959ee-134">Response</span></span>
<span data-ttu-id="959ee-p103">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="959ee-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
