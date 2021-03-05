---
title: Тип ресурса directoryRole
description: Представляет роль каталога Azure AD. Роли каталога Azure AD также известны как *роли администратора*.
localization_priority: Priority
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: ffff28d87464289db6280aa1a7e3822736db02b8
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439900"
---
# <a name="directoryrole-resource-type"></a><span data-ttu-id="4e966-104">Тип ресурса directoryRole</span><span class="sxs-lookup"><span data-stu-id="4e966-104">directoryRole resource type</span></span>

<span data-ttu-id="4e966-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e966-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4e966-106">Представляет роль каталога Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4e966-106">Represents an Azure AD directory role.</span></span> <span data-ttu-id="4e966-107">Роли каталога Azure AD также известны как *роли администратора*.</span><span class="sxs-lookup"><span data-stu-id="4e966-107">Azure AD directory roles are also known as *administrator roles*.</span></span> <span data-ttu-id="4e966-108">Для получения дополнительных сведений о ролях каталога (администратора) см. статью [Назначение ролей администратора в Azure AD](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span><span class="sxs-lookup"><span data-stu-id="4e966-108">For more information about directory (administrator) roles, see [Assigning administrator roles in Azure AD](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span> <span data-ttu-id="4e966-109">С помощью Microsoft Graph можно назначать пользователям роли каталога, чтобы предоставить им разрешения целевой роли.</span><span class="sxs-lookup"><span data-stu-id="4e966-109">With the Microsoft Graph, you can assign users to directory roles to grant them the permissions of the target role.</span></span> <span data-ttu-id="4e966-110">Чтобы можно было считать роль каталога или обновить ее членов, сначала следует активировать ее на клиенте.</span><span class="sxs-lookup"><span data-stu-id="4e966-110">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="4e966-111">По умолчанию активируется только роль каталога администраторов организации.</span><span class="sxs-lookup"><span data-stu-id="4e966-111">Only the Company Administrators directory role is activated by default.</span></span> <span data-ttu-id="4e966-112">Чтобы активировать остальные доступные роли каталога, следует отправить запрос POST с идентификатором ресурса [directoryRoleTemplate](directoryroletemplate.md), определяющего значения свойств для роли каталога.</span><span class="sxs-lookup"><span data-stu-id="4e966-112">To activate other available directory roles you send a POST request with the ID of the [directoryRoleTemplate](directoryroletemplate.md) on which the directory role is based.</span></span> <span data-ttu-id="4e966-113">[Перечислите шаблоны для ролей каталогов](../api/directoryroletemplate-list.md), чтобы получить все остальные доступные роли каталогов.</span><span class="sxs-lookup"><span data-stu-id="4e966-113">[List directory role templates](../api/directoryroletemplate-list.md) to get all the other available directory roles.</span></span> <span data-ttu-id="4e966-114">Наследуется от [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="4e966-114">Inherits from [directoryObject](directoryobject.md).</span></span>

<span data-ttu-id="4e966-115">Этот ресурс поддерживает:</span><span class="sxs-lookup"><span data-stu-id="4e966-115">This resource supports:</span></span>

- <span data-ttu-id="4e966-116">отслеживание дополнений, удалений и обновлений с помощью [запроса изменений](/graph/delta-query-overview) (функция [delta](../api/directoryrole-delta.md)).</span><span class="sxs-lookup"><span data-stu-id="4e966-116">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryrole-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="4e966-117">Методы</span><span class="sxs-lookup"><span data-stu-id="4e966-117">Methods</span></span>

| <span data-ttu-id="4e966-118">Метод</span><span class="sxs-lookup"><span data-stu-id="4e966-118">Method</span></span>       | <span data-ttu-id="4e966-119">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4e966-119">Return Type</span></span>  |<span data-ttu-id="4e966-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4e966-120">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4e966-121">Получение directoryRole</span><span class="sxs-lookup"><span data-stu-id="4e966-121">Get directoryRole</span></span>](../api/directoryrole-get.md) | [<span data-ttu-id="4e966-122">directoryRole</span><span class="sxs-lookup"><span data-stu-id="4e966-122">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="4e966-123">Считывание свойств и отношений объекта directoryRole.</span><span class="sxs-lookup"><span data-stu-id="4e966-123">Read properties and relationships of directoryRole object.</span></span> |
|[<span data-ttu-id="4e966-124">Перечисление объектов directoryRole</span><span class="sxs-lookup"><span data-stu-id="4e966-124">List directoryRoles</span></span>](../api/directoryrole-list.md) | <span data-ttu-id="4e966-125">Коллекция объектов [directoryRole](directoryrole.md)</span><span class="sxs-lookup"><span data-stu-id="4e966-125">[directoryRole](directoryrole.md) collection</span></span> | <span data-ttu-id="4e966-126">Перечисление ролей каталога, активированных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="4e966-126">List the directory roles that are activated in the tenant.</span></span> |
|[<span data-ttu-id="4e966-127">Добавление элемента</span><span class="sxs-lookup"><span data-stu-id="4e966-127">Add member</span></span>](../api/directoryrole-post-members.md) |[<span data-ttu-id="4e966-128">directoryObject</span><span class="sxs-lookup"><span data-stu-id="4e966-128">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="4e966-129">Добавление пользователя в роль каталога путем записи данных в свойство навигации members.</span><span class="sxs-lookup"><span data-stu-id="4e966-129">Add a user to the directory role by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="4e966-130">Список членов</span><span class="sxs-lookup"><span data-stu-id="4e966-130">List members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="4e966-131">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="4e966-131">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="4e966-132">Получение пользователей, которые относятся к членам роли каталога, из свойства навигации members.</span><span class="sxs-lookup"><span data-stu-id="4e966-132">Get the users that are members of the directory role from the members navigation property.</span></span>|
|[<span data-ttu-id="4e966-133">Удаление члена</span><span class="sxs-lookup"><span data-stu-id="4e966-133">Remove a member</span></span>](../api/directoryrole-delete-member.md) |[<span data-ttu-id="4e966-134">directoryObject</span><span class="sxs-lookup"><span data-stu-id="4e966-134">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="4e966-135">Удаление ресурса user из роли каталога.</span><span class="sxs-lookup"><span data-stu-id="4e966-135">Remove a user from the directory role.</span></span>|
|[<span data-ttu-id="4e966-136">Активация directoryRole</span><span class="sxs-lookup"><span data-stu-id="4e966-136">Activate directoryRole</span></span>](../api/directoryrole-post-directoryroles.md) |[<span data-ttu-id="4e966-137">directoryRole</span><span class="sxs-lookup"><span data-stu-id="4e966-137">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="4e966-138">Активация роли каталога.</span><span class="sxs-lookup"><span data-stu-id="4e966-138">Activate a directory role.</span></span>|
|[<span data-ttu-id="4e966-139">delta</span><span class="sxs-lookup"><span data-stu-id="4e966-139">delta</span></span>](../api/directoryrole-delta.md)|<span data-ttu-id="4e966-140">Коллекция объектов directoryRole</span><span class="sxs-lookup"><span data-stu-id="4e966-140">directoryRole collection</span></span>| <span data-ttu-id="4e966-141">Получение добавочных изменений для ролей каталога.</span><span class="sxs-lookup"><span data-stu-id="4e966-141">Get incremental changes for directory roles.</span></span> |

## <a name="properties"></a><span data-ttu-id="4e966-142">Свойства</span><span class="sxs-lookup"><span data-stu-id="4e966-142">Properties</span></span>
| <span data-ttu-id="4e966-143">Свойство</span><span class="sxs-lookup"><span data-stu-id="4e966-143">Property</span></span>   | <span data-ttu-id="4e966-144">Тип</span><span class="sxs-lookup"><span data-stu-id="4e966-144">Type</span></span> | <span data-ttu-id="4e966-145">Описание</span><span class="sxs-lookup"><span data-stu-id="4e966-145">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="4e966-146">description</span><span class="sxs-lookup"><span data-stu-id="4e966-146">description</span></span>|<span data-ttu-id="4e966-147">String</span><span class="sxs-lookup"><span data-stu-id="4e966-147">String</span></span>|<span data-ttu-id="4e966-p103">Описание роли каталога. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4e966-p103">The description for the directory role. Read-only.</span></span> |
|<span data-ttu-id="4e966-150">displayName</span><span class="sxs-lookup"><span data-stu-id="4e966-150">displayName</span></span>|<span data-ttu-id="4e966-151">Строка</span><span class="sxs-lookup"><span data-stu-id="4e966-151">String</span></span>|<span data-ttu-id="4e966-p104">Отображаемое имя роли каталога. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4e966-p104">The display name for the directory role. Read-only.</span></span> |
|<span data-ttu-id="4e966-154">id</span><span class="sxs-lookup"><span data-stu-id="4e966-154">id</span></span>|<span data-ttu-id="4e966-155">Строка</span><span class="sxs-lookup"><span data-stu-id="4e966-155">String</span></span>|<span data-ttu-id="4e966-p105">Уникальный идентификатор роли каталога. Наследуется из [directoryObject](directoryobject.md). Ключ, значение null не допускается, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4e966-p105">The unique identifier for the directory role. Inherited from [directoryObject](directoryobject.md). Key, Not nullable, Read-only.</span></span>|
|<span data-ttu-id="4e966-159">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="4e966-159">roleTemplateId</span></span>|<span data-ttu-id="4e966-160">String</span><span class="sxs-lookup"><span data-stu-id="4e966-160">String</span></span>| <span data-ttu-id="4e966-p106">Свойство **id** ресурса [directoryRoleTemplate](directoryroletemplate.md), определяющего значения свойств для этой роли. При активации роли каталога на клиенте следует указать свойство с помощью операции POST. После активации роли каталога свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4e966-p106">The **id** of the [directoryRoleTemplate](directoryroletemplate.md) that this role is based on. The property must be specified when activating a directory role in a tenant with a POST operation. After the directory role has been activated, the property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="4e966-164">Связи</span><span class="sxs-lookup"><span data-stu-id="4e966-164">Relationships</span></span>
| <span data-ttu-id="4e966-165">Связь</span><span class="sxs-lookup"><span data-stu-id="4e966-165">Relationship</span></span> | <span data-ttu-id="4e966-166">Тип</span><span class="sxs-lookup"><span data-stu-id="4e966-166">Type</span></span> |<span data-ttu-id="4e966-167">Описание</span><span class="sxs-lookup"><span data-stu-id="4e966-167">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4e966-168">members</span><span class="sxs-lookup"><span data-stu-id="4e966-168">members</span></span>|<span data-ttu-id="4e966-169">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="4e966-169">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="4e966-p107">Пользователи, которые относятся к членам этой роли каталога. Методы HTTP: GET, POST, DELETE. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="4e966-p107">Users that are members of this directory role. HTTP Methods: GET, POST, DELETE. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4e966-174">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4e966-174">JSON representation</span></span>

<span data-ttu-id="4e966-175">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4e966-175">Here is a JSON representation of the resource</span></span>

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
