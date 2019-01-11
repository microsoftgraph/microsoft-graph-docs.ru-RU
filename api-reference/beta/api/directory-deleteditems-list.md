---
title: Перечисление удаленных элементов
description: Получение списка недавно удаленных элементов.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: ef23704c01a7d1b6cd3a85ffcab1dc34ded0936d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879438"
---
# <a name="list-deleted-items"></a><span data-ttu-id="4eec1-103">Перечисление удаленных элементов</span><span class="sxs-lookup"><span data-stu-id="4eec1-103">List deleted items</span></span>

> <span data-ttu-id="4eec1-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4eec1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4eec1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4eec1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4eec1-106">Получение списка недавно [удаленных элементов](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="4eec1-106">Retrieve a list of recently deleted items from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="4eec1-107">В настоящее время хранение удаленных элементов поддерживается только для ресурсов [group](../resources/group.md) и [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="4eec1-107">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="4eec1-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4eec1-108">Permissions</span></span>
<span data-ttu-id="4eec1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4eec1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="4eec1-111">Для пользователей: User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4eec1-111">For users: User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.AccessAsUser.All</span></span>
* <span data-ttu-id="4eec1-112">Для групп: Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4eec1-112">For groups: Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="4eec1-113">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4eec1-113">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http 
GET /directory/deleteditems/microsoft.graph.group
GET /directory/deletedItems/microsoft.graph.user
```

<span data-ttu-id="4eec1-114">В настоящее время этот API поддерживает получение групп (microsoft.graph.group) и пользователей (microsoft.graph.user) из удаленных элементов.</span><span class="sxs-lookup"><span data-stu-id="4eec1-114">This API currently supports retrieving object types of groups (microsoft.graph.group) or users (microsoft.graph.user) from deleted items.</span></span> <span data-ttu-id="4eec1-115">Тип является обязательной частью URI.</span><span class="sxs-lookup"><span data-stu-id="4eec1-115">The type is specified as a required part of the URI.</span></span> <span data-ttu-id="4eec1-116">Вызов GET /directory/deleteditems без типа не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4eec1-116">Calling GET /directory/deleteditems without a type is not supported.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="4eec1-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4eec1-117">Optional query parameters</span></span>
<span data-ttu-id="4eec1-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="4eec1-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4eec1-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4eec1-119">Request headers</span></span>
| <span data-ttu-id="4eec1-120">Имя</span><span class="sxs-lookup"><span data-stu-id="4eec1-120">Name</span></span>      |<span data-ttu-id="4eec1-121">Описание</span><span class="sxs-lookup"><span data-stu-id="4eec1-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4eec1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4eec1-122">Authorization</span></span>  | <span data-ttu-id="4eec1-123">Bearer &lt;code&gt; *Обязательный*.</span><span class="sxs-lookup"><span data-stu-id="4eec1-123">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="4eec1-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4eec1-124">Accept</span></span>  | <span data-ttu-id="4eec1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4eec1-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="4eec1-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4eec1-126">Request body</span></span>
<span data-ttu-id="4eec1-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4eec1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4eec1-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="4eec1-128">Response</span></span>

<span data-ttu-id="4eec1-129">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4eec1-129">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4eec1-130">Пример</span><span class="sxs-lookup"><span data-stu-id="4eec1-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4eec1-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="4eec1-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_deleteditems"
}-->
```http
GET https://graph.microsoft.com/beta/directory/deleteditems/microsoft.graph.group
```
##### <a name="response"></a><span data-ttu-id="4eec1-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="4eec1-132">Response</span></span>
<span data-ttu-id="4eec1-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4eec1-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List deleteditems",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
