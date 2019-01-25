---
title: Тип ресурса directoryRole
description: Представляет роль каталога Azure AD. Роли каталога Azure AD также известны как *роли администратора*. Для получения дополнительных сведений о ролях каталога (администратора) см. статью Назначение ролей администратора в Azure AD. С помощью Microsoft Graph можно назначать пользователям роли каталога, чтобы предоставить им разрешения целевой роли. Чтобы можно было считать роль каталога или обновить ее членов, сначала следует активировать ее на клиенте. По умолчанию активируется только роль каталога администраторов организации. Чтобы активировать остальные доступные роли каталога, следует отправить запрос POST с идентификатором ресурса directoryRoleTemplate, определяющего значения свойств для роли каталога. Наследуется из directoryObject.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 30b22313da70c33bffc0b759f9b474f4deac2ac1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521252"
---
# <a name="directoryrole-resource-type"></a><span data-ttu-id="9ebce-110">Тип ресурса directoryRole</span><span class="sxs-lookup"><span data-stu-id="9ebce-110">directoryRole resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ebce-p102">Представляет роль каталога Azure AD. Роли каталога Azure AD также известны как *роли администратора*. Для получения дополнительных сведений о ролях каталога (администратора) см. статью [Назначение ролей администратора в Azure AD](https://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/). С помощью Microsoft Graph можно назначать пользователям роли каталога, чтобы предоставить им разрешения целевой роли. Чтобы можно было считать роль каталога или обновить ее членов, сначала следует активировать ее на клиенте. По умолчанию активируется только роль каталога администраторов организации. Чтобы активировать остальные доступные роли каталога, следует отправить запрос POST с идентификатором ресурса [directoryRoleTemplate](directoryroletemplate.md), определяющего значения свойств для роли каталога. Наследуется из [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="9ebce-p102">Represents an Azure AD directory role. Azure AD directory roles are also known as *administrator roles*. For more information about directory (administrator) roles, see [Assigning administrator roles in Azure AD](https://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/). With the Microsoft Graph, you can assign users to directory roles to grant them the permissions of the target role. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators directory role is activated by default. To activate other available directory roles, you send a POST request with the ID of the [directoryRoleTemplate](directoryroletemplate.md) on which the directory role is based. Inherits from [directoryObject](directoryobject.md).</span></span>

<span data-ttu-id="9ebce-119">По умолчанию каталог роли распространяются всей клиента.</span><span class="sxs-lookup"><span data-stu-id="9ebce-119">By default, directory roles are scoped to be tenant-wide.</span></span>  <span data-ttu-id="9ebce-120">Тем не менее каталог роли (в настоящее время только *администратора учетной записи пользователя* и *администратора служба технической поддержки*) может также областью действия [администратора единиц измерения](administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="9ebce-120">However, directory roles (currently only the *user account admin* and *helpdesk admin*) may also be scoped to [administrative units](administrativeunit.md).</span></span>

<span data-ttu-id="9ebce-121">Этот ресурс поддерживает:</span><span class="sxs-lookup"><span data-stu-id="9ebce-121">This resource supports:</span></span>

- <span data-ttu-id="9ebce-122">отслеживание дополнений, удалений и обновлений с помощью [запроса изменений](/graph/delta-query-overview) (функция [delta](../api/directoryrole-delta.md)).</span><span class="sxs-lookup"><span data-stu-id="9ebce-122">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryrole-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="9ebce-123">Методы</span><span class="sxs-lookup"><span data-stu-id="9ebce-123">Methods</span></span>

| <span data-ttu-id="9ebce-124">Метод</span><span class="sxs-lookup"><span data-stu-id="9ebce-124">Method</span></span>       | <span data-ttu-id="9ebce-125">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9ebce-125">Return Type</span></span>  |<span data-ttu-id="9ebce-126">Описание</span><span class="sxs-lookup"><span data-stu-id="9ebce-126">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9ebce-127">Получение directoryRole</span><span class="sxs-lookup"><span data-stu-id="9ebce-127">Get directoryRole</span></span>](../api/directoryrole-get.md) | [<span data-ttu-id="9ebce-128">directoryRole</span><span class="sxs-lookup"><span data-stu-id="9ebce-128">directoryRole</span></span>](directoryrole.md) |<span data-ttu-id="9ebce-129">Считывание свойств и отношений объекта directoryRole.</span><span class="sxs-lookup"><span data-stu-id="9ebce-129">Read properties and relationships of directoryRole object.</span></span>|
|[<span data-ttu-id="9ebce-130">Перечисление объектов directoryRole</span><span class="sxs-lookup"><span data-stu-id="9ebce-130">List directoryRoles</span></span>](../api/directoryrole-list.md) | <span data-ttu-id="9ebce-131">Коллекция объектов [directoryRole](directoryrole.md)</span><span class="sxs-lookup"><span data-stu-id="9ebce-131">[directoryRole](directoryrole.md) collection</span></span> | <span data-ttu-id="9ebce-132">Перечисление ролей каталога, активированных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="9ebce-132">List the directory roles that are activated in the tenant.</span></span> |
|[<span data-ttu-id="9ebce-133">Добавление элемента</span><span class="sxs-lookup"><span data-stu-id="9ebce-133">Add member</span></span>](../api/directoryrole-post-members.md) |[<span data-ttu-id="9ebce-134">directoryObject</span><span class="sxs-lookup"><span data-stu-id="9ebce-134">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="9ebce-135">Добавление пользователя в роль каталога путем записи данных в свойство навигации members.</span><span class="sxs-lookup"><span data-stu-id="9ebce-135">Add a user to the directory role by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="9ebce-136">Список членов</span><span class="sxs-lookup"><span data-stu-id="9ebce-136">List members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="9ebce-137">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="9ebce-137">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="9ebce-138">Получение пользователей, которые относятся к членам роли каталога, из свойства навигации members.</span><span class="sxs-lookup"><span data-stu-id="9ebce-138">Get the users that are members of the directory role from the members navigation property.</span></span>|
|[<span data-ttu-id="9ebce-139">Удаление члена</span><span class="sxs-lookup"><span data-stu-id="9ebce-139">Remove a member</span></span>](../api/directoryrole-delete-member.md) |[<span data-ttu-id="9ebce-140">directoryObject</span><span class="sxs-lookup"><span data-stu-id="9ebce-140">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="9ebce-141">Удаление ресурса user из роли каталога.</span><span class="sxs-lookup"><span data-stu-id="9ebce-141">Remove a user from the directory role.</span></span>|
|[<span data-ttu-id="9ebce-142">Список элементов области определения роли</span><span class="sxs-lookup"><span data-stu-id="9ebce-142">List scoped-role members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="9ebce-143">[scopedRoleMembership](scopedrolemembership.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="9ebce-143">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="9ebce-144">Список пользователей, которым эта роль каталогов, предназначенные для [администрирования единиц измерения](administrativeunit.md), через коллекцию ресурсов scopedRoleMembership.</span><span class="sxs-lookup"><span data-stu-id="9ebce-144">List the members of this directory role that are scoped to [administrative units](administrativeunit.md), through the scopedRoleMembership resource collection.</span></span>|
|[<span data-ttu-id="9ebce-145">delta</span><span class="sxs-lookup"><span data-stu-id="9ebce-145">delta</span></span>](../api/directoryrole-delta.md)|<span data-ttu-id="9ebce-146">Коллекция объектов directoryRole</span><span class="sxs-lookup"><span data-stu-id="9ebce-146">directoryRole collection</span></span>| <span data-ttu-id="9ebce-147">Получите добавочные изменения для каталога ролей.</span><span class="sxs-lookup"><span data-stu-id="9ebce-147">Get incremental changes for directory roles.</span></span> |

## <a name="properties"></a><span data-ttu-id="9ebce-148">Свойства</span><span class="sxs-lookup"><span data-stu-id="9ebce-148">Properties</span></span>
| <span data-ttu-id="9ebce-149">Свойство</span><span class="sxs-lookup"><span data-stu-id="9ebce-149">Property</span></span>   | <span data-ttu-id="9ebce-150">Тип</span><span class="sxs-lookup"><span data-stu-id="9ebce-150">Type</span></span> |<span data-ttu-id="9ebce-151">Описание</span><span class="sxs-lookup"><span data-stu-id="9ebce-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9ebce-152">description</span><span class="sxs-lookup"><span data-stu-id="9ebce-152">description</span></span>|<span data-ttu-id="9ebce-153">String</span><span class="sxs-lookup"><span data-stu-id="9ebce-153">String</span></span>|<span data-ttu-id="9ebce-p104">Описание роли каталога. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9ebce-p104">The description for the directory role. Read-only.</span></span> |
|<span data-ttu-id="9ebce-156">displayName</span><span class="sxs-lookup"><span data-stu-id="9ebce-156">displayName</span></span>|<span data-ttu-id="9ebce-157">Строка</span><span class="sxs-lookup"><span data-stu-id="9ebce-157">String</span></span>|<span data-ttu-id="9ebce-p105">Отображаемое имя роли каталога. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9ebce-p105">The display name for the directory role. Read-only.</span></span> |
|<span data-ttu-id="9ebce-160">id</span><span class="sxs-lookup"><span data-stu-id="9ebce-160">id</span></span>|<span data-ttu-id="9ebce-161">String</span><span class="sxs-lookup"><span data-stu-id="9ebce-161">String</span></span>|<span data-ttu-id="9ebce-p106">Уникальный идентификатор роли каталога. Наследуется из [directoryObject](directoryobject.md). Ключ, значение null не допускается, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9ebce-p106">The unique identifier for the directory role. Inherited from [directoryObject](directoryobject.md). Key, Not nullable, Read-only.</span></span>|
|<span data-ttu-id="9ebce-165">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="9ebce-165">roleTemplateId</span></span>|<span data-ttu-id="9ebce-166">String</span><span class="sxs-lookup"><span data-stu-id="9ebce-166">String</span></span>| <span data-ttu-id="9ebce-p107">Свойство **id** ресурса [directoryRoleTemplate](directoryroletemplate.md), определяющего значения свойств для этой роли. При активации роли каталога на клиенте следует указать свойство с помощью операции POST. После активации роли каталога свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9ebce-p107">The **id** of the [directoryRoleTemplate](directoryroletemplate.md) that this role is based on. The property must be specified when activating a directory role in a tenant with a POST operation. After the directory role has been activated, the property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="9ebce-170">Связи</span><span class="sxs-lookup"><span data-stu-id="9ebce-170">Relationships</span></span>
| <span data-ttu-id="9ebce-171">Связь</span><span class="sxs-lookup"><span data-stu-id="9ebce-171">Relationship</span></span> | <span data-ttu-id="9ebce-172">Тип</span><span class="sxs-lookup"><span data-stu-id="9ebce-172">Type</span></span> |<span data-ttu-id="9ebce-173">Описание</span><span class="sxs-lookup"><span data-stu-id="9ebce-173">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9ebce-174">members</span><span class="sxs-lookup"><span data-stu-id="9ebce-174">members</span></span>|<span data-ttu-id="9ebce-175">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="9ebce-175">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="9ebce-p108">Пользователи, которые относятся к членам этой роли каталога. Методы HTTP: GET, POST, DELETE. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="9ebce-p108">Users that are members of this directory role. HTTP Methods: GET, POST, DELETE. Read-only. Nullable.</span></span>|
|<span data-ttu-id="9ebce-180">scopedMembers</span><span class="sxs-lookup"><span data-stu-id="9ebce-180">scopedMembers</span></span>|<span data-ttu-id="9ebce-181">[scopedRoleMembership](scopedrolemembership.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="9ebce-181">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="9ebce-182">Члены этой роли каталога, предназначенные для [администрирования единиц измерения](administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="9ebce-182">Members of this directory role that are scoped to [administrative units](administrativeunit.md).</span></span> <span data-ttu-id="9ebce-183">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9ebce-183">Read-only.</span></span> <span data-ttu-id="9ebce-184">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="9ebce-184">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9ebce-185">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9ebce-185">JSON representation</span></span>

<span data-ttu-id="9ebce-186">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9ebce-186">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "memberOf",
    "members",
    "ownedObjects",
    "owners"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryRole"
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
<!--
{
  "type": "#page.annotation",
  "description": "directoryRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/directoryrole.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
