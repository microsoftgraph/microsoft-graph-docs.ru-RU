---
title: Перечисление удаленных элементов
description: Получение списка недавно удаленных элементов.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 72a7e810f26b281158cc83c91627d6abf7982301
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32455200"
---
# <a name="list-deleted-items"></a><span data-ttu-id="ad5ed-103">Перечисление удаленных элементов</span><span class="sxs-lookup"><span data-stu-id="ad5ed-103">List deleted items</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad5ed-104">Получение списка недавно [удаленных элементов](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="ad5ed-104">Retrieve a list of recently deleted items from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="ad5ed-105">В настоящее время хранение удаленных элементов поддерживается только для ресурсов [group](../resources/group.md) и [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="ad5ed-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="ad5ed-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ad5ed-106">Permissions</span></span>
<span data-ttu-id="ad5ed-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad5ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="ad5ed-109">Для пользователей: User. Read. ALL, Directory. Read. ALL, User. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="ad5ed-109">For users: User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.AccessAsUser.All</span></span>
* <span data-ttu-id="ad5ed-110">Для групп: Group. Read. ALL, Directory. Read. ALL, Group. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="ad5ed-110">For groups: Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="ad5ed-111">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ad5ed-111">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http 
GET /directory/deleteditems/microsoft.graph.group
GET /directory/deletedItems/microsoft.graph.user
```

<span data-ttu-id="ad5ed-112">В настоящее время этот API поддерживает получение групп (microsoft.graph.group) и пользователей (microsoft.graph.user) из удаленных элементов.</span><span class="sxs-lookup"><span data-stu-id="ad5ed-112">This API currently supports retrieving object types of groups (microsoft.graph.group) or users (microsoft.graph.user) from deleted items.</span></span> <span data-ttu-id="ad5ed-113">Тип является обязательной частью URI.</span><span class="sxs-lookup"><span data-stu-id="ad5ed-113">The type is specified as a required part of the URI.</span></span> <span data-ttu-id="ad5ed-114">Вызов GET /directory/deleteditems без типа не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad5ed-114">Calling GET /directory/deleteditems without a type is not supported.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="ad5ed-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ad5ed-115">Optional query parameters</span></span>
<span data-ttu-id="ad5ed-116">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="ad5ed-116">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ad5ed-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ad5ed-117">Request headers</span></span>
| <span data-ttu-id="ad5ed-118">Имя</span><span class="sxs-lookup"><span data-stu-id="ad5ed-118">Name</span></span>      |<span data-ttu-id="ad5ed-119">Описание</span><span class="sxs-lookup"><span data-stu-id="ad5ed-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ad5ed-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad5ed-120">Authorization</span></span>  | <span data-ttu-id="ad5ed-121">Bearer &lt;code&gt; *Обязательный*.</span><span class="sxs-lookup"><span data-stu-id="ad5ed-121">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="ad5ed-122">Accept</span><span class="sxs-lookup"><span data-stu-id="ad5ed-122">Accept</span></span>  | <span data-ttu-id="ad5ed-123">application/json</span><span class="sxs-lookup"><span data-stu-id="ad5ed-123">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ad5ed-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ad5ed-124">Request body</span></span>
<span data-ttu-id="ad5ed-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ad5ed-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad5ed-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad5ed-126">Response</span></span>

<span data-ttu-id="ad5ed-127">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ad5ed-127">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ad5ed-128">Пример</span><span class="sxs-lookup"><span data-stu-id="ad5ed-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ad5ed-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad5ed-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_deleteditems"
}-->
```http
GET https://graph.microsoft.com/beta/directory/deleteditems/microsoft.graph.group
```
##### <a name="response"></a><span data-ttu-id="ad5ed-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad5ed-130">Response</span></span>
<span data-ttu-id="ad5ed-p103">Примечание. Показанный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ad5ed-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/directory-deleteditems-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
