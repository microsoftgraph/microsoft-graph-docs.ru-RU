---
title: Восстановление удаленного элемента
description: 'Восстановление недавно удаленного элемента из контейнера для удаленных элементов. '
ms.openlocfilehash: 325d4fb3f94d27259f26bc48c8b43f37f7e38d49
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077221"
---
# <a name="restore-deleted-item"></a><span data-ttu-id="8d9ca-103">Восстановление удаленного элемента</span><span class="sxs-lookup"><span data-stu-id="8d9ca-103">Restore deleted item</span></span>

> <span data-ttu-id="8d9ca-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8d9ca-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8d9ca-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d9ca-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8d9ca-106">Восстановление недавно удаленного элемента из контейнера для [удаленных элементов](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="8d9ca-106">Restores a recently deleted item from [deleted items](../resources/directory.md).</span></span> 

<span data-ttu-id="8d9ca-107">В настоящее время хранение удаленных элементов поддерживается только для ресурсов [group](../resources/group.md) и [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="8d9ca-107">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="8d9ca-108">Вы можете полностью восстановить случайно удаленный элемент.</span><span class="sxs-lookup"><span data-stu-id="8d9ca-108">If an item was accidentally deleted, you can fully restore the item.</span></span>

<span data-ttu-id="8d9ca-109">Удаленный элемент можно восстановить в течение 30 дней.</span><span class="sxs-lookup"><span data-stu-id="8d9ca-109">A recently deleted item will remain available for up to 30 days.</span></span> <span data-ttu-id="8d9ca-110">Через 30 дней элемент удаляется без возможности восстановления.</span><span class="sxs-lookup"><span data-stu-id="8d9ca-110">After 30 days, the item is permanently deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="8d9ca-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8d9ca-111">Permissions</span></span>
<span data-ttu-id="8d9ca-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d9ca-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="8d9ca-114">Для пользователей: User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8d9ca-114">For users: User.ReadWrite.All, Directory.AccessAsUser.All</span></span>
* <span data-ttu-id="8d9ca-115">Для групп: Group.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8d9ca-115">For groups: Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="8d9ca-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8d9ca-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directory/deleteditems/{id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="8d9ca-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8d9ca-117">Request headers</span></span>
| <span data-ttu-id="8d9ca-118">Имя</span><span class="sxs-lookup"><span data-stu-id="8d9ca-118">Name</span></span>       | <span data-ttu-id="8d9ca-119">Описание</span><span class="sxs-lookup"><span data-stu-id="8d9ca-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8d9ca-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d9ca-120">Authorization</span></span>  | <span data-ttu-id="8d9ca-121">Bearer &lt;code&gt; *Обязательный*.</span><span class="sxs-lookup"><span data-stu-id="8d9ca-121">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="8d9ca-122">Accept</span><span class="sxs-lookup"><span data-stu-id="8d9ca-122">Accept</span></span> | <span data-ttu-id="8d9ca-123">application/json</span><span class="sxs-lookup"><span data-stu-id="8d9ca-123">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="8d9ca-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8d9ca-124">Request body</span></span>
<span data-ttu-id="8d9ca-125">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8d9ca-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d9ca-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d9ca-126">Response</span></span>

<span data-ttu-id="8d9ca-127">В случае успеха этот метод возвращает код отклика `200 OK` и объект [directoryObject](../resources/directoryobject.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8d9ca-127">If successful, this method returns `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d9ca-128">Пример</span><span class="sxs-lookup"><span data-stu-id="8d9ca-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8d9ca-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d9ca-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directory"
}-->
```http
POST https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb/restore
```
<span data-ttu-id="8d9ca-130">Предоставьте в тексте запроса описание объекта [directoryObject](../resources/directoryobject.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8d9ca-130">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="8d9ca-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d9ca-131">Response</span></span>
<span data-ttu-id="8d9ca-p105">Примечание. Представленный здесь объект отклика может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8d9ca-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create deletedItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->