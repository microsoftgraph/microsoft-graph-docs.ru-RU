---
title: Восстановление удаленного элемента
description: 'Восстановление недавно удаленного элемента из контейнера для удаленных элементов. '
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f58233f90e232c18d4a7a4aef3b355c51a38036e
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33591732"
---
# <a name="restore-deleted-item"></a><span data-ttu-id="657c1-103">Восстановление удаленного элемента</span><span class="sxs-lookup"><span data-stu-id="657c1-103">Restore deleted item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="657c1-104">Восстановление недавно удаленного элемента из контейнера для [удаленных элементов](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="657c1-104">Restores a recently deleted item from [deleted items](../resources/directory.md).</span></span> 

<span data-ttu-id="657c1-105">В настоящее время хранение удаленных элементов поддерживается только для ресурсов [group](../resources/group.md) и [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="657c1-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="657c1-106">Вы можете полностью восстановить случайно удаленный элемент.</span><span class="sxs-lookup"><span data-stu-id="657c1-106">If an item was accidentally deleted, you can fully restore the item.</span></span>

<span data-ttu-id="657c1-107">Удаленный элемент можно восстановить в течение 30 дней.</span><span class="sxs-lookup"><span data-stu-id="657c1-107">A recently deleted item will remain available for up to 30 days.</span></span> <span data-ttu-id="657c1-108">Через 30 дней элемент удаляется без возможности восстановления.</span><span class="sxs-lookup"><span data-stu-id="657c1-108">After 30 days, the item is permanently deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="657c1-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="657c1-109">Permissions</span></span>
<span data-ttu-id="657c1-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="657c1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="657c1-112">Для пользователей: User. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="657c1-112">For users: User.ReadWrite.All, Directory.AccessAsUser.All</span></span>
* <span data-ttu-id="657c1-113">Для групп: Group. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="657c1-113">For groups: Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="657c1-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="657c1-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directory/deleteditems/{id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="657c1-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="657c1-115">Request headers</span></span>
| <span data-ttu-id="657c1-116">Имя</span><span class="sxs-lookup"><span data-stu-id="657c1-116">Name</span></span>       | <span data-ttu-id="657c1-117">Описание</span><span class="sxs-lookup"><span data-stu-id="657c1-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="657c1-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="657c1-118">Authorization</span></span>  | <span data-ttu-id="657c1-119">Bearer &lt;code&gt; *Обязательный*.</span><span class="sxs-lookup"><span data-stu-id="657c1-119">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="657c1-120">Accept</span><span class="sxs-lookup"><span data-stu-id="657c1-120">Accept</span></span> | <span data-ttu-id="657c1-121">application/json</span><span class="sxs-lookup"><span data-stu-id="657c1-121">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="657c1-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="657c1-122">Request body</span></span>
<span data-ttu-id="657c1-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="657c1-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="657c1-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="657c1-124">Response</span></span>

<span data-ttu-id="657c1-125">В случае успеха этот метод возвращает код отклика `200 OK` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="657c1-125">If successful, this method returns `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="657c1-126">Пример</span><span class="sxs-lookup"><span data-stu-id="657c1-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="657c1-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="657c1-127">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directory"
}-->
```http
POST https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb/restore
```
<span data-ttu-id="657c1-128">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="657c1-128">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="657c1-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="657c1-129">Response</span></span>
<span data-ttu-id="657c1-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="657c1-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects/$entity",
  "@odata.type":"#microsoft.graph.group",
  "id":"46cc6179-19d0-473e-97ad-6ff84347bbbb",
  "displayName":"SampleGroup",
  "groupTypes":["Unified"],
  "mail":"example@contoso.com",
  "mailEnabled":true,
  "mailNickname":"Example",
  "securityEnabled":false,
  "visibility":"Public"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="657c1-132">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="657c1-132">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="657c1-133">Языках</span><span class="sxs-lookup"><span data-stu-id="657c1-133">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_directory-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="657c1-134">Язык</span><span class="sxs-lookup"><span data-stu-id="657c1-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_directory-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create deletedItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directory-deleteditems-restore.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/directory-deleteditems-restore.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
