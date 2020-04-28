---
title: Восстановление удаленного элемента
description: 'Восстановление недавно удаленного элемента из контейнера для удаленных элементов. '
author: keylimesoda
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 911f5c661f8e7393fcbf0f0cf0d8365415779e6a
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181016"
---
# <a name="restore-deleted-item"></a><span data-ttu-id="d1b74-103">Восстановление удаленного элемента</span><span class="sxs-lookup"><span data-stu-id="d1b74-103">Restore deleted item</span></span>

<span data-ttu-id="d1b74-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1b74-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1b74-105">Восстановление недавно удаленного элемента из контейнера для [удаленных элементов](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="d1b74-105">Restores a recently deleted item from [deleted items](../resources/directory.md).</span></span> 

<span data-ttu-id="d1b74-106">В настоящее время функции удаленных элементов поддерживаются только для ресурсов [приложения](../resources/application.md), [групп](../resources/group.md) и [пользователей](../resources/user.md) .</span><span class="sxs-lookup"><span data-stu-id="d1b74-106">Currently, deleted items functionality is only supported for the [application](../resources/application.md), [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="d1b74-107">Вы можете полностью восстановить случайно удаленный элемент.</span><span class="sxs-lookup"><span data-stu-id="d1b74-107">If an item was accidentally deleted, you can fully restore the item.</span></span>

<span data-ttu-id="d1b74-108">Удаленный элемент можно восстановить в течение 30 дней.</span><span class="sxs-lookup"><span data-stu-id="d1b74-108">A recently deleted item will remain available for up to 30 days.</span></span> <span data-ttu-id="d1b74-109">Через 30 дней элемент удаляется без возможности восстановления.</span><span class="sxs-lookup"><span data-stu-id="d1b74-109">After 30 days, the item is permanently deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="d1b74-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d1b74-110">Permissions</span></span>
<span data-ttu-id="d1b74-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1b74-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="d1b74-113">Для приложений: Application. ReadWrite. Овнедби, Application. ReadWrite. ALL, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="d1b74-113">For applications: Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>
* <span data-ttu-id="d1b74-114">Для пользователей: User. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="d1b74-114">For users: User.ReadWrite.All, Directory.AccessAsUser.All</span></span>
* <span data-ttu-id="d1b74-115">Для групп: Group. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="d1b74-115">For groups: Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="d1b74-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d1b74-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directory/deleteditems/{id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="d1b74-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d1b74-117">Request headers</span></span>
| <span data-ttu-id="d1b74-118">Имя</span><span class="sxs-lookup"><span data-stu-id="d1b74-118">Name</span></span>       | <span data-ttu-id="d1b74-119">Описание</span><span class="sxs-lookup"><span data-stu-id="d1b74-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d1b74-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d1b74-120">Authorization</span></span>  | <span data-ttu-id="d1b74-121">&lt;&gt; *Необходим* маркер носителя</span><span class="sxs-lookup"><span data-stu-id="d1b74-121">Bearer &lt;token&gt; *Required*</span></span>|
| <span data-ttu-id="d1b74-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d1b74-122">Content-type</span></span> | <span data-ttu-id="d1b74-123">application/json</span><span class="sxs-lookup"><span data-stu-id="d1b74-123">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d1b74-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d1b74-124">Request body</span></span>
<span data-ttu-id="d1b74-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d1b74-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1b74-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="d1b74-126">Response</span></span>

<span data-ttu-id="d1b74-127">В случае успеха этот метод возвращает код отклика `200 OK` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d1b74-127">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1b74-128">Пример</span><span class="sxs-lookup"><span data-stu-id="d1b74-128">Example</span></span>
### <a name="request"></a><span data-ttu-id="d1b74-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="d1b74-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d1b74-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="d1b74-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directory"
}-->
```http
POST https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb/restore
```
# <a name="c"></a>[<span data-ttu-id="d1b74-131">C#</span><span class="sxs-lookup"><span data-stu-id="d1b74-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d1b74-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d1b74-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d1b74-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d1b74-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="d1b74-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1b74-134">Response</span></span>
<span data-ttu-id="d1b74-p104">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d1b74-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
