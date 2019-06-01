---
title: Тип ресурса directoryRole
description: Представляет роль каталога Azure AD. Роли каталога Azure AD также известны как *роли администратора*. Для получения дополнительных сведений о ролях каталога (администратора) см. статью "Назначение ролей администратора в Azure AD". С помощью Microsoft Graph можно назначать пользователям роли каталога, чтобы предоставить им разрешения целевой роли. Чтобы можно было считать роль каталога или обновить ее членов, сначала следует активировать ее на клиенте. По умолчанию активируется только роль каталога администраторов организации. Чтобы активировать другие доступные роли каталога, отправьте запрос POST с ИДЕНТИФИКАТОРом directoryRoleTemplate, на котором основана роль каталога. Наследуется от directoryObject.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ac9b08e2e39bce6a20703089d6bfe69c8b25f55f
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657905"
---
# <a name="directoryrole-resource-type"></a><span data-ttu-id="19710-110">Тип ресурса directoryRole</span><span class="sxs-lookup"><span data-stu-id="19710-110">directoryRole resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19710-111">Представляет роль каталога Azure AD.</span><span class="sxs-lookup"><span data-stu-id="19710-111">Represents an Azure AD directory role.</span></span> <span data-ttu-id="19710-112">Роли каталога Azure AD также известны как *роли администратора*.</span><span class="sxs-lookup"><span data-stu-id="19710-112">Azure AD directory roles are also known as *administrator roles*.</span></span> <span data-ttu-id="19710-113">Для получения дополнительных сведений о ролях каталога (администратора) см. статью [Назначение ролей администратора в Azure AD](https://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/).</span><span class="sxs-lookup"><span data-stu-id="19710-113">For more information about directory (administrator) roles, see [Assigning administrator roles in Azure AD](https://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/).</span></span> <span data-ttu-id="19710-114">С помощью Microsoft Graph можно назначать пользователям роли каталога, чтобы предоставить им разрешения целевой роли.</span><span class="sxs-lookup"><span data-stu-id="19710-114">With the Microsoft Graph, you can assign users to directory roles to grant them the permissions of the target role.</span></span> <span data-ttu-id="19710-115">Чтобы можно было считать роль каталога или обновить ее членов, сначала следует активировать ее на клиенте.</span><span class="sxs-lookup"><span data-stu-id="19710-115">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="19710-116">По умолчанию активируется только роль каталога администраторов организации.</span><span class="sxs-lookup"><span data-stu-id="19710-116">Only the Company Administrators directory role is activated by default.</span></span> <span data-ttu-id="19710-117">Чтобы активировать другие доступные роли каталога, отправьте запрос POST с ИДЕНТИФИКАТОРом [directoryRoleTemplate](directoryroletemplate.md) , на котором основана роль каталога.</span><span class="sxs-lookup"><span data-stu-id="19710-117">To activate other available directory roles, you send a POST request with the ID of the [directoryRoleTemplate](directoryroletemplate.md) on which the directory role is based.</span></span> <span data-ttu-id="19710-118">Наследуется от [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="19710-118">Inherits from [directoryObject](directoryobject.md).</span></span>

<span data-ttu-id="19710-119">По умолчанию роли каталога разделяются на уровне клиента.</span><span class="sxs-lookup"><span data-stu-id="19710-119">By default, directory roles are scoped to be tenant-wide.</span></span>  <span data-ttu-id="19710-120">Однако роли каталогов (в настоящее время только *Администратор учетной записи пользователя* и *администратор службы поддержки*) также могут быть ограничены [административными единицами](administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="19710-120">However, directory roles (currently only the *user account admin* and *helpdesk admin*) may also be scoped to [administrative units](administrativeunit.md).</span></span>

<span data-ttu-id="19710-121">Этот ресурс поддерживает:</span><span class="sxs-lookup"><span data-stu-id="19710-121">This resource supports:</span></span>

- <span data-ttu-id="19710-122">отслеживание дополнений, удалений и обновлений с помощью [запроса изменений](/graph/delta-query-overview) (функция [delta](../api/directoryrole-delta.md)).</span><span class="sxs-lookup"><span data-stu-id="19710-122">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryrole-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="19710-123">Методы</span><span class="sxs-lookup"><span data-stu-id="19710-123">Methods</span></span>

| <span data-ttu-id="19710-124">Метод</span><span class="sxs-lookup"><span data-stu-id="19710-124">Method</span></span>       | <span data-ttu-id="19710-125">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="19710-125">Return Type</span></span>  |<span data-ttu-id="19710-126">Описание</span><span class="sxs-lookup"><span data-stu-id="19710-126">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="19710-127">Получение directoryRole</span><span class="sxs-lookup"><span data-stu-id="19710-127">Get directoryRole</span></span>](../api/directoryrole-get.md) | [<span data-ttu-id="19710-128">directoryRole</span><span class="sxs-lookup"><span data-stu-id="19710-128">directoryRole</span></span>](directoryrole.md) |<span data-ttu-id="19710-129">Считывание свойств и отношений объекта directoryRole.</span><span class="sxs-lookup"><span data-stu-id="19710-129">Read properties and relationships of directoryRole object.</span></span>|
|[<span data-ttu-id="19710-130">Перечисление объектов directoryRole</span><span class="sxs-lookup"><span data-stu-id="19710-130">List directoryRoles</span></span>](../api/directoryrole-list.md) | <span data-ttu-id="19710-131">Коллекция объектов [directoryRole](directoryrole.md)</span><span class="sxs-lookup"><span data-stu-id="19710-131">[directoryRole](directoryrole.md) collection</span></span> | <span data-ttu-id="19710-132">Перечисление ролей каталога, активированных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="19710-132">List the directory roles that are activated in the tenant.</span></span> |
|[<span data-ttu-id="19710-133">Добавление элемента</span><span class="sxs-lookup"><span data-stu-id="19710-133">Add member</span></span>](../api/directoryrole-post-members.md) |[<span data-ttu-id="19710-134">directoryObject</span><span class="sxs-lookup"><span data-stu-id="19710-134">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="19710-135">Добавление пользователя в роль каталога путем записи данных в свойство навигации members.</span><span class="sxs-lookup"><span data-stu-id="19710-135">Add a user to the directory role by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="19710-136">Список членов</span><span class="sxs-lookup"><span data-stu-id="19710-136">List members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="19710-137">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="19710-137">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="19710-138">Получение пользователей, которые относятся к членам роли каталога, из свойства навигации members.</span><span class="sxs-lookup"><span data-stu-id="19710-138">Get the users that are members of the directory role from the members navigation property.</span></span>|
|[<span data-ttu-id="19710-139">Удаление члена</span><span class="sxs-lookup"><span data-stu-id="19710-139">Remove a member</span></span>](../api/directoryrole-delete-member.md) |[<span data-ttu-id="19710-140">directoryObject</span><span class="sxs-lookup"><span data-stu-id="19710-140">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="19710-141">Удаление ресурса user из роли каталога.</span><span class="sxs-lookup"><span data-stu-id="19710-141">Remove a user from the directory role.</span></span>|
|[<span data-ttu-id="19710-142">Область списка — элементы роли</span><span class="sxs-lookup"><span data-stu-id="19710-142">List scoped-role members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="19710-143">Коллекция [scopedRoleMembership](scopedrolemembership.md)</span><span class="sxs-lookup"><span data-stu-id="19710-143">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="19710-144">Перечислите членов этой роли каталога, область действия которой ограничена [административными единицами](administrativeunit.md), с помощью коллекции ресурсов scopedrolemembership изменен.</span><span class="sxs-lookup"><span data-stu-id="19710-144">List the members of this directory role that are scoped to [administrative units](administrativeunit.md), through the scopedRoleMembership resource collection.</span></span>|
|[<span data-ttu-id="19710-145">delta</span><span class="sxs-lookup"><span data-stu-id="19710-145">delta</span></span>](../api/directoryrole-delta.md)|<span data-ttu-id="19710-146">Коллекция объектов directoryRole</span><span class="sxs-lookup"><span data-stu-id="19710-146">directoryRole collection</span></span>| <span data-ttu-id="19710-147">Получение добавочных изменений для ролей каталога.</span><span class="sxs-lookup"><span data-stu-id="19710-147">Get incremental changes for directory roles.</span></span> |

## <a name="properties"></a><span data-ttu-id="19710-148">Свойства</span><span class="sxs-lookup"><span data-stu-id="19710-148">Properties</span></span>
| <span data-ttu-id="19710-149">Свойство</span><span class="sxs-lookup"><span data-stu-id="19710-149">Property</span></span>   | <span data-ttu-id="19710-150">Тип</span><span class="sxs-lookup"><span data-stu-id="19710-150">Type</span></span> |<span data-ttu-id="19710-151">Описание</span><span class="sxs-lookup"><span data-stu-id="19710-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="19710-152">description</span><span class="sxs-lookup"><span data-stu-id="19710-152">description</span></span>|<span data-ttu-id="19710-153">String</span><span class="sxs-lookup"><span data-stu-id="19710-153">String</span></span>|<span data-ttu-id="19710-p104">Описание роли каталога. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="19710-p104">The description for the directory role. Read-only.</span></span> |
|<span data-ttu-id="19710-156">displayName</span><span class="sxs-lookup"><span data-stu-id="19710-156">displayName</span></span>|<span data-ttu-id="19710-157">Строка</span><span class="sxs-lookup"><span data-stu-id="19710-157">String</span></span>|<span data-ttu-id="19710-p105">Отображаемое имя роли каталога. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="19710-p105">The display name for the directory role. Read-only.</span></span> |
|<span data-ttu-id="19710-160">id</span><span class="sxs-lookup"><span data-stu-id="19710-160">id</span></span>|<span data-ttu-id="19710-161">Строка</span><span class="sxs-lookup"><span data-stu-id="19710-161">String</span></span>|<span data-ttu-id="19710-p106">Уникальный идентификатор роли каталога. Наследуется из [directoryObject](directoryobject.md). Ключ, значение null не допускается, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="19710-p106">The unique identifier for the directory role. Inherited from [directoryObject](directoryobject.md). Key, Not nullable, Read-only.</span></span>|
|<span data-ttu-id="19710-165">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="19710-165">roleTemplateId</span></span>|<span data-ttu-id="19710-166">String</span><span class="sxs-lookup"><span data-stu-id="19710-166">String</span></span>| <span data-ttu-id="19710-p107">Свойство **id** ресурса [directoryRoleTemplate](directoryroletemplate.md), определяющего значения свойств для этой роли. При активации роли каталога на клиенте следует указать свойство с помощью операции POST. После активации роли каталога свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="19710-p107">The **id** of the [directoryRoleTemplate](directoryroletemplate.md) that this role is based on. The property must be specified when activating a directory role in a tenant with a POST operation. After the directory role has been activated, the property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="19710-170">Связи</span><span class="sxs-lookup"><span data-stu-id="19710-170">Relationships</span></span>
| <span data-ttu-id="19710-171">Отношение</span><span class="sxs-lookup"><span data-stu-id="19710-171">Relationship</span></span> | <span data-ttu-id="19710-172">Тип</span><span class="sxs-lookup"><span data-stu-id="19710-172">Type</span></span> |<span data-ttu-id="19710-173">Описание</span><span class="sxs-lookup"><span data-stu-id="19710-173">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="19710-174">members</span><span class="sxs-lookup"><span data-stu-id="19710-174">members</span></span>|<span data-ttu-id="19710-175">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="19710-175">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="19710-p108">Пользователи, которые относятся к членам этой роли каталога. Методы HTTP: GET, POST, DELETE. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="19710-p108">Users that are members of this directory role. HTTP Methods: GET, POST, DELETE. Read-only. Nullable.</span></span>|
|<span data-ttu-id="19710-180">Scopedadministrators</span><span class="sxs-lookup"><span data-stu-id="19710-180">scopedMembers</span></span>|<span data-ttu-id="19710-181">Коллекция [scopedRoleMembership](scopedrolemembership.md)</span><span class="sxs-lookup"><span data-stu-id="19710-181">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="19710-182">Члены этой роли каталога, областью действия которой являются [административные единицы](administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="19710-182">Members of this directory role that are scoped to [administrative units](administrativeunit.md).</span></span> <span data-ttu-id="19710-183">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="19710-183">Read-only.</span></span> <span data-ttu-id="19710-184">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="19710-184">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="19710-185">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="19710-185">JSON representation</span></span>

<span data-ttu-id="19710-186">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="19710-186">Here is a JSON representation of the resource</span></span>

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
