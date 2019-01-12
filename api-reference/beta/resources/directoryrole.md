---
title: Тип ресурса directoryRole
description: Представляет роль directory Azure AD. Каталог роли Azure AD также называются *ролями администратора*. Дополнительные сведения о ролях каталогов (администратор) в разделе назначение ролей администратора в Azure AD. Microsoft Graph можно назначить роли каталог, чтобы предоставлять им разрешения целевой роли пользователей. Для чтения роли каталога или обновите его члены, необходимо активировать в клиентов. Только роль directory Администраторы организации активируется по умолчанию. Активация других ролей доступных каталогов, отправьте запрос POST с Идентификатором directoryRoleTemplate, лежащие в основе роли каталога. Наследуется от directoryObject.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e6753369be070ab04419cab0c870aec7e96b1fb2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927746"
---
# <a name="directoryrole-resource-type"></a><span data-ttu-id="a009b-110">Тип ресурса directoryRole</span><span class="sxs-lookup"><span data-stu-id="a009b-110">directoryRole resource type</span></span>

> <span data-ttu-id="a009b-111">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a009b-111">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a009b-112">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a009b-112">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a009b-113">Представляет роль directory Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a009b-113">Represents an Azure AD directory role.</span></span> <span data-ttu-id="a009b-114">Каталог роли Azure AD также называются *ролями администратора*.</span><span class="sxs-lookup"><span data-stu-id="a009b-114">Azure AD directory roles are also known as *administrator roles*.</span></span> <span data-ttu-id="a009b-115">Дополнительные сведения о ролях каталогов (администратор) можно [Назначение ролей администратора в Azure AD](https://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/).</span><span class="sxs-lookup"><span data-stu-id="a009b-115">For more information about directory (administrator) roles, see [Assigning administrator roles in Azure AD](https://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/).</span></span> <span data-ttu-id="a009b-116">Microsoft Graph можно назначить роли каталог, чтобы предоставлять им разрешения целевой роли пользователей.</span><span class="sxs-lookup"><span data-stu-id="a009b-116">With the Microsoft Graph, you can assign users to directory roles to grant them the permissions of the target role.</span></span> <span data-ttu-id="a009b-117">Для чтения роли каталога или обновите его члены, необходимо активировать в клиентов.</span><span class="sxs-lookup"><span data-stu-id="a009b-117">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="a009b-118">Только роль directory Администраторы организации активируется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a009b-118">Only the Company Administrators directory role is activated by default.</span></span> <span data-ttu-id="a009b-119">Активация других ролей доступных каталогов, отправьте запрос POST с Идентификатором [directoryRoleTemplate](directoryroletemplate.md) , лежащие в основе роли каталога.</span><span class="sxs-lookup"><span data-stu-id="a009b-119">To activate other available directory roles, you send a POST request with the ID of the [directoryRoleTemplate](directoryroletemplate.md) on which the directory role is based.</span></span> <span data-ttu-id="a009b-120">Наследуется от [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="a009b-120">Inherits from [directoryObject](directoryobject.md).</span></span>

<span data-ttu-id="a009b-121">По умолчанию каталог роли распространяются всей клиента.</span><span class="sxs-lookup"><span data-stu-id="a009b-121">By default, directory roles are scoped to be tenant-wide.</span></span>  <span data-ttu-id="a009b-122">Тем не менее каталог роли (в настоящее время только *администратора учетной записи пользователя* и *администратора служба технической поддержки*) может также областью действия [администратора единиц измерения](administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="a009b-122">However, directory roles (currently only the *user account admin* and *helpdesk admin*) may also be scoped to [administrative units](administrativeunit.md).</span></span>

<span data-ttu-id="a009b-123">Этот ресурс поддерживает:</span><span class="sxs-lookup"><span data-stu-id="a009b-123">This resource supports:</span></span>

- <span data-ttu-id="a009b-124">отслеживание дополнений, удалений и обновлений с помощью [запроса изменений](/graph/delta-query-overview) (функция [delta](../api/directoryrole-delta.md)).</span><span class="sxs-lookup"><span data-stu-id="a009b-124">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryrole-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="a009b-125">Методы</span><span class="sxs-lookup"><span data-stu-id="a009b-125">Methods</span></span>

| <span data-ttu-id="a009b-126">Метод</span><span class="sxs-lookup"><span data-stu-id="a009b-126">Method</span></span>       | <span data-ttu-id="a009b-127">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a009b-127">Return Type</span></span>  |<span data-ttu-id="a009b-128">Описание</span><span class="sxs-lookup"><span data-stu-id="a009b-128">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a009b-129">Получение directoryRole</span><span class="sxs-lookup"><span data-stu-id="a009b-129">Get directoryRole</span></span>](../api/directoryrole-get.md) | [<span data-ttu-id="a009b-130">directoryRole</span><span class="sxs-lookup"><span data-stu-id="a009b-130">directoryRole</span></span>](directoryrole.md) |<span data-ttu-id="a009b-131">Считывание свойств и отношений объекта directoryRole.</span><span class="sxs-lookup"><span data-stu-id="a009b-131">Read properties and relationships of directoryRole object.</span></span>|
|[<span data-ttu-id="a009b-132">Перечисление объектов directoryRole</span><span class="sxs-lookup"><span data-stu-id="a009b-132">List directoryRoles</span></span>](../api/directoryrole-list.md) | <span data-ttu-id="a009b-133">Коллекция объектов [directoryRole](directoryrole.md)</span><span class="sxs-lookup"><span data-stu-id="a009b-133">[directoryRole](directoryrole.md) collection</span></span> | <span data-ttu-id="a009b-134">Перечисление ролей каталога, активированных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="a009b-134">List the directory roles that are activated in the tenant.</span></span> |
|[<span data-ttu-id="a009b-135">Добавление элемента</span><span class="sxs-lookup"><span data-stu-id="a009b-135">Add member</span></span>](../api/directoryrole-post-members.md) |[<span data-ttu-id="a009b-136">directoryObject</span><span class="sxs-lookup"><span data-stu-id="a009b-136">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="a009b-137">Добавление пользователя в роль каталога путем записи данных в свойство навигации members.</span><span class="sxs-lookup"><span data-stu-id="a009b-137">Add a user to the directory role by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="a009b-138">Список членов</span><span class="sxs-lookup"><span data-stu-id="a009b-138">List members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="a009b-139">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="a009b-139">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="a009b-140">Получение пользователей, которые относятся к членам роли каталога, из свойства навигации members.</span><span class="sxs-lookup"><span data-stu-id="a009b-140">Get the users that are members of the directory role from the members navigation property.</span></span>|
|[<span data-ttu-id="a009b-141">Удаление члена</span><span class="sxs-lookup"><span data-stu-id="a009b-141">Remove a member</span></span>](../api/directoryrole-delete-member.md) |[<span data-ttu-id="a009b-142">directoryObject</span><span class="sxs-lookup"><span data-stu-id="a009b-142">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="a009b-143">Удаление ресурса user из роли каталога.</span><span class="sxs-lookup"><span data-stu-id="a009b-143">Remove a user from the directory role.</span></span>|
|[<span data-ttu-id="a009b-144">Список элементов области определения роли</span><span class="sxs-lookup"><span data-stu-id="a009b-144">List scoped-role members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="a009b-145">[scopedRoleMembership](scopedrolemembership.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="a009b-145">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="a009b-146">Список пользователей, которым эта роль каталогов, предназначенные для [администрирования единиц измерения](administrativeunit.md), через коллекцию ресурсов scopedRoleMembership.</span><span class="sxs-lookup"><span data-stu-id="a009b-146">List the members of this directory role that are scoped to [administrative units](administrativeunit.md), through the scopedRoleMembership resource collection.</span></span>|
|[<span data-ttu-id="a009b-147">delta</span><span class="sxs-lookup"><span data-stu-id="a009b-147">delta</span></span>](../api/directoryrole-delta.md)|<span data-ttu-id="a009b-148">Коллекция объектов directoryRole</span><span class="sxs-lookup"><span data-stu-id="a009b-148">directoryRole collection</span></span>| <span data-ttu-id="a009b-149">Получите добавочные изменения для каталога ролей.</span><span class="sxs-lookup"><span data-stu-id="a009b-149">Get incremental changes for directory roles.</span></span> |

## <a name="properties"></a><span data-ttu-id="a009b-150">Свойства</span><span class="sxs-lookup"><span data-stu-id="a009b-150">Properties</span></span>
| <span data-ttu-id="a009b-151">Свойство</span><span class="sxs-lookup"><span data-stu-id="a009b-151">Property</span></span>   | <span data-ttu-id="a009b-152">Тип</span><span class="sxs-lookup"><span data-stu-id="a009b-152">Type</span></span> |<span data-ttu-id="a009b-153">Описание</span><span class="sxs-lookup"><span data-stu-id="a009b-153">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a009b-154">описание</span><span class="sxs-lookup"><span data-stu-id="a009b-154">description</span></span>|<span data-ttu-id="a009b-155">String</span><span class="sxs-lookup"><span data-stu-id="a009b-155">String</span></span>|<span data-ttu-id="a009b-p105">Описание роли каталога. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a009b-p105">The description for the directory role. Read-only.</span></span> |
|<span data-ttu-id="a009b-158">displayName</span><span class="sxs-lookup"><span data-stu-id="a009b-158">displayName</span></span>|<span data-ttu-id="a009b-159">Строка</span><span class="sxs-lookup"><span data-stu-id="a009b-159">String</span></span>|<span data-ttu-id="a009b-p106">Отображаемое имя роли каталога. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a009b-p106">The display name for the directory role. Read-only.</span></span> |
|<span data-ttu-id="a009b-162">id</span><span class="sxs-lookup"><span data-stu-id="a009b-162">id</span></span>|<span data-ttu-id="a009b-163">String</span><span class="sxs-lookup"><span data-stu-id="a009b-163">String</span></span>|<span data-ttu-id="a009b-p107">Уникальный идентификатор роли каталога. Наследуется из [directoryObject](directoryobject.md). Ключ, значение null не допускается, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a009b-p107">The unique identifier for the directory role. Inherited from [directoryObject](directoryobject.md). Key, Not nullable, Read-only.</span></span>|
|<span data-ttu-id="a009b-167">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="a009b-167">roleTemplateId</span></span>|<span data-ttu-id="a009b-168">String</span><span class="sxs-lookup"><span data-stu-id="a009b-168">String</span></span>| <span data-ttu-id="a009b-p108">Свойство **id** ресурса [directoryRoleTemplate](directoryroletemplate.md), определяющего значения свойств для этой роли. При активации роли каталога на клиенте следует указать свойство с помощью операции POST. После активации роли каталога свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a009b-p108">The **id** of the [directoryRoleTemplate](directoryroletemplate.md) that this role is based on. The property must be specified when activating a directory role in a tenant with a POST operation. After the directory role has been activated, the property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="a009b-172">Связи</span><span class="sxs-lookup"><span data-stu-id="a009b-172">Relationships</span></span>
| <span data-ttu-id="a009b-173">Связь</span><span class="sxs-lookup"><span data-stu-id="a009b-173">Relationship</span></span> | <span data-ttu-id="a009b-174">Тип</span><span class="sxs-lookup"><span data-stu-id="a009b-174">Type</span></span> |<span data-ttu-id="a009b-175">Описание</span><span class="sxs-lookup"><span data-stu-id="a009b-175">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a009b-176">members</span><span class="sxs-lookup"><span data-stu-id="a009b-176">members</span></span>|<span data-ttu-id="a009b-177">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="a009b-177">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="a009b-p109">Пользователи, которые относятся к членам этой роли каталога. Методы HTTP: GET, POST, DELETE. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="a009b-p109">Users that are members of this directory role. HTTP Methods: GET, POST, DELETE. Read-only. Nullable.</span></span>|
|<span data-ttu-id="a009b-182">scopedMembers</span><span class="sxs-lookup"><span data-stu-id="a009b-182">scopedMembers</span></span>|<span data-ttu-id="a009b-183">[scopedRoleMembership](scopedrolemembership.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="a009b-183">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="a009b-184">Члены этой роли каталога, предназначенные для [администрирования единиц измерения](administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="a009b-184">Members of this directory role that are scoped to [administrative units](administrativeunit.md).</span></span> <span data-ttu-id="a009b-185">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a009b-185">Read-only.</span></span> <span data-ttu-id="a009b-186">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="a009b-186">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a009b-187">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a009b-187">JSON representation</span></span>

<span data-ttu-id="a009b-188">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a009b-188">Here is a JSON representation of the resource</span></span>

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
