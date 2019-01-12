---
title: Тип ресурса directoryRole
description: Представляет роль directory Azure AD. Каталог роли Azure AD также называются *ролями администратора*. Дополнительные сведения о ролях каталогов (администратор) в разделе назначение ролей администратора в Azure AD. Microsoft Graph можно назначить роли каталог, чтобы предоставлять им разрешения целевой роли пользователей. Для чтения роли каталога или обновите его члены, необходимо активировать в клиентов. Только роль directory Администраторы организации активируется по умолчанию. Активация других ролей доступны directory отправить запрос POST с Идентификатором directoryRoleTemplate, лежащие в основе роли каталога. Наследуется от directoryObject.
localization_priority: Priority
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4b3379bbbecd86612043dcc3cb8455f5c43ba9cf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939548"
---
# <a name="directoryrole-resource-type"></a><span data-ttu-id="ed1bf-110">Тип ресурса directoryRole</span><span class="sxs-lookup"><span data-stu-id="ed1bf-110">directoryRole resource type</span></span>

<span data-ttu-id="ed1bf-111">Представляет роль directory Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ed1bf-111">Represents an Azure AD directory role.</span></span> <span data-ttu-id="ed1bf-112">Каталог роли Azure AD также называются *ролями администратора*.</span><span class="sxs-lookup"><span data-stu-id="ed1bf-112">Azure AD directory roles are also known as *administrator roles*.</span></span> <span data-ttu-id="ed1bf-113">Дополнительные сведения о ролях каталогов (администратор) можно [Назначение ролей администратора в Azure AD](http://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/).</span><span class="sxs-lookup"><span data-stu-id="ed1bf-113">For more information about directory (administrator) roles, see [Assigning administrator roles in Azure AD](http://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/).</span></span> <span data-ttu-id="ed1bf-114">Microsoft Graph можно назначить роли каталог, чтобы предоставлять им разрешения целевой роли пользователей.</span><span class="sxs-lookup"><span data-stu-id="ed1bf-114">With the Microsoft Graph, you can assign users to directory roles to grant them the permissions of the target role.</span></span> <span data-ttu-id="ed1bf-115">Для чтения роли каталога или обновите его члены, необходимо активировать в клиентов.</span><span class="sxs-lookup"><span data-stu-id="ed1bf-115">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="ed1bf-116">Только роль directory Администраторы организации активируется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ed1bf-116">Only the Company Administrators directory role is activated by default.</span></span> <span data-ttu-id="ed1bf-117">Активация других ролей доступны directory отправить запрос POST с Идентификатором [directoryRoleTemplate](directoryroletemplate.md) , лежащие в основе роли каталога.</span><span class="sxs-lookup"><span data-stu-id="ed1bf-117">To activate other available directory roles you send a POST request with the ID of the [directoryRoleTemplate](directoryroletemplate.md) on which the directory role is based.</span></span> <span data-ttu-id="ed1bf-118">Наследуется от [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="ed1bf-118">Inherits from [directoryObject](directoryobject.md).</span></span>
<span data-ttu-id="ed1bf-119">Этот ресурс поддерживает:</span><span class="sxs-lookup"><span data-stu-id="ed1bf-119">This resource supports:</span></span>

- <span data-ttu-id="ed1bf-120">отслеживание дополнений, удалений и обновлений с помощью [запроса изменений](/graph/delta-query-overview) (функция [delta](../api/directoryrole-delta.md)).</span><span class="sxs-lookup"><span data-stu-id="ed1bf-120">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryrole-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="ed1bf-121">Методы</span><span class="sxs-lookup"><span data-stu-id="ed1bf-121">Methods</span></span>

| <span data-ttu-id="ed1bf-122">Метод</span><span class="sxs-lookup"><span data-stu-id="ed1bf-122">Method</span></span>       | <span data-ttu-id="ed1bf-123">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="ed1bf-123">Return Type</span></span>  |<span data-ttu-id="ed1bf-124">Описание</span><span class="sxs-lookup"><span data-stu-id="ed1bf-124">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ed1bf-125">Получение directoryRole</span><span class="sxs-lookup"><span data-stu-id="ed1bf-125">Get directoryRole</span></span>](../api/directoryrole-get.md) | [<span data-ttu-id="ed1bf-126">directoryRole</span><span class="sxs-lookup"><span data-stu-id="ed1bf-126">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="ed1bf-127">Считывание свойств и отношений объекта directoryRole.</span><span class="sxs-lookup"><span data-stu-id="ed1bf-127">Read properties and relationships of directoryRole object.</span></span> |
|[<span data-ttu-id="ed1bf-128">Перечисление объектов directoryRole</span><span class="sxs-lookup"><span data-stu-id="ed1bf-128">List directoryRoles</span></span>](../api/directoryrole-list.md) | <span data-ttu-id="ed1bf-129">Коллекция объектов [directoryRole](directoryrole.md)</span><span class="sxs-lookup"><span data-stu-id="ed1bf-129">[directoryRole](directoryrole.md) collection</span></span> | <span data-ttu-id="ed1bf-130">Перечисление ролей каталога, активированных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="ed1bf-130">List the directory roles that are activated in the tenant.</span></span> |
|[<span data-ttu-id="ed1bf-131">Добавление элемента</span><span class="sxs-lookup"><span data-stu-id="ed1bf-131">Add member</span></span>](../api/directoryrole-post-members.md) |[<span data-ttu-id="ed1bf-132">directoryObject</span><span class="sxs-lookup"><span data-stu-id="ed1bf-132">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="ed1bf-133">Добавление пользователя в роль каталога путем записи данных в свойство навигации members.</span><span class="sxs-lookup"><span data-stu-id="ed1bf-133">Add a user to the directory role by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="ed1bf-134">Список членов</span><span class="sxs-lookup"><span data-stu-id="ed1bf-134">List members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="ed1bf-135">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="ed1bf-135">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="ed1bf-136">Получение пользователей, которые относятся к членам роли каталога, из свойства навигации members.</span><span class="sxs-lookup"><span data-stu-id="ed1bf-136">Get the users that are members of the directory role from the members navigation property.</span></span>|
|[<span data-ttu-id="ed1bf-137">Удаление члена</span><span class="sxs-lookup"><span data-stu-id="ed1bf-137">Remove a member</span></span>](../api/directoryrole-delete-member.md) |[<span data-ttu-id="ed1bf-138">directoryObject</span><span class="sxs-lookup"><span data-stu-id="ed1bf-138">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="ed1bf-139">Удаление ресурса user из роли каталога.</span><span class="sxs-lookup"><span data-stu-id="ed1bf-139">Remove a user from the directory role.</span></span>|
|[<span data-ttu-id="ed1bf-140">Активация directoryRole</span><span class="sxs-lookup"><span data-stu-id="ed1bf-140">Activate directoryRole</span></span>](../api/directoryrole-post-directoryroles.md) |[<span data-ttu-id="ed1bf-141">directoryRole</span><span class="sxs-lookup"><span data-stu-id="ed1bf-141">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="ed1bf-142">Активация роли каталога.</span><span class="sxs-lookup"><span data-stu-id="ed1bf-142">Activate a directory role.</span></span>|
|[<span data-ttu-id="ed1bf-143">delta</span><span class="sxs-lookup"><span data-stu-id="ed1bf-143">delta</span></span>](../api/directoryrole-delta.md)|<span data-ttu-id="ed1bf-144">Коллекция объектов directoryRole</span><span class="sxs-lookup"><span data-stu-id="ed1bf-144">directoryRole collection</span></span>| <span data-ttu-id="ed1bf-145">Получите добавочные изменения для каталога ролей.</span><span class="sxs-lookup"><span data-stu-id="ed1bf-145">Get incremental changes for directory roles.</span></span> |

## <a name="properties"></a><span data-ttu-id="ed1bf-146">Свойства</span><span class="sxs-lookup"><span data-stu-id="ed1bf-146">Properties</span></span>
| <span data-ttu-id="ed1bf-147">Свойство</span><span class="sxs-lookup"><span data-stu-id="ed1bf-147">Property</span></span>   | <span data-ttu-id="ed1bf-148">Тип</span><span class="sxs-lookup"><span data-stu-id="ed1bf-148">Type</span></span> | <span data-ttu-id="ed1bf-149">Описание</span><span class="sxs-lookup"><span data-stu-id="ed1bf-149">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="ed1bf-150">описание</span><span class="sxs-lookup"><span data-stu-id="ed1bf-150">description</span></span>|<span data-ttu-id="ed1bf-151">String</span><span class="sxs-lookup"><span data-stu-id="ed1bf-151">String</span></span>|<span data-ttu-id="ed1bf-p103">Описание роли каталога. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ed1bf-p103">The description for the directory role. Read-only.</span></span> |
|<span data-ttu-id="ed1bf-154">displayName</span><span class="sxs-lookup"><span data-stu-id="ed1bf-154">displayName</span></span>|<span data-ttu-id="ed1bf-155">String</span><span class="sxs-lookup"><span data-stu-id="ed1bf-155">String</span></span>|<span data-ttu-id="ed1bf-p104">Отображаемое имя роли каталога. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ed1bf-p104">The display name for the directory role. Read-only.</span></span> |
|<span data-ttu-id="ed1bf-158">id</span><span class="sxs-lookup"><span data-stu-id="ed1bf-158">id</span></span>|<span data-ttu-id="ed1bf-159">String</span><span class="sxs-lookup"><span data-stu-id="ed1bf-159">String</span></span>|<span data-ttu-id="ed1bf-p105">Уникальный идентификатор роли каталога. Наследуется из [directoryObject](directoryobject.md). Ключ, значение null не допускается, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ed1bf-p105">The unique identifier for the directory role. Inherited from [directoryObject](directoryobject.md). Key, Not nullable, Read-only.</span></span>|
|<span data-ttu-id="ed1bf-163">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="ed1bf-163">roleTemplateId</span></span>|<span data-ttu-id="ed1bf-164">String</span><span class="sxs-lookup"><span data-stu-id="ed1bf-164">String</span></span>| <span data-ttu-id="ed1bf-p106">Свойство **id** ресурса [directoryRoleTemplate](directoryroletemplate.md), определяющего значения свойств для этой роли. При активации роли каталога на клиенте следует указать свойство с помощью операции POST. После активации роли каталога свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ed1bf-p106">The **id** of the [directoryRoleTemplate](directoryroletemplate.md) that this role is based on. The property must be specified when activating a directory role in a tenant with a POST operation. After the directory role has been activated, the property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="ed1bf-168">Связи</span><span class="sxs-lookup"><span data-stu-id="ed1bf-168">Relationships</span></span>
| <span data-ttu-id="ed1bf-169">Связь</span><span class="sxs-lookup"><span data-stu-id="ed1bf-169">Relationship</span></span> | <span data-ttu-id="ed1bf-170">Тип</span><span class="sxs-lookup"><span data-stu-id="ed1bf-170">Type</span></span> |<span data-ttu-id="ed1bf-171">Описание</span><span class="sxs-lookup"><span data-stu-id="ed1bf-171">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ed1bf-172">members</span><span class="sxs-lookup"><span data-stu-id="ed1bf-172">members</span></span>|<span data-ttu-id="ed1bf-173">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="ed1bf-173">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="ed1bf-p107">Пользователи, которые относятся к членам этой роли каталога. Методы HTTP: GET, POST, DELETE. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="ed1bf-p107">Users that are members of this directory role. HTTP Methods: GET, POST, DELETE. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ed1bf-178">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ed1bf-178">JSON representation</span></span>

<span data-ttu-id="ed1bf-179">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ed1bf-179">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [
    "memberOf",
    "members",
    "ownedObjects",
    "owners"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.directoryRole",
  "@odata.annotations": [
    {
      "capabilities": {
        "toppable": false
      }
    }
  ]
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
  "roleTemplateId": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
