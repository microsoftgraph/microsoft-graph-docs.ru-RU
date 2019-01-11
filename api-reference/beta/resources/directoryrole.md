---
title: Тип ресурса directoryRole
description: Представляет роль directory Azure AD. Каталог роли Azure AD также называются *ролями администратора*. Дополнительные сведения о ролях каталогов (администратор) в разделе назначение ролей администратора в Azure AD. Microsoft Graph можно назначить роли каталог, чтобы предоставлять им разрешения целевой роли пользователей. Для чтения роли каталога или обновите его члены, необходимо активировать в клиентов. Только роль directory Администраторы организации активируется по умолчанию. Активация других ролей доступных каталогов, отправьте запрос POST с Идентификатором directoryRoleTemplate, лежащие в основе роли каталога. Наследуется от directoryObject.
localization_priority: Normal
ms.openlocfilehash: 30f9b56652d3e4c7ebb1466941930cea0cf12ebf
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876225"
---
# <a name="directoryrole-resource-type"></a><span data-ttu-id="da3b8-110">Тип ресурса directoryRole</span><span class="sxs-lookup"><span data-stu-id="da3b8-110">directoryRole resource type</span></span>

> <span data-ttu-id="da3b8-111">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="da3b8-111">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="da3b8-112">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="da3b8-112">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="da3b8-113">Представляет роль directory Azure AD.</span><span class="sxs-lookup"><span data-stu-id="da3b8-113">Represents an Azure AD directory role.</span></span> <span data-ttu-id="da3b8-114">Каталог роли Azure AD также называются *ролями администратора*.</span><span class="sxs-lookup"><span data-stu-id="da3b8-114">Azure AD directory roles are also known as *administrator roles*.</span></span> <span data-ttu-id="da3b8-115">Дополнительные сведения о ролях каталогов (администратор) можно [Назначение ролей администратора в Azure AD](https://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/).</span><span class="sxs-lookup"><span data-stu-id="da3b8-115">For more information about directory (administrator) roles, see [Assigning administrator roles in Azure AD](https://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/).</span></span> <span data-ttu-id="da3b8-116">Microsoft Graph можно назначить роли каталог, чтобы предоставлять им разрешения целевой роли пользователей.</span><span class="sxs-lookup"><span data-stu-id="da3b8-116">With the Microsoft Graph, you can assign users to directory roles to grant them the permissions of the target role.</span></span> <span data-ttu-id="da3b8-117">Для чтения роли каталога или обновите его члены, необходимо активировать в клиентов.</span><span class="sxs-lookup"><span data-stu-id="da3b8-117">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="da3b8-118">Только роль directory Администраторы организации активируется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="da3b8-118">Only the Company Administrators directory role is activated by default.</span></span> <span data-ttu-id="da3b8-119">Активация других ролей доступных каталогов, отправьте запрос POST с Идентификатором [directoryRoleTemplate](directoryroletemplate.md) , лежащие в основе роли каталога.</span><span class="sxs-lookup"><span data-stu-id="da3b8-119">To activate other available directory roles, you send a POST request with the ID of the [directoryRoleTemplate](directoryroletemplate.md) on which the directory role is based.</span></span> <span data-ttu-id="da3b8-120">Наследуется от [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="da3b8-120">Inherits from [directoryObject](directoryobject.md).</span></span>

<span data-ttu-id="da3b8-121">По умолчанию каталог роли распространяются всей клиента.</span><span class="sxs-lookup"><span data-stu-id="da3b8-121">By default, directory roles are scoped to be tenant-wide.</span></span>  <span data-ttu-id="da3b8-122">Тем не менее каталог роли (в настоящее время только *администратора учетной записи пользователя* и *администратора служба технической поддержки*) может также областью действия [администратора единиц измерения](administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="da3b8-122">However, directory roles (currently only the *user account admin* and *helpdesk admin*) may also be scoped to [administrative units](administrativeunit.md).</span></span>

<span data-ttu-id="da3b8-123">Этот ресурс поддерживает:</span><span class="sxs-lookup"><span data-stu-id="da3b8-123">This resource supports:</span></span>

- <span data-ttu-id="da3b8-124">отслеживание дополнений, удалений и обновлений с помощью [запроса изменений](/graph/delta-query-overview) (функция [delta](../api/directoryrole-delta.md)).</span><span class="sxs-lookup"><span data-stu-id="da3b8-124">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryrole-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="da3b8-125">Методы</span><span class="sxs-lookup"><span data-stu-id="da3b8-125">Methods</span></span>

| <span data-ttu-id="da3b8-126">Метод</span><span class="sxs-lookup"><span data-stu-id="da3b8-126">Method</span></span>       | <span data-ttu-id="da3b8-127">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="da3b8-127">Return Type</span></span>  |<span data-ttu-id="da3b8-128">Описание</span><span class="sxs-lookup"><span data-stu-id="da3b8-128">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="da3b8-129">Получение directoryRole</span><span class="sxs-lookup"><span data-stu-id="da3b8-129">Get directoryRole</span></span>](../api/directoryrole-get.md) | [<span data-ttu-id="da3b8-130">directoryRole</span><span class="sxs-lookup"><span data-stu-id="da3b8-130">directoryRole</span></span>](directoryrole.md) |<span data-ttu-id="da3b8-131">Считывание свойств и отношений объекта directoryRole.</span><span class="sxs-lookup"><span data-stu-id="da3b8-131">Read properties and relationships of directoryRole object.</span></span>|
|[<span data-ttu-id="da3b8-132">Перечисление объектов directoryRole</span><span class="sxs-lookup"><span data-stu-id="da3b8-132">List directoryRoles</span></span>](../api/directoryrole-list.md) | <span data-ttu-id="da3b8-133">Коллекция объектов [directoryRole](directoryrole.md)</span><span class="sxs-lookup"><span data-stu-id="da3b8-133">[directoryRole](directoryrole.md) collection</span></span> | <span data-ttu-id="da3b8-134">Перечисление ролей каталога, активированных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="da3b8-134">List the directory roles that are activated in the tenant.</span></span> |
|[<span data-ttu-id="da3b8-135">Добавление элемента</span><span class="sxs-lookup"><span data-stu-id="da3b8-135">Add member</span></span>](../api/directoryrole-post-members.md) |[<span data-ttu-id="da3b8-136">directoryObject</span><span class="sxs-lookup"><span data-stu-id="da3b8-136">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="da3b8-137">Добавление пользователя в роль каталога путем записи данных в свойство навигации members.</span><span class="sxs-lookup"><span data-stu-id="da3b8-137">Add a user to the directory role by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="da3b8-138">Список членов</span><span class="sxs-lookup"><span data-stu-id="da3b8-138">List members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="da3b8-139">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="da3b8-139">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="da3b8-140">Получение пользователей, которые относятся к членам роли каталога, из свойства навигации members.</span><span class="sxs-lookup"><span data-stu-id="da3b8-140">Get the users that are members of the directory role from the members navigation property.</span></span>|
|[<span data-ttu-id="da3b8-141">Удаление члена</span><span class="sxs-lookup"><span data-stu-id="da3b8-141">Remove a member</span></span>](../api/directoryrole-delete-member.md) |[<span data-ttu-id="da3b8-142">directoryObject</span><span class="sxs-lookup"><span data-stu-id="da3b8-142">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="da3b8-143">Удаление ресурса user из роли каталога.</span><span class="sxs-lookup"><span data-stu-id="da3b8-143">Remove a user from the directory role.</span></span>|
|[<span data-ttu-id="da3b8-144">Список элементов области определения роли</span><span class="sxs-lookup"><span data-stu-id="da3b8-144">List scoped-role members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="da3b8-145">[scopedRoleMembership](scopedrolemembership.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="da3b8-145">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="da3b8-146">Список пользователей, которым эта роль каталогов, предназначенные для [администрирования единиц измерения](administrativeunit.md), через коллекцию ресурсов scopedRoleMembership.</span><span class="sxs-lookup"><span data-stu-id="da3b8-146">List the members of this directory role that are scoped to [administrative units](administrativeunit.md), through the scopedRoleMembership resource collection.</span></span>|
|[<span data-ttu-id="da3b8-147">delta</span><span class="sxs-lookup"><span data-stu-id="da3b8-147">delta</span></span>](../api/directoryrole-delta.md)|<span data-ttu-id="da3b8-148">Коллекция объектов directoryRole</span><span class="sxs-lookup"><span data-stu-id="da3b8-148">directoryRole collection</span></span>| <span data-ttu-id="da3b8-149">Получите добавочные изменения для каталога ролей.</span><span class="sxs-lookup"><span data-stu-id="da3b8-149">Get incremental changes for directory roles.</span></span> |

## <a name="properties"></a><span data-ttu-id="da3b8-150">Свойства</span><span class="sxs-lookup"><span data-stu-id="da3b8-150">Properties</span></span>
| <span data-ttu-id="da3b8-151">Свойство</span><span class="sxs-lookup"><span data-stu-id="da3b8-151">Property</span></span>   | <span data-ttu-id="da3b8-152">Тип</span><span class="sxs-lookup"><span data-stu-id="da3b8-152">Type</span></span> |<span data-ttu-id="da3b8-153">Описание</span><span class="sxs-lookup"><span data-stu-id="da3b8-153">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="da3b8-154">описание</span><span class="sxs-lookup"><span data-stu-id="da3b8-154">description</span></span>|<span data-ttu-id="da3b8-155">String</span><span class="sxs-lookup"><span data-stu-id="da3b8-155">String</span></span>|<span data-ttu-id="da3b8-p105">Описание роли каталога. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="da3b8-p105">The description for the directory role. Read-only.</span></span> |
|<span data-ttu-id="da3b8-158">displayName</span><span class="sxs-lookup"><span data-stu-id="da3b8-158">displayName</span></span>|<span data-ttu-id="da3b8-159">Строка</span><span class="sxs-lookup"><span data-stu-id="da3b8-159">String</span></span>|<span data-ttu-id="da3b8-p106">Отображаемое имя роли каталога. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="da3b8-p106">The display name for the directory role. Read-only.</span></span> |
|<span data-ttu-id="da3b8-162">id</span><span class="sxs-lookup"><span data-stu-id="da3b8-162">id</span></span>|<span data-ttu-id="da3b8-163">String</span><span class="sxs-lookup"><span data-stu-id="da3b8-163">String</span></span>|<span data-ttu-id="da3b8-p107">Уникальный идентификатор роли каталога. Наследуется из [directoryObject](directoryobject.md). Ключ, значение null не допускается, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="da3b8-p107">The unique identifier for the directory role. Inherited from [directoryObject](directoryobject.md). Key, Not nullable, Read-only.</span></span>|
|<span data-ttu-id="da3b8-167">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="da3b8-167">roleTemplateId</span></span>|<span data-ttu-id="da3b8-168">String</span><span class="sxs-lookup"><span data-stu-id="da3b8-168">String</span></span>| <span data-ttu-id="da3b8-p108">Свойство **id** ресурса [directoryRoleTemplate](directoryroletemplate.md), определяющего значения свойств для этой роли. При активации роли каталога на клиенте следует указать свойство с помощью операции POST. После активации роли каталога свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="da3b8-p108">The **id** of the [directoryRoleTemplate](directoryroletemplate.md) that this role is based on. The property must be specified when activating a directory role in a tenant with a POST operation. After the directory role has been activated, the property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="da3b8-172">Связи</span><span class="sxs-lookup"><span data-stu-id="da3b8-172">Relationships</span></span>
| <span data-ttu-id="da3b8-173">Связь</span><span class="sxs-lookup"><span data-stu-id="da3b8-173">Relationship</span></span> | <span data-ttu-id="da3b8-174">Тип</span><span class="sxs-lookup"><span data-stu-id="da3b8-174">Type</span></span> |<span data-ttu-id="da3b8-175">Описание</span><span class="sxs-lookup"><span data-stu-id="da3b8-175">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="da3b8-176">members</span><span class="sxs-lookup"><span data-stu-id="da3b8-176">members</span></span>|<span data-ttu-id="da3b8-177">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="da3b8-177">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="da3b8-p109">Пользователи, которые относятся к членам этой роли каталога. Методы HTTP: GET, POST, DELETE. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="da3b8-p109">Users that are members of this directory role. HTTP Methods: GET, POST, DELETE. Read-only. Nullable.</span></span>|
|<span data-ttu-id="da3b8-182">scopedMembers</span><span class="sxs-lookup"><span data-stu-id="da3b8-182">scopedMembers</span></span>|<span data-ttu-id="da3b8-183">[scopedRoleMembership](scopedrolemembership.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="da3b8-183">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="da3b8-184">Члены этой роли каталога, предназначенные для [администрирования единиц измерения](administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="da3b8-184">Members of this directory role that are scoped to [administrative units](administrativeunit.md).</span></span> <span data-ttu-id="da3b8-185">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="da3b8-185">Read-only.</span></span> <span data-ttu-id="da3b8-186">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="da3b8-186">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="da3b8-187">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="da3b8-187">JSON representation</span></span>

<span data-ttu-id="da3b8-188">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="da3b8-188">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "directoryRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
