---
title: Тип ресурса directoryRole
description: Представляет роль каталога Azure AD. Роли каталога Azure AD также известны как *роли администратора*. Дополнительные сведения о ролях каталогов (администратора) см. в разделе Назначение ролей администратора в Azure AD. С помощью Microsoft Graph вы можете назначить пользователям роли каталога, чтобы предоставить им разрешения целевой роли. Чтобы можно было считать роль каталога или обновить ее членов, сначала следует активировать ее на клиенте. По умолчанию активирована только роль каталога администраторов компании. Чтобы активировать другие доступные роли каталога, отправьте запрос POST с ИДЕНТИФИКАТОРом directoryRoleTemplate, на котором основана роль каталога. Наследуется от directoryObject.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 110febf3213431a0a44941a4cdd2bd9bca255bff
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334602"
---
# <a name="directoryrole-resource-type"></a><span data-ttu-id="34b78-110">Тип ресурса directoryRole</span><span class="sxs-lookup"><span data-stu-id="34b78-110">directoryRole resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="34b78-111">Представляет роль каталога Azure AD.</span><span class="sxs-lookup"><span data-stu-id="34b78-111">Represents an Azure AD directory role.</span></span> <span data-ttu-id="34b78-112">Роли каталога Azure AD также известны как *роли администратора*.</span><span class="sxs-lookup"><span data-stu-id="34b78-112">Azure AD directory roles are also known as *administrator roles*.</span></span> <span data-ttu-id="34b78-113">Дополнительные сведения о ролях каталогов (администратора) см. [в разделе Назначение ролей администратора в Azure AD](https://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/).</span><span class="sxs-lookup"><span data-stu-id="34b78-113">For more information about directory (administrator) roles, see [Assigning administrator roles in Azure AD](https://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/).</span></span> <span data-ttu-id="34b78-114">С помощью Microsoft Graph вы можете назначить пользователям роли каталога, чтобы предоставить им разрешения целевой роли.</span><span class="sxs-lookup"><span data-stu-id="34b78-114">With the Microsoft Graph, you can assign users to directory roles to grant them the permissions of the target role.</span></span> <span data-ttu-id="34b78-115">Чтобы можно было считать роль каталога или обновить ее членов, сначала следует активировать ее на клиенте.</span><span class="sxs-lookup"><span data-stu-id="34b78-115">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="34b78-116">По умолчанию активирована только роль каталога администраторов компании.</span><span class="sxs-lookup"><span data-stu-id="34b78-116">Only the Company Administrators directory role is activated by default.</span></span> <span data-ttu-id="34b78-117">Чтобы активировать другие доступные роли каталога, отправьте запрос POST с ИДЕНТИФИКАТОРом [directoryRoleTemplate](directoryroletemplate.md) , на котором основана роль каталога.</span><span class="sxs-lookup"><span data-stu-id="34b78-117">To activate other available directory roles, you send a POST request with the ID of the [directoryRoleTemplate](directoryroletemplate.md) on which the directory role is based.</span></span> <span data-ttu-id="34b78-118">Наследуется от [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="34b78-118">Inherits from [directoryObject](directoryobject.md).</span></span>

<span data-ttu-id="34b78-119">По умолчанию роли каталога разделяются на уровне клиента.</span><span class="sxs-lookup"><span data-stu-id="34b78-119">By default, directory roles are scoped to be tenant-wide.</span></span>  <span data-ttu-id="34b78-120">Однако роли каталогов (в настоящее время только *Администратор учетной записи пользователя* и *администратор службы поддержки*) также могут быть ограничены [административными единицами](administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="34b78-120">However, directory roles (currently only the *user account admin* and *helpdesk admin*) may also be scoped to [administrative units](administrativeunit.md).</span></span>

<span data-ttu-id="34b78-121">Этот ресурс поддерживает:</span><span class="sxs-lookup"><span data-stu-id="34b78-121">This resource supports:</span></span>

- <span data-ttu-id="34b78-122">отслеживание дополнений, удалений и обновлений с помощью [запроса изменений](/graph/delta-query-overview) (функция [delta](../api/directoryrole-delta.md)).</span><span class="sxs-lookup"><span data-stu-id="34b78-122">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryrole-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="34b78-123">Методы</span><span class="sxs-lookup"><span data-stu-id="34b78-123">Methods</span></span>

| <span data-ttu-id="34b78-124">Метод</span><span class="sxs-lookup"><span data-stu-id="34b78-124">Method</span></span>       | <span data-ttu-id="34b78-125">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="34b78-125">Return Type</span></span>  |<span data-ttu-id="34b78-126">Описание</span><span class="sxs-lookup"><span data-stu-id="34b78-126">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="34b78-127">Получение directoryRole</span><span class="sxs-lookup"><span data-stu-id="34b78-127">Get directoryRole</span></span>](../api/directoryrole-get.md) | [<span data-ttu-id="34b78-128">directoryRole</span><span class="sxs-lookup"><span data-stu-id="34b78-128">directoryRole</span></span>](directoryrole.md) |<span data-ttu-id="34b78-129">Считывание свойств и отношений объекта directoryRole.</span><span class="sxs-lookup"><span data-stu-id="34b78-129">Read properties and relationships of directoryRole object.</span></span>|
|[<span data-ttu-id="34b78-130">Список перечисление directoryrole</span><span class="sxs-lookup"><span data-stu-id="34b78-130">List directoryRoles</span></span>](../api/directoryrole-list.md) | <span data-ttu-id="34b78-131">Коллекция объектов [directoryRole](directoryrole.md)</span><span class="sxs-lookup"><span data-stu-id="34b78-131">[directoryRole](directoryrole.md) collection</span></span> | <span data-ttu-id="34b78-132">Список ролей каталога, активированных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="34b78-132">List the directory roles that are activated in the tenant.</span></span> |
|[<span data-ttu-id="34b78-133">Добавление участника</span><span class="sxs-lookup"><span data-stu-id="34b78-133">Add member</span></span>](../api/directoryrole-post-members.md) |[<span data-ttu-id="34b78-134">directoryObject</span><span class="sxs-lookup"><span data-stu-id="34b78-134">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="34b78-135">Добавление пользователя в роль каталога путем записи данных в свойство навигации members.</span><span class="sxs-lookup"><span data-stu-id="34b78-135">Add a user to the directory role by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="34b78-136">Перечисление участников</span><span class="sxs-lookup"><span data-stu-id="34b78-136">List members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="34b78-137">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="34b78-137">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="34b78-138">Получение пользователей, которые относятся к членам роли каталога, из свойства навигации members.</span><span class="sxs-lookup"><span data-stu-id="34b78-138">Get the users that are members of the directory role from the members navigation property.</span></span>|
|[<span data-ttu-id="34b78-139">Удаление участника</span><span class="sxs-lookup"><span data-stu-id="34b78-139">Remove a member</span></span>](../api/directoryrole-delete-member.md) |[<span data-ttu-id="34b78-140">directoryObject</span><span class="sxs-lookup"><span data-stu-id="34b78-140">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="34b78-141">Удаление пользователя из роли каталога.</span><span class="sxs-lookup"><span data-stu-id="34b78-141">Remove a user from the directory role.</span></span>|
|[<span data-ttu-id="34b78-142">Область списка — элементы роли</span><span class="sxs-lookup"><span data-stu-id="34b78-142">List scoped-role members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="34b78-143">Коллекция [scopedRoleMembership](scopedrolemembership.md)</span><span class="sxs-lookup"><span data-stu-id="34b78-143">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="34b78-144">ПереЧислите членов этой роли каталога, область действия которой ограничена [административными единицами](administrativeunit.md), с помощью коллекции ресурсов scopedrolemembership изменен.</span><span class="sxs-lookup"><span data-stu-id="34b78-144">List the members of this directory role that are scoped to [administrative units](administrativeunit.md), through the scopedRoleMembership resource collection.</span></span>|
|[<span data-ttu-id="34b78-145">delta</span><span class="sxs-lookup"><span data-stu-id="34b78-145">delta</span></span>](../api/directoryrole-delta.md)|<span data-ttu-id="34b78-146">Коллекция объектов directoryRole</span><span class="sxs-lookup"><span data-stu-id="34b78-146">directoryRole collection</span></span>| <span data-ttu-id="34b78-147">Получение добавочных изменений для ролей каталога.</span><span class="sxs-lookup"><span data-stu-id="34b78-147">Get incremental changes for directory roles.</span></span> |

## <a name="properties"></a><span data-ttu-id="34b78-148">Свойства</span><span class="sxs-lookup"><span data-stu-id="34b78-148">Properties</span></span>
| <span data-ttu-id="34b78-149">Свойство</span><span class="sxs-lookup"><span data-stu-id="34b78-149">Property</span></span>   | <span data-ttu-id="34b78-150">Тип</span><span class="sxs-lookup"><span data-stu-id="34b78-150">Type</span></span> |<span data-ttu-id="34b78-151">Описание</span><span class="sxs-lookup"><span data-stu-id="34b78-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="34b78-152">description</span><span class="sxs-lookup"><span data-stu-id="34b78-152">description</span></span>|<span data-ttu-id="34b78-153">String</span><span class="sxs-lookup"><span data-stu-id="34b78-153">String</span></span>|<span data-ttu-id="34b78-p104">Описание роли каталога. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="34b78-p104">The description for the directory role. Read-only.</span></span> |
|<span data-ttu-id="34b78-156">displayName</span><span class="sxs-lookup"><span data-stu-id="34b78-156">displayName</span></span>|<span data-ttu-id="34b78-157">Строка</span><span class="sxs-lookup"><span data-stu-id="34b78-157">String</span></span>|<span data-ttu-id="34b78-p105">Отображаемое имя роли каталога. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="34b78-p105">The display name for the directory role. Read-only.</span></span> |
|<span data-ttu-id="34b78-160">id</span><span class="sxs-lookup"><span data-stu-id="34b78-160">id</span></span>|<span data-ttu-id="34b78-161">Строка</span><span class="sxs-lookup"><span data-stu-id="34b78-161">String</span></span>|<span data-ttu-id="34b78-p106">Уникальный идентификатор роли каталога. Наследуется из [directoryObject](directoryobject.md). Ключ, значение null не допускается, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="34b78-p106">The unique identifier for the directory role. Inherited from [directoryObject](directoryobject.md). Key, Not nullable, Read-only.</span></span>|
|<span data-ttu-id="34b78-165">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="34b78-165">roleTemplateId</span></span>|<span data-ttu-id="34b78-166">String</span><span class="sxs-lookup"><span data-stu-id="34b78-166">String</span></span>| <span data-ttu-id="34b78-p107">Свойство **id** ресурса [directoryRoleTemplate](directoryroletemplate.md), определяющего значения свойств для этой роли. При активации роли каталога на клиенте следует указать свойство с помощью операции POST. После активации роли каталога свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="34b78-p107">The **id** of the [directoryRoleTemplate](directoryroletemplate.md) that this role is based on. The property must be specified when activating a directory role in a tenant with a POST operation. After the directory role has been activated, the property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="34b78-170">Отношения</span><span class="sxs-lookup"><span data-stu-id="34b78-170">Relationships</span></span>
| <span data-ttu-id="34b78-171">Отношение</span><span class="sxs-lookup"><span data-stu-id="34b78-171">Relationship</span></span> | <span data-ttu-id="34b78-172">Тип</span><span class="sxs-lookup"><span data-stu-id="34b78-172">Type</span></span> |<span data-ttu-id="34b78-173">Описание</span><span class="sxs-lookup"><span data-stu-id="34b78-173">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="34b78-174">members</span><span class="sxs-lookup"><span data-stu-id="34b78-174">members</span></span>|<span data-ttu-id="34b78-175">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="34b78-175">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="34b78-p108">Пользователи, которые относятся к членам этой роли каталога. Методы HTTP: GET, POST, DELETE. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="34b78-p108">Users that are members of this directory role. HTTP Methods: GET, POST, DELETE. Read-only. Nullable.</span></span>|
|<span data-ttu-id="34b78-180">Scopedadministrators</span><span class="sxs-lookup"><span data-stu-id="34b78-180">scopedMembers</span></span>|<span data-ttu-id="34b78-181">Коллекция [scopedRoleMembership](scopedrolemembership.md)</span><span class="sxs-lookup"><span data-stu-id="34b78-181">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="34b78-182">Члены этой роли каталога, областью действия которой являются [административные единицы](administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="34b78-182">Members of this directory role that are scoped to [administrative units](administrativeunit.md).</span></span> <span data-ttu-id="34b78-183">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="34b78-183">Read-only.</span></span> <span data-ttu-id="34b78-184">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="34b78-184">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="34b78-185">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="34b78-185">JSON representation</span></span>

<span data-ttu-id="34b78-186">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="34b78-186">Here is a JSON representation of the resource</span></span>

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
  "suppressions": []
}
-->
