---
title: Тип ресурса directoryRole
description: Представляет роль каталога Azure AD. Роли каталога Azure AD также известны как *роли администратора*.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f09a6f248e7a677cb5e19bcc00085933b90b24a4
ms.sourcegitcommit: 9cd96fcbaae9d2ebaa3f3b69e440a1aea106f535
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/17/2019
ms.locfileid: "36450503"
---
# <a name="directoryrole-resource-type"></a><span data-ttu-id="37de1-104">Тип ресурса directoryRole</span><span class="sxs-lookup"><span data-stu-id="37de1-104">directoryRole resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37de1-105">Представляет роль каталога Azure AD.</span><span class="sxs-lookup"><span data-stu-id="37de1-105">Represents an Azure AD directory role.</span></span> <span data-ttu-id="37de1-106">Роли каталога Azure AD также известны как *роли администратора*.</span><span class="sxs-lookup"><span data-stu-id="37de1-106">Azure AD directory roles are also known as *administrator roles*.</span></span> <span data-ttu-id="37de1-107">Для получения дополнительных сведений о ролях каталога (администратора) см. статью [Назначение ролей администратора в Azure AD](https://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/).</span><span class="sxs-lookup"><span data-stu-id="37de1-107">For more information about directory (administrator) roles, see [Assigning administrator roles in Azure AD](https://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/).</span></span> <span data-ttu-id="37de1-108">С помощью Microsoft Graph можно назначать пользователям роли каталога, чтобы предоставить им разрешения целевой роли.</span><span class="sxs-lookup"><span data-stu-id="37de1-108">With the Microsoft Graph, you can assign users to directory roles to grant them the permissions of the target role.</span></span> <span data-ttu-id="37de1-109">Чтобы можно было считать роль каталога или обновить ее членов, сначала следует активировать ее на клиенте.</span><span class="sxs-lookup"><span data-stu-id="37de1-109">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="37de1-110">По умолчанию активируется только роль каталога администраторов организации.</span><span class="sxs-lookup"><span data-stu-id="37de1-110">Only the Company Administrators directory role is activated by default.</span></span> <span data-ttu-id="37de1-111">Чтобы активировать другие доступные роли каталога, отправьте запрос POST с ИДЕНТИФИКАТОРом [directoryRoleTemplate](directoryroletemplate.md) , на котором основана роль каталога.</span><span class="sxs-lookup"><span data-stu-id="37de1-111">To activate other available directory roles, you send a POST request with the ID of the [directoryRoleTemplate](directoryroletemplate.md) on which the directory role is based.</span></span> <span data-ttu-id="37de1-112">[Список шаблонов роли каталога](../api/directoryroletemplate-list.md) для получения всех других доступных ролей каталога.</span><span class="sxs-lookup"><span data-stu-id="37de1-112">[List directory role templates](../api/directoryroletemplate-list.md) to get all the other available directory roles.</span></span> <span data-ttu-id="37de1-113">Наследуется от [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="37de1-113">Inherits from [directoryObject](directoryobject.md).</span></span>

<span data-ttu-id="37de1-114">По умолчанию роли каталога разделяются на уровне клиента.</span><span class="sxs-lookup"><span data-stu-id="37de1-114">By default, directory roles are scoped to be tenant-wide.</span></span>  <span data-ttu-id="37de1-115">Однако роли каталогов (в настоящее время только *Администратор учетной записи пользователя* и *администратор службы поддержки*) также могут быть ограничены [административными единицами](administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="37de1-115">However, directory roles (currently only the *user account admin* and *helpdesk admin*) may also be scoped to [administrative units](administrativeunit.md).</span></span>

<span data-ttu-id="37de1-116">Этот ресурс поддерживает:</span><span class="sxs-lookup"><span data-stu-id="37de1-116">This resource supports:</span></span>

- <span data-ttu-id="37de1-117">отслеживание дополнений, удалений и обновлений с помощью [запроса изменений](/graph/delta-query-overview) (функция [delta](../api/directoryrole-delta.md)).</span><span class="sxs-lookup"><span data-stu-id="37de1-117">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryrole-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="37de1-118">Методы</span><span class="sxs-lookup"><span data-stu-id="37de1-118">Methods</span></span>

| <span data-ttu-id="37de1-119">Метод</span><span class="sxs-lookup"><span data-stu-id="37de1-119">Method</span></span>       | <span data-ttu-id="37de1-120">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="37de1-120">Return Type</span></span>  |<span data-ttu-id="37de1-121">Описание</span><span class="sxs-lookup"><span data-stu-id="37de1-121">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="37de1-122">Получение directoryRole</span><span class="sxs-lookup"><span data-stu-id="37de1-122">Get directoryRole</span></span>](../api/directoryrole-get.md) | [<span data-ttu-id="37de1-123">directoryRole</span><span class="sxs-lookup"><span data-stu-id="37de1-123">directoryRole</span></span>](directoryrole.md) |<span data-ttu-id="37de1-124">Считывание свойств и отношений объекта directoryRole.</span><span class="sxs-lookup"><span data-stu-id="37de1-124">Read properties and relationships of directoryRole object.</span></span>|
|[<span data-ttu-id="37de1-125">Перечисление объектов directoryRole</span><span class="sxs-lookup"><span data-stu-id="37de1-125">List directoryRoles</span></span>](../api/directoryrole-list.md) | <span data-ttu-id="37de1-126">Коллекция объектов [directoryRole](directoryrole.md)</span><span class="sxs-lookup"><span data-stu-id="37de1-126">[directoryRole](directoryrole.md) collection</span></span> | <span data-ttu-id="37de1-127">Перечисление ролей каталога, активированных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="37de1-127">List the directory roles that are activated in the tenant.</span></span> |
|[<span data-ttu-id="37de1-128">Добавление элемента</span><span class="sxs-lookup"><span data-stu-id="37de1-128">Add member</span></span>](../api/directoryrole-post-members.md) |[<span data-ttu-id="37de1-129">directoryObject</span><span class="sxs-lookup"><span data-stu-id="37de1-129">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="37de1-130">Добавление пользователя в роль каталога путем записи данных в свойство навигации members.</span><span class="sxs-lookup"><span data-stu-id="37de1-130">Add a user to the directory role by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="37de1-131">Список членов</span><span class="sxs-lookup"><span data-stu-id="37de1-131">List members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="37de1-132">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="37de1-132">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="37de1-133">Получение пользователей, которые относятся к членам роли каталога, из свойства навигации members.</span><span class="sxs-lookup"><span data-stu-id="37de1-133">Get the users that are members of the directory role from the members navigation property.</span></span>|
|[<span data-ttu-id="37de1-134">Удаление члена</span><span class="sxs-lookup"><span data-stu-id="37de1-134">Remove a member</span></span>](../api/directoryrole-delete-member.md) |[<span data-ttu-id="37de1-135">directoryObject</span><span class="sxs-lookup"><span data-stu-id="37de1-135">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="37de1-136">Удаление ресурса user из роли каталога.</span><span class="sxs-lookup"><span data-stu-id="37de1-136">Remove a user from the directory role.</span></span>|
|[<span data-ttu-id="37de1-137">Область списка — элементы роли</span><span class="sxs-lookup"><span data-stu-id="37de1-137">List scoped-role members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="37de1-138">Коллекция [scopedRoleMembership](scopedrolemembership.md)</span><span class="sxs-lookup"><span data-stu-id="37de1-138">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="37de1-139">Перечислите членов этой роли каталога, область действия которой ограничена [административными единицами](administrativeunit.md), с помощью коллекции ресурсов scopedrolemembership изменен.</span><span class="sxs-lookup"><span data-stu-id="37de1-139">List the members of this directory role that are scoped to [administrative units](administrativeunit.md), through the scopedRoleMembership resource collection.</span></span>|
|[<span data-ttu-id="37de1-140">delta</span><span class="sxs-lookup"><span data-stu-id="37de1-140">delta</span></span>](../api/directoryrole-delta.md)|<span data-ttu-id="37de1-141">Коллекция объектов directoryRole</span><span class="sxs-lookup"><span data-stu-id="37de1-141">directoryRole collection</span></span>| <span data-ttu-id="37de1-142">Получение добавочных изменений для ролей каталога.</span><span class="sxs-lookup"><span data-stu-id="37de1-142">Get incremental changes for directory roles.</span></span> |

## <a name="properties"></a><span data-ttu-id="37de1-143">Свойства</span><span class="sxs-lookup"><span data-stu-id="37de1-143">Properties</span></span>
| <span data-ttu-id="37de1-144">Свойство</span><span class="sxs-lookup"><span data-stu-id="37de1-144">Property</span></span>   | <span data-ttu-id="37de1-145">Тип</span><span class="sxs-lookup"><span data-stu-id="37de1-145">Type</span></span> |<span data-ttu-id="37de1-146">Описание</span><span class="sxs-lookup"><span data-stu-id="37de1-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="37de1-147">description</span><span class="sxs-lookup"><span data-stu-id="37de1-147">description</span></span>|<span data-ttu-id="37de1-148">String</span><span class="sxs-lookup"><span data-stu-id="37de1-148">String</span></span>|<span data-ttu-id="37de1-p104">Описание роли каталога. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="37de1-p104">The description for the directory role. Read-only.</span></span> |
|<span data-ttu-id="37de1-151">displayName</span><span class="sxs-lookup"><span data-stu-id="37de1-151">displayName</span></span>|<span data-ttu-id="37de1-152">Строка</span><span class="sxs-lookup"><span data-stu-id="37de1-152">String</span></span>|<span data-ttu-id="37de1-p105">Отображаемое имя роли каталога. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="37de1-p105">The display name for the directory role. Read-only.</span></span> |
|<span data-ttu-id="37de1-155">id</span><span class="sxs-lookup"><span data-stu-id="37de1-155">id</span></span>|<span data-ttu-id="37de1-156">Строка</span><span class="sxs-lookup"><span data-stu-id="37de1-156">String</span></span>|<span data-ttu-id="37de1-p106">Уникальный идентификатор роли каталога. Наследуется из [directoryObject](directoryobject.md). Ключ, значение null не допускается, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="37de1-p106">The unique identifier for the directory role. Inherited from [directoryObject](directoryobject.md). Key, Not nullable, Read-only.</span></span>|
|<span data-ttu-id="37de1-160">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="37de1-160">roleTemplateId</span></span>|<span data-ttu-id="37de1-161">String</span><span class="sxs-lookup"><span data-stu-id="37de1-161">String</span></span>| <span data-ttu-id="37de1-p107">Свойство **id** ресурса [directoryRoleTemplate](directoryroletemplate.md), определяющего значения свойств для этой роли. При активации роли каталога на клиенте следует указать свойство с помощью операции POST. После активации роли каталога свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="37de1-p107">The **id** of the [directoryRoleTemplate](directoryroletemplate.md) that this role is based on. The property must be specified when activating a directory role in a tenant with a POST operation. After the directory role has been activated, the property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="37de1-165">Связи</span><span class="sxs-lookup"><span data-stu-id="37de1-165">Relationships</span></span>
| <span data-ttu-id="37de1-166">Отношение</span><span class="sxs-lookup"><span data-stu-id="37de1-166">Relationship</span></span> | <span data-ttu-id="37de1-167">Тип</span><span class="sxs-lookup"><span data-stu-id="37de1-167">Type</span></span> |<span data-ttu-id="37de1-168">Описание</span><span class="sxs-lookup"><span data-stu-id="37de1-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="37de1-169">members</span><span class="sxs-lookup"><span data-stu-id="37de1-169">members</span></span>|<span data-ttu-id="37de1-170">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="37de1-170">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="37de1-p108">Пользователи, которые относятся к членам этой роли каталога. Методы HTTP: GET, POST, DELETE. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="37de1-p108">Users that are members of this directory role. HTTP Methods: GET, POST, DELETE. Read-only. Nullable.</span></span>|
|<span data-ttu-id="37de1-175">Scopedadministrators</span><span class="sxs-lookup"><span data-stu-id="37de1-175">scopedMembers</span></span>|<span data-ttu-id="37de1-176">Коллекция [scopedRoleMembership](scopedrolemembership.md)</span><span class="sxs-lookup"><span data-stu-id="37de1-176">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="37de1-177">Члены этой роли каталога, областью действия которой являются [административные единицы](administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="37de1-177">Members of this directory role that are scoped to [administrative units](administrativeunit.md).</span></span> <span data-ttu-id="37de1-178">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="37de1-178">Read-only.</span></span> <span data-ttu-id="37de1-179">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="37de1-179">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="37de1-180">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="37de1-180">JSON representation</span></span>

<span data-ttu-id="37de1-181">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="37de1-181">Here is a JSON representation of the resource</span></span>

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
