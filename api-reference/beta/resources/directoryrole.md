---
title: Тип ресурса directoryRole
description: Представляет роль каталога Azure AD. Роли каталога Azure AD также известны как *роли администратора*.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f4b462f2f597f777befd643004d918e5b2044620
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181815"
---
# <a name="directoryrole-resource-type"></a><span data-ttu-id="fb96e-104">Тип ресурса directoryRole</span><span class="sxs-lookup"><span data-stu-id="fb96e-104">directoryRole resource type</span></span>

<span data-ttu-id="fb96e-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb96e-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb96e-106">Представляет роль каталога Azure AD.</span><span class="sxs-lookup"><span data-stu-id="fb96e-106">Represents an Azure AD directory role.</span></span> <span data-ttu-id="fb96e-107">Роли каталога Azure AD также известны как *роли администратора*.</span><span class="sxs-lookup"><span data-stu-id="fb96e-107">Azure AD directory roles are also known as *administrator roles*.</span></span> <span data-ttu-id="fb96e-108">Для получения дополнительных сведений о ролях каталога (администратора) см. статью [Назначение ролей администратора в Azure AD](https://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/).</span><span class="sxs-lookup"><span data-stu-id="fb96e-108">For more information about directory (administrator) roles, see [Assigning administrator roles in Azure AD](https://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/).</span></span> <span data-ttu-id="fb96e-109">С помощью Microsoft Graph можно назначать пользователям роли каталога, чтобы предоставить им разрешения целевой роли.</span><span class="sxs-lookup"><span data-stu-id="fb96e-109">With the Microsoft Graph, you can assign users to directory roles to grant them the permissions of the target role.</span></span> <span data-ttu-id="fb96e-110">Чтобы можно было считать роль каталога или обновить ее членов, сначала следует активировать ее на клиенте.</span><span class="sxs-lookup"><span data-stu-id="fb96e-110">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="fb96e-111">По умолчанию активируется только роль каталога администраторов организации.</span><span class="sxs-lookup"><span data-stu-id="fb96e-111">Only the Company Administrators directory role is activated by default.</span></span> <span data-ttu-id="fb96e-112">Чтобы активировать другие доступные роли каталога, отправьте запрос POST с ИДЕНТИФИКАТОРом [directoryRoleTemplate](directoryroletemplate.md) , на котором основана роль каталога.</span><span class="sxs-lookup"><span data-stu-id="fb96e-112">To activate other available directory roles, you send a POST request with the ID of the [directoryRoleTemplate](directoryroletemplate.md) on which the directory role is based.</span></span> <span data-ttu-id="fb96e-113">[Перечислите шаблоны для ролей каталогов](../api/directoryroletemplate-list.md), чтобы получить все остальные доступные роли каталогов.</span><span class="sxs-lookup"><span data-stu-id="fb96e-113">[List directory role templates](../api/directoryroletemplate-list.md) to get all the other available directory roles.</span></span> <span data-ttu-id="fb96e-114">Наследуется от [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="fb96e-114">Inherits from [directoryObject](directoryobject.md).</span></span>

<span data-ttu-id="fb96e-115">По умолчанию роли каталога разделяются на уровне клиента.</span><span class="sxs-lookup"><span data-stu-id="fb96e-115">By default, directory roles are scoped to be tenant-wide.</span></span>  <span data-ttu-id="fb96e-116">Однако роли каталогов (в настоящее время только *Администратор учетной записи пользователя* и *администратор службы поддержки*) также могут быть ограничены [административными единицами](administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="fb96e-116">However, directory roles (currently only the *user account admin* and *helpdesk admin*) may also be scoped to [administrative units](administrativeunit.md).</span></span>

<span data-ttu-id="fb96e-117">Этот ресурс поддерживает:</span><span class="sxs-lookup"><span data-stu-id="fb96e-117">This resource supports:</span></span>

- <span data-ttu-id="fb96e-118">отслеживание дополнений, удалений и обновлений с помощью [запроса изменений](/graph/delta-query-overview) (функция [delta](../api/directoryrole-delta.md)).</span><span class="sxs-lookup"><span data-stu-id="fb96e-118">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryrole-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="fb96e-119">Методы</span><span class="sxs-lookup"><span data-stu-id="fb96e-119">Methods</span></span>

| <span data-ttu-id="fb96e-120">Метод</span><span class="sxs-lookup"><span data-stu-id="fb96e-120">Method</span></span>       | <span data-ttu-id="fb96e-121">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fb96e-121">Return Type</span></span>  |<span data-ttu-id="fb96e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="fb96e-122">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fb96e-123">Получение directoryRole</span><span class="sxs-lookup"><span data-stu-id="fb96e-123">Get directoryRole</span></span>](../api/directoryrole-get.md) | [<span data-ttu-id="fb96e-124">directoryRole</span><span class="sxs-lookup"><span data-stu-id="fb96e-124">directoryRole</span></span>](directoryrole.md) |<span data-ttu-id="fb96e-125">Считывание свойств и отношений объекта directoryRole.</span><span class="sxs-lookup"><span data-stu-id="fb96e-125">Read properties and relationships of directoryRole object.</span></span>|
|[<span data-ttu-id="fb96e-126">Перечисление объектов directoryRole</span><span class="sxs-lookup"><span data-stu-id="fb96e-126">List directoryRoles</span></span>](../api/directoryrole-list.md) | <span data-ttu-id="fb96e-127">Коллекция объектов [directoryRole](directoryrole.md)</span><span class="sxs-lookup"><span data-stu-id="fb96e-127">[directoryRole](directoryrole.md) collection</span></span> | <span data-ttu-id="fb96e-128">Перечисление ролей каталога, активированных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="fb96e-128">List the directory roles that are activated in the tenant.</span></span> |
|[<span data-ttu-id="fb96e-129">Добавление элемента</span><span class="sxs-lookup"><span data-stu-id="fb96e-129">Add member</span></span>](../api/directoryrole-post-members.md) |[<span data-ttu-id="fb96e-130">directoryObject</span><span class="sxs-lookup"><span data-stu-id="fb96e-130">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="fb96e-131">Добавление пользователя в роль каталога путем записи данных в свойство навигации members.</span><span class="sxs-lookup"><span data-stu-id="fb96e-131">Add a user to the directory role by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="fb96e-132">Список членов</span><span class="sxs-lookup"><span data-stu-id="fb96e-132">List members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="fb96e-133">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="fb96e-133">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="fb96e-134">Получение пользователей, которые относятся к членам роли каталога, из свойства навигации members.</span><span class="sxs-lookup"><span data-stu-id="fb96e-134">Get the users that are members of the directory role from the members navigation property.</span></span>|
|[<span data-ttu-id="fb96e-135">Удаление члена</span><span class="sxs-lookup"><span data-stu-id="fb96e-135">Remove a member</span></span>](../api/directoryrole-delete-member.md) |[<span data-ttu-id="fb96e-136">directoryObject</span><span class="sxs-lookup"><span data-stu-id="fb96e-136">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="fb96e-137">Удаление ресурса user из роли каталога.</span><span class="sxs-lookup"><span data-stu-id="fb96e-137">Remove a user from the directory role.</span></span>|
|[<span data-ttu-id="fb96e-138">Область списка — элементы роли</span><span class="sxs-lookup"><span data-stu-id="fb96e-138">List scoped-role members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="fb96e-139">Коллекция [scopedRoleMembership](scopedrolemembership.md)</span><span class="sxs-lookup"><span data-stu-id="fb96e-139">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="fb96e-140">Перечислите членов этой роли каталога, область действия которой ограничена [административными единицами](administrativeunit.md), с помощью коллекции ресурсов scopedrolemembership изменен.</span><span class="sxs-lookup"><span data-stu-id="fb96e-140">List the members of this directory role that are scoped to [administrative units](administrativeunit.md), through the scopedRoleMembership resource collection.</span></span>|
|[<span data-ttu-id="fb96e-141">delta</span><span class="sxs-lookup"><span data-stu-id="fb96e-141">delta</span></span>](../api/directoryrole-delta.md)|<span data-ttu-id="fb96e-142">Коллекция объектов directoryRole</span><span class="sxs-lookup"><span data-stu-id="fb96e-142">directoryRole collection</span></span>| <span data-ttu-id="fb96e-143">Получение добавочных изменений для ролей каталога.</span><span class="sxs-lookup"><span data-stu-id="fb96e-143">Get incremental changes for directory roles.</span></span> |

## <a name="properties"></a><span data-ttu-id="fb96e-144">Свойства</span><span class="sxs-lookup"><span data-stu-id="fb96e-144">Properties</span></span>
| <span data-ttu-id="fb96e-145">Свойство</span><span class="sxs-lookup"><span data-stu-id="fb96e-145">Property</span></span>   | <span data-ttu-id="fb96e-146">Тип</span><span class="sxs-lookup"><span data-stu-id="fb96e-146">Type</span></span> |<span data-ttu-id="fb96e-147">Описание</span><span class="sxs-lookup"><span data-stu-id="fb96e-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fb96e-148">description</span><span class="sxs-lookup"><span data-stu-id="fb96e-148">description</span></span>|<span data-ttu-id="fb96e-149">String</span><span class="sxs-lookup"><span data-stu-id="fb96e-149">String</span></span>|<span data-ttu-id="fb96e-p104">Описание роли каталога. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fb96e-p104">The description for the directory role. Read-only.</span></span> |
|<span data-ttu-id="fb96e-152">displayName</span><span class="sxs-lookup"><span data-stu-id="fb96e-152">displayName</span></span>|<span data-ttu-id="fb96e-153">Строка</span><span class="sxs-lookup"><span data-stu-id="fb96e-153">String</span></span>|<span data-ttu-id="fb96e-p105">Отображаемое имя роли каталога. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fb96e-p105">The display name for the directory role. Read-only.</span></span> |
|<span data-ttu-id="fb96e-156">id</span><span class="sxs-lookup"><span data-stu-id="fb96e-156">id</span></span>|<span data-ttu-id="fb96e-157">Строка</span><span class="sxs-lookup"><span data-stu-id="fb96e-157">String</span></span>|<span data-ttu-id="fb96e-p106">Уникальный идентификатор роли каталога. Наследуется из [directoryObject](directoryobject.md). Ключ, значение null не допускается, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fb96e-p106">The unique identifier for the directory role. Inherited from [directoryObject](directoryobject.md). Key, Not nullable, Read-only.</span></span>|
|<span data-ttu-id="fb96e-161">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="fb96e-161">roleTemplateId</span></span>|<span data-ttu-id="fb96e-162">String</span><span class="sxs-lookup"><span data-stu-id="fb96e-162">String</span></span>| <span data-ttu-id="fb96e-p107">Свойство **id** ресурса [directoryRoleTemplate](directoryroletemplate.md), определяющего значения свойств для этой роли. При активации роли каталога на клиенте следует указать свойство с помощью операции POST. После активации роли каталога свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fb96e-p107">The **id** of the [directoryRoleTemplate](directoryroletemplate.md) that this role is based on. The property must be specified when activating a directory role in a tenant with a POST operation. After the directory role has been activated, the property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="fb96e-166">Связи</span><span class="sxs-lookup"><span data-stu-id="fb96e-166">Relationships</span></span>
| <span data-ttu-id="fb96e-167">Связь</span><span class="sxs-lookup"><span data-stu-id="fb96e-167">Relationship</span></span> | <span data-ttu-id="fb96e-168">Тип</span><span class="sxs-lookup"><span data-stu-id="fb96e-168">Type</span></span> |<span data-ttu-id="fb96e-169">Описание</span><span class="sxs-lookup"><span data-stu-id="fb96e-169">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fb96e-170">members</span><span class="sxs-lookup"><span data-stu-id="fb96e-170">members</span></span>|<span data-ttu-id="fb96e-171">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="fb96e-171">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="fb96e-p108">Пользователи, которые относятся к членам этой роли каталога. Методы HTTP: GET, POST, DELETE. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="fb96e-p108">Users that are members of this directory role. HTTP Methods: GET, POST, DELETE. Read-only. Nullable.</span></span>|
|<span data-ttu-id="fb96e-176">Scopedadministrators</span><span class="sxs-lookup"><span data-stu-id="fb96e-176">scopedMembers</span></span>|<span data-ttu-id="fb96e-177">Коллекция [scopedRoleMembership](scopedrolemembership.md)</span><span class="sxs-lookup"><span data-stu-id="fb96e-177">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="fb96e-178">Члены этой роли каталога, областью действия которой являются [административные единицы](administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="fb96e-178">Members of this directory role that are scoped to [administrative units](administrativeunit.md).</span></span> <span data-ttu-id="fb96e-179">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fb96e-179">Read-only.</span></span> <span data-ttu-id="fb96e-180">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="fb96e-180">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fb96e-181">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fb96e-181">JSON representation</span></span>

<span data-ttu-id="fb96e-182">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fb96e-182">Here is a JSON representation of the resource</span></span>

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
