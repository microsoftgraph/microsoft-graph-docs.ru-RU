---
title: Тип ресурса directoryRole
description: Представляет роль каталога Azure AD. Роли каталога Azure AD также известны как *роли администратора*. Дополнительные сведения о ролях каталогов (администратора) см. в разделе Назначение ролей администратора в Azure AD. С помощью Microsoft Graph вы можете назначить пользователям роли каталога, чтобы предоставить им разрешения целевой роли. Чтобы можно было считать роль каталога или обновить ее членов, сначала следует активировать ее на клиенте. По умолчанию активирована только роль каталога администраторов компании. Чтобы активировать другие доступные роли каталога, отправьте запрос POST с ИДЕНТИФИКАТОРом directoryRoleTemplate, на котором основана роль каталога. Наследуется от directoryObject.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 30b22313da70c33bffc0b759f9b474f4deac2ac1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535275"
---
# <a name="directoryrole-resource-type"></a><span data-ttu-id="c89bd-110">Тип ресурса directoryRole</span><span class="sxs-lookup"><span data-stu-id="c89bd-110">directoryRole resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c89bd-111">Представляет роль каталога Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c89bd-111">Represents an Azure AD directory role.</span></span> <span data-ttu-id="c89bd-112">Роли каталога Azure AD также известны как *роли администратора*.</span><span class="sxs-lookup"><span data-stu-id="c89bd-112">Azure AD directory roles are also known as *administrator roles*.</span></span> <span data-ttu-id="c89bd-113">Дополнительные сведения о ролях каталогов (администратора) см. [в разделе Назначение ролей администратора в Azure AD](https://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/).</span><span class="sxs-lookup"><span data-stu-id="c89bd-113">For more information about directory (administrator) roles, see [Assigning administrator roles in Azure AD](https://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/).</span></span> <span data-ttu-id="c89bd-114">С помощью Microsoft Graph вы можете назначить пользователям роли каталога, чтобы предоставить им разрешения целевой роли.</span><span class="sxs-lookup"><span data-stu-id="c89bd-114">With the Microsoft Graph, you can assign users to directory roles to grant them the permissions of the target role.</span></span> <span data-ttu-id="c89bd-115">Чтобы можно было считать роль каталога или обновить ее членов, сначала следует активировать ее на клиенте.</span><span class="sxs-lookup"><span data-stu-id="c89bd-115">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="c89bd-116">По умолчанию активирована только роль каталога администраторов компании.</span><span class="sxs-lookup"><span data-stu-id="c89bd-116">Only the Company Administrators directory role is activated by default.</span></span> <span data-ttu-id="c89bd-117">Чтобы активировать другие доступные роли каталога, отправьте запрос POST с ИДЕНТИФИКАТОРом [directoryRoleTemplate](directoryroletemplate.md) , на котором основана роль каталога.</span><span class="sxs-lookup"><span data-stu-id="c89bd-117">To activate other available directory roles, you send a POST request with the ID of the [directoryRoleTemplate](directoryroletemplate.md) on which the directory role is based.</span></span> <span data-ttu-id="c89bd-118">Наследуется от [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="c89bd-118">Inherits from [directoryObject](directoryobject.md).</span></span>

<span data-ttu-id="c89bd-119">По умолчанию роли каталога разделяются на уровне клиента.</span><span class="sxs-lookup"><span data-stu-id="c89bd-119">By default, directory roles are scoped to be tenant-wide.</span></span>  <span data-ttu-id="c89bd-120">Однако роли каталогов (в настоящее время только *Администратор учетной записи пользователя* и *администратор службы поддержки*) также могут быть ограничены [административными единицами](administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="c89bd-120">However, directory roles (currently only the *user account admin* and *helpdesk admin*) may also be scoped to [administrative units](administrativeunit.md).</span></span>

<span data-ttu-id="c89bd-121">Этот ресурс поддерживает:</span><span class="sxs-lookup"><span data-stu-id="c89bd-121">This resource supports:</span></span>

- <span data-ttu-id="c89bd-122">отслеживание дополнений, удалений и обновлений с помощью [запроса изменений](/graph/delta-query-overview) (функция [delta](../api/directoryrole-delta.md)).</span><span class="sxs-lookup"><span data-stu-id="c89bd-122">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryrole-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="c89bd-123">Методы</span><span class="sxs-lookup"><span data-stu-id="c89bd-123">Methods</span></span>

| <span data-ttu-id="c89bd-124">Метод</span><span class="sxs-lookup"><span data-stu-id="c89bd-124">Method</span></span>       | <span data-ttu-id="c89bd-125">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c89bd-125">Return Type</span></span>  |<span data-ttu-id="c89bd-126">Описание</span><span class="sxs-lookup"><span data-stu-id="c89bd-126">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c89bd-127">Получение directoryRole</span><span class="sxs-lookup"><span data-stu-id="c89bd-127">Get directoryRole</span></span>](../api/directoryrole-get.md) | [<span data-ttu-id="c89bd-128">directoryRole</span><span class="sxs-lookup"><span data-stu-id="c89bd-128">directoryRole</span></span>](directoryrole.md) |<span data-ttu-id="c89bd-129">Считывание свойств и отношений объекта directoryRole.</span><span class="sxs-lookup"><span data-stu-id="c89bd-129">Read properties and relationships of directoryRole object.</span></span>|
|[<span data-ttu-id="c89bd-130">Список перечисление directoryrole</span><span class="sxs-lookup"><span data-stu-id="c89bd-130">List directoryRoles</span></span>](../api/directoryrole-list.md) | <span data-ttu-id="c89bd-131">Коллекция объектов [directoryRole](directoryrole.md)</span><span class="sxs-lookup"><span data-stu-id="c89bd-131">[directoryRole](directoryrole.md) collection</span></span> | <span data-ttu-id="c89bd-132">Список ролей каталога, активированных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="c89bd-132">List the directory roles that are activated in the tenant.</span></span> |
|[<span data-ttu-id="c89bd-133">Добавление участника</span><span class="sxs-lookup"><span data-stu-id="c89bd-133">Add member</span></span>](../api/directoryrole-post-members.md) |[<span data-ttu-id="c89bd-134">directoryObject</span><span class="sxs-lookup"><span data-stu-id="c89bd-134">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="c89bd-135">Добавление пользователя в роль каталога путем записи данных в свойство навигации members.</span><span class="sxs-lookup"><span data-stu-id="c89bd-135">Add a user to the directory role by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="c89bd-136">Список членов</span><span class="sxs-lookup"><span data-stu-id="c89bd-136">List members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="c89bd-137">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="c89bd-137">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="c89bd-138">Получение пользователей, которые относятся к членам роли каталога, из свойства навигации members.</span><span class="sxs-lookup"><span data-stu-id="c89bd-138">Get the users that are members of the directory role from the members navigation property.</span></span>|
|[<span data-ttu-id="c89bd-139">Удаление участника</span><span class="sxs-lookup"><span data-stu-id="c89bd-139">Remove a member</span></span>](../api/directoryrole-delete-member.md) |[<span data-ttu-id="c89bd-140">directoryObject</span><span class="sxs-lookup"><span data-stu-id="c89bd-140">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="c89bd-141">Удаление пользователя из роли каталога.</span><span class="sxs-lookup"><span data-stu-id="c89bd-141">Remove a user from the directory role.</span></span>|
|[<span data-ttu-id="c89bd-142">Область списка — элементы роли</span><span class="sxs-lookup"><span data-stu-id="c89bd-142">List scoped-role members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="c89bd-143">Коллекция [scopedRoleMembership](scopedrolemembership.md)</span><span class="sxs-lookup"><span data-stu-id="c89bd-143">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="c89bd-144">ПереЧислите членов этой роли каталога, область действия которой ограничена [административными единицами](administrativeunit.md), с помощью коллекции ресурсов scopedrolemembership изменен.</span><span class="sxs-lookup"><span data-stu-id="c89bd-144">List the members of this directory role that are scoped to [administrative units](administrativeunit.md), through the scopedRoleMembership resource collection.</span></span>|
|[<span data-ttu-id="c89bd-145">delta</span><span class="sxs-lookup"><span data-stu-id="c89bd-145">delta</span></span>](../api/directoryrole-delta.md)|<span data-ttu-id="c89bd-146">Коллекция объектов directoryRole</span><span class="sxs-lookup"><span data-stu-id="c89bd-146">directoryRole collection</span></span>| <span data-ttu-id="c89bd-147">Получение добавочных изменений для ролей каталога.</span><span class="sxs-lookup"><span data-stu-id="c89bd-147">Get incremental changes for directory roles.</span></span> |

## <a name="properties"></a><span data-ttu-id="c89bd-148">Свойства</span><span class="sxs-lookup"><span data-stu-id="c89bd-148">Properties</span></span>
| <span data-ttu-id="c89bd-149">Свойство</span><span class="sxs-lookup"><span data-stu-id="c89bd-149">Property</span></span>   | <span data-ttu-id="c89bd-150">Тип</span><span class="sxs-lookup"><span data-stu-id="c89bd-150">Type</span></span> |<span data-ttu-id="c89bd-151">Описание</span><span class="sxs-lookup"><span data-stu-id="c89bd-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c89bd-152">description</span><span class="sxs-lookup"><span data-stu-id="c89bd-152">description</span></span>|<span data-ttu-id="c89bd-153">String</span><span class="sxs-lookup"><span data-stu-id="c89bd-153">String</span></span>|<span data-ttu-id="c89bd-p104">Описание роли каталога. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c89bd-p104">The description for the directory role. Read-only.</span></span> |
|<span data-ttu-id="c89bd-156">displayName</span><span class="sxs-lookup"><span data-stu-id="c89bd-156">displayName</span></span>|<span data-ttu-id="c89bd-157">Строка</span><span class="sxs-lookup"><span data-stu-id="c89bd-157">String</span></span>|<span data-ttu-id="c89bd-p105">Отображаемое имя роли каталога. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c89bd-p105">The display name for the directory role. Read-only.</span></span> |
|<span data-ttu-id="c89bd-160">id</span><span class="sxs-lookup"><span data-stu-id="c89bd-160">id</span></span>|<span data-ttu-id="c89bd-161">Строка</span><span class="sxs-lookup"><span data-stu-id="c89bd-161">String</span></span>|<span data-ttu-id="c89bd-p106">Уникальный идентификатор роли каталога. Наследуется из [directoryObject](directoryobject.md). Ключ, значение null не допускается, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c89bd-p106">The unique identifier for the directory role. Inherited from [directoryObject](directoryobject.md). Key, Not nullable, Read-only.</span></span>|
|<span data-ttu-id="c89bd-165">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="c89bd-165">roleTemplateId</span></span>|<span data-ttu-id="c89bd-166">String</span><span class="sxs-lookup"><span data-stu-id="c89bd-166">String</span></span>| <span data-ttu-id="c89bd-p107">Свойство **id** ресурса [directoryRoleTemplate](directoryroletemplate.md), определяющего значения свойств для этой роли. При активации роли каталога на клиенте следует указать свойство с помощью операции POST. После активации роли каталога свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c89bd-p107">The **id** of the [directoryRoleTemplate](directoryroletemplate.md) that this role is based on. The property must be specified when activating a directory role in a tenant with a POST operation. After the directory role has been activated, the property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="c89bd-170">Связи</span><span class="sxs-lookup"><span data-stu-id="c89bd-170">Relationships</span></span>
| <span data-ttu-id="c89bd-171">Отношение</span><span class="sxs-lookup"><span data-stu-id="c89bd-171">Relationship</span></span> | <span data-ttu-id="c89bd-172">Тип</span><span class="sxs-lookup"><span data-stu-id="c89bd-172">Type</span></span> |<span data-ttu-id="c89bd-173">Описание</span><span class="sxs-lookup"><span data-stu-id="c89bd-173">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c89bd-174">members</span><span class="sxs-lookup"><span data-stu-id="c89bd-174">members</span></span>|<span data-ttu-id="c89bd-175">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="c89bd-175">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="c89bd-p108">Пользователи, которые относятся к членам этой роли каталога. Методы HTTP: GET, POST, DELETE. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c89bd-p108">Users that are members of this directory role. HTTP Methods: GET, POST, DELETE. Read-only. Nullable.</span></span>|
|<span data-ttu-id="c89bd-180">Scopedadministrators</span><span class="sxs-lookup"><span data-stu-id="c89bd-180">scopedMembers</span></span>|<span data-ttu-id="c89bd-181">Коллекция [scopedRoleMembership](scopedrolemembership.md)</span><span class="sxs-lookup"><span data-stu-id="c89bd-181">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="c89bd-182">Члены этой роли каталога, областью действия которой являются [административные единицы](administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="c89bd-182">Members of this directory role that are scoped to [administrative units](administrativeunit.md).</span></span> <span data-ttu-id="c89bd-183">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c89bd-183">Read-only.</span></span> <span data-ttu-id="c89bd-184">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="c89bd-184">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c89bd-185">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c89bd-185">JSON representation</span></span>

<span data-ttu-id="c89bd-186">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c89bd-186">Here is a JSON representation of the resource</span></span>

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
