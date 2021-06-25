---
title: Тип ресурса directoryRole
description: Представляет роль каталога Azure AD. Роли каталога Azure AD также известны как *роли администратора*.
localization_priority: Priority
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 4ed98c9fef582d2299fb9ed63f2474b0a3903611
ms.sourcegitcommit: d0d2d17a31cbcb01b1ae18bd6a18c39d7077069a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53118681"
---
# <a name="directoryrole-resource-type"></a><span data-ttu-id="72f2e-104">Тип ресурса directoryRole</span><span class="sxs-lookup"><span data-stu-id="72f2e-104">directoryRole resource type</span></span>

<span data-ttu-id="72f2e-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72f2e-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="72f2e-106">Представляет роль каталога Azure AD.</span><span class="sxs-lookup"><span data-stu-id="72f2e-106">Represents an Azure AD directory role.</span></span> <span data-ttu-id="72f2e-107">Роли каталога Azure AD также известны как *роли администратора*.</span><span class="sxs-lookup"><span data-stu-id="72f2e-107">Azure AD directory roles are also known as *administrator roles*.</span></span> <span data-ttu-id="72f2e-108">Для получения дополнительных сведений о ролях каталога (администратора) см. статью [Назначение ролей администратора в Azure AD](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span><span class="sxs-lookup"><span data-stu-id="72f2e-108">For more information about directory (administrator) roles, see [Assigning administrator roles in Azure AD](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span> <span data-ttu-id="72f2e-109">С помощью Microsoft Graph можно назначать пользователям роли каталога, чтобы предоставить им разрешения целевой роли.</span><span class="sxs-lookup"><span data-stu-id="72f2e-109">With the Microsoft Graph, you can assign users to directory roles to grant them the permissions of the target role.</span></span> <span data-ttu-id="72f2e-110">Чтобы можно было считать роль каталога или обновить ее членов, сначала следует активировать ее на клиенте.</span><span class="sxs-lookup"><span data-stu-id="72f2e-110">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="72f2e-111">По умолчанию активируется только роль каталога администраторов организации.</span><span class="sxs-lookup"><span data-stu-id="72f2e-111">Only the Company Administrators directory role is activated by default.</span></span> <span data-ttu-id="72f2e-112">Чтобы активировать остальные доступные роли каталога, следует отправить запрос POST с идентификатором ресурса [directoryRoleTemplate](directoryroletemplate.md), определяющего значения свойств для роли каталога.</span><span class="sxs-lookup"><span data-stu-id="72f2e-112">To activate other available directory roles you send a POST request with the ID of the [directoryRoleTemplate](directoryroletemplate.md) on which the directory role is based.</span></span> <span data-ttu-id="72f2e-113">[Перечислите шаблоны для ролей каталогов](../api/directoryroletemplate-list.md), чтобы получить все остальные доступные роли каталогов.</span><span class="sxs-lookup"><span data-stu-id="72f2e-113">[List directory role templates](../api/directoryroletemplate-list.md) to get all the other available directory roles.</span></span> <span data-ttu-id="72f2e-114">Наследуется от [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="72f2e-114">Inherits from [directoryObject](directoryobject.md).</span></span>

<span data-ttu-id="72f2e-115">Этот ресурс поддерживает:</span><span class="sxs-lookup"><span data-stu-id="72f2e-115">This resource supports:</span></span>

- <span data-ttu-id="72f2e-116">отслеживание дополнений, удалений и обновлений с помощью [запроса изменений](/graph/delta-query-overview) (функция [delta](../api/directoryrole-delta.md)).</span><span class="sxs-lookup"><span data-stu-id="72f2e-116">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryrole-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="72f2e-117">Методы</span><span class="sxs-lookup"><span data-stu-id="72f2e-117">Methods</span></span>

| <span data-ttu-id="72f2e-118">Метод</span><span class="sxs-lookup"><span data-stu-id="72f2e-118">Method</span></span>       | <span data-ttu-id="72f2e-119">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="72f2e-119">Return Type</span></span>  |<span data-ttu-id="72f2e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="72f2e-120">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="72f2e-121">Получение directoryRole</span><span class="sxs-lookup"><span data-stu-id="72f2e-121">Get directoryRole</span></span>](../api/directoryrole-get.md) | [<span data-ttu-id="72f2e-122">directoryRole</span><span class="sxs-lookup"><span data-stu-id="72f2e-122">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="72f2e-123">Считывание свойств и отношений объекта directoryRole.</span><span class="sxs-lookup"><span data-stu-id="72f2e-123">Read properties and relationships of directoryRole object.</span></span> |
|[<span data-ttu-id="72f2e-124">Перечисление объектов directoryRole</span><span class="sxs-lookup"><span data-stu-id="72f2e-124">List directoryRoles</span></span>](../api/directoryrole-list.md) | <span data-ttu-id="72f2e-125">Коллекция объектов [directoryRole](directoryrole.md)</span><span class="sxs-lookup"><span data-stu-id="72f2e-125">[directoryRole](directoryrole.md) collection</span></span> | <span data-ttu-id="72f2e-126">Перечисление ролей каталога, активированных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="72f2e-126">List the directory roles that are activated in the tenant.</span></span> |
|[<span data-ttu-id="72f2e-127">Добавление элемента</span><span class="sxs-lookup"><span data-stu-id="72f2e-127">Add member</span></span>](../api/directoryrole-post-members.md) |[<span data-ttu-id="72f2e-128">directoryObject</span><span class="sxs-lookup"><span data-stu-id="72f2e-128">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="72f2e-129">Добавление пользователя в роль каталога путем записи данных в свойство навигации members.</span><span class="sxs-lookup"><span data-stu-id="72f2e-129">Add a user to the directory role by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="72f2e-130">Список членов</span><span class="sxs-lookup"><span data-stu-id="72f2e-130">List members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="72f2e-131">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="72f2e-131">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="72f2e-132">Получение пользователей, которые относятся к членам роли каталога, из свойства навигации members.</span><span class="sxs-lookup"><span data-stu-id="72f2e-132">Get the users that are members of the directory role from the members navigation property.</span></span>|
|[<span data-ttu-id="72f2e-133">Удаление члена</span><span class="sxs-lookup"><span data-stu-id="72f2e-133">Remove a member</span></span>](../api/directoryrole-delete-member.md) |[<span data-ttu-id="72f2e-134">directoryObject</span><span class="sxs-lookup"><span data-stu-id="72f2e-134">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="72f2e-135">Удаление ресурса user из роли каталога.</span><span class="sxs-lookup"><span data-stu-id="72f2e-135">Remove a user from the directory role.</span></span>|
|[<span data-ttu-id="72f2e-136">Активация directoryRole</span><span class="sxs-lookup"><span data-stu-id="72f2e-136">Activate directoryRole</span></span>](../api/directoryrole-post-directoryroles.md) |[<span data-ttu-id="72f2e-137">directoryRole</span><span class="sxs-lookup"><span data-stu-id="72f2e-137">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="72f2e-138">Активация роли каталога.</span><span class="sxs-lookup"><span data-stu-id="72f2e-138">Activate a directory role.</span></span>|
|[<span data-ttu-id="72f2e-139">Перечисление объектов scopedMember</span><span class="sxs-lookup"><span data-stu-id="72f2e-139">List scopedMembers</span></span>](../api/directoryrole-list-scopedmembers.md) |<span data-ttu-id="72f2e-140">Коллекция [scopedRoleMembership](scopedrolemembership.md)</span><span class="sxs-lookup"><span data-stu-id="72f2e-140">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="72f2e-141">Перечисление участников этой роли каталога, относящихся к области [административных единиц](administrativeunit.md), с помощью коллекции ресурсов scopedRoleMembership.</span><span class="sxs-lookup"><span data-stu-id="72f2e-141">List the members of this directory role that are scoped to [administrative units](administrativeunit.md), through the scopedRoleMembership resource collection.</span></span>|
|[<span data-ttu-id="72f2e-142">delta</span><span class="sxs-lookup"><span data-stu-id="72f2e-142">delta</span></span>](../api/directoryrole-delta.md)|<span data-ttu-id="72f2e-143">Коллекция объектов directoryRole</span><span class="sxs-lookup"><span data-stu-id="72f2e-143">directoryRole collection</span></span>| <span data-ttu-id="72f2e-144">Получение добавочных изменений для ролей каталога.</span><span class="sxs-lookup"><span data-stu-id="72f2e-144">Get incremental changes for directory roles.</span></span> |

## <a name="properties"></a><span data-ttu-id="72f2e-145">Свойства</span><span class="sxs-lookup"><span data-stu-id="72f2e-145">Properties</span></span>
| <span data-ttu-id="72f2e-146">Свойство</span><span class="sxs-lookup"><span data-stu-id="72f2e-146">Property</span></span>   | <span data-ttu-id="72f2e-147">Тип</span><span class="sxs-lookup"><span data-stu-id="72f2e-147">Type</span></span> | <span data-ttu-id="72f2e-148">Описание</span><span class="sxs-lookup"><span data-stu-id="72f2e-148">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="72f2e-149">description</span><span class="sxs-lookup"><span data-stu-id="72f2e-149">description</span></span>|<span data-ttu-id="72f2e-150">String</span><span class="sxs-lookup"><span data-stu-id="72f2e-150">String</span></span>|<span data-ttu-id="72f2e-p103">Описание роли каталога. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="72f2e-p103">The description for the directory role. Read-only.</span></span> |
|<span data-ttu-id="72f2e-153">displayName</span><span class="sxs-lookup"><span data-stu-id="72f2e-153">displayName</span></span>|<span data-ttu-id="72f2e-154">Строка</span><span class="sxs-lookup"><span data-stu-id="72f2e-154">String</span></span>|<span data-ttu-id="72f2e-p104">Отображаемое имя роли каталога. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="72f2e-p104">The display name for the directory role. Read-only.</span></span> |
|<span data-ttu-id="72f2e-157">id</span><span class="sxs-lookup"><span data-stu-id="72f2e-157">id</span></span>|<span data-ttu-id="72f2e-158">Строка</span><span class="sxs-lookup"><span data-stu-id="72f2e-158">String</span></span>|<span data-ttu-id="72f2e-p105">Уникальный идентификатор роли каталога. Наследуется из [directoryObject](directoryobject.md). Ключ, значение null не допускается, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="72f2e-p105">The unique identifier for the directory role. Inherited from [directoryObject](directoryobject.md). Key, Not nullable, Read-only.</span></span>|
|<span data-ttu-id="72f2e-162">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="72f2e-162">roleTemplateId</span></span>|<span data-ttu-id="72f2e-163">String</span><span class="sxs-lookup"><span data-stu-id="72f2e-163">String</span></span>| <span data-ttu-id="72f2e-p106">Свойство **id** ресурса [directoryRoleTemplate](directoryroletemplate.md), определяющего значения свойств для этой роли. При активации роли каталога на клиенте следует указать свойство с помощью операции POST. После активации роли каталога свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="72f2e-p106">The **id** of the [directoryRoleTemplate](directoryroletemplate.md) that this role is based on. The property must be specified when activating a directory role in a tenant with a POST operation. After the directory role has been activated, the property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="72f2e-167">Связи</span><span class="sxs-lookup"><span data-stu-id="72f2e-167">Relationships</span></span>
| <span data-ttu-id="72f2e-168">Связь</span><span class="sxs-lookup"><span data-stu-id="72f2e-168">Relationship</span></span> | <span data-ttu-id="72f2e-169">Тип</span><span class="sxs-lookup"><span data-stu-id="72f2e-169">Type</span></span> |<span data-ttu-id="72f2e-170">Описание</span><span class="sxs-lookup"><span data-stu-id="72f2e-170">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="72f2e-171">members</span><span class="sxs-lookup"><span data-stu-id="72f2e-171">members</span></span>|<span data-ttu-id="72f2e-172">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="72f2e-172">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="72f2e-p107">Пользователи, которые относятся к членам этой роли каталога. Методы HTTP: GET, POST, DELETE. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="72f2e-p107">Users that are members of this directory role. HTTP Methods: GET, POST, DELETE. Read-only. Nullable.</span></span>|
|<span data-ttu-id="72f2e-177">scopedMembers</span><span class="sxs-lookup"><span data-stu-id="72f2e-177">scopedMembers</span></span>|<span data-ttu-id="72f2e-178">Коллекция [scopedRoleMembership](scopedrolemembership.md)</span><span class="sxs-lookup"><span data-stu-id="72f2e-178">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="72f2e-179">Участники роли каталога, относящихся к области [административных единиц](administrativeunit.md).</span><span class="sxs-lookup"><span data-stu-id="72f2e-179">Members of this directory role that are scoped to [administrative units](administrativeunit.md).</span></span> <span data-ttu-id="72f2e-180">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="72f2e-180">Read-only.</span></span> <span data-ttu-id="72f2e-181">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="72f2e-181">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="72f2e-182">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="72f2e-182">JSON representation</span></span>

<span data-ttu-id="72f2e-183">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="72f2e-183">Here is a JSON representation of the resource</span></span>

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
