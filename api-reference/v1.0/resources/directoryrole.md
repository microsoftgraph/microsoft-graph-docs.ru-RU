---
title: Тип ресурса directoryRole
description: Представляет роль каталога Azure AD. Роли каталога Azure AD также известны как *роли администратора*.
localization_priority: Priority
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d9b500e3f5a3768dd345d1e7e8df41c63b1aa54b
ms.sourcegitcommit: 9cd96fcbaae9d2ebaa3f3b69e440a1aea106f535
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/17/2019
ms.locfileid: "36450678"
---
# <a name="directoryrole-resource-type"></a><span data-ttu-id="64ace-104">Тип ресурса directoryRole</span><span class="sxs-lookup"><span data-stu-id="64ace-104">directoryRole resource type</span></span>

<span data-ttu-id="64ace-105">Представляет роль каталога Azure AD.</span><span class="sxs-lookup"><span data-stu-id="64ace-105">Represents an Azure AD directory role.</span></span> <span data-ttu-id="64ace-106">Роли каталога Azure AD также известны как *роли администратора*.</span><span class="sxs-lookup"><span data-stu-id="64ace-106">Azure AD directory roles are also known as *administrator roles*.</span></span> <span data-ttu-id="64ace-107">Для получения дополнительных сведений о ролях каталога (администратора) см. статью [Назначение ролей администратора в Azure AD](http://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/).</span><span class="sxs-lookup"><span data-stu-id="64ace-107">For more information about directory (administrator) roles, see [Assigning administrator roles in Azure AD](http://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/).</span></span> <span data-ttu-id="64ace-108">С помощью Microsoft Graph можно назначать пользователям роли каталога, чтобы предоставить им разрешения целевой роли.</span><span class="sxs-lookup"><span data-stu-id="64ace-108">With the Microsoft Graph, you can assign users to directory roles to grant them the permissions of the target role.</span></span> <span data-ttu-id="64ace-109">Чтобы можно было считать роль каталога или обновить ее членов, сначала следует активировать ее на клиенте.</span><span class="sxs-lookup"><span data-stu-id="64ace-109">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="64ace-110">По умолчанию активируется только роль каталога администраторов организации.</span><span class="sxs-lookup"><span data-stu-id="64ace-110">Only the Company Administrators directory role is activated by default.</span></span> <span data-ttu-id="64ace-111">Чтобы активировать остальные доступные роли каталога, следует отправить запрос POST с идентификатором ресурса [directoryRoleTemplate](directoryroletemplate.md), определяющего значения свойств для роли каталога.</span><span class="sxs-lookup"><span data-stu-id="64ace-111">To activate other available directory roles you send a POST request with the ID of the [directoryRoleTemplate](directoryroletemplate.md) on which the directory role is based.</span></span> <span data-ttu-id="64ace-112">[Перечислите шаблоны для ролей каталогов](../api/directoryroletemplate-list.md), чтобы получить все остальные доступные роли каталогов.</span><span class="sxs-lookup"><span data-stu-id="64ace-112">[List directory role templates](../api/directoryroletemplate-list.md) to get all the other available directory roles.</span></span> <span data-ttu-id="64ace-113">Наследуется от [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="64ace-113">Inherits from [directoryObject](directoryobject.md).</span></span>

<span data-ttu-id="64ace-114">Этот ресурс поддерживает:</span><span class="sxs-lookup"><span data-stu-id="64ace-114">This resource supports:</span></span>

- <span data-ttu-id="64ace-115">отслеживание дополнений, удалений и обновлений с помощью [запроса изменений](/graph/delta-query-overview) (функция [delta](../api/directoryrole-delta.md)).</span><span class="sxs-lookup"><span data-stu-id="64ace-115">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryrole-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="64ace-116">Методы</span><span class="sxs-lookup"><span data-stu-id="64ace-116">Methods</span></span>

| <span data-ttu-id="64ace-117">Метод</span><span class="sxs-lookup"><span data-stu-id="64ace-117">Method</span></span>       | <span data-ttu-id="64ace-118">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="64ace-118">Return Type</span></span>  |<span data-ttu-id="64ace-119">Описание</span><span class="sxs-lookup"><span data-stu-id="64ace-119">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="64ace-120">Получение directoryRole</span><span class="sxs-lookup"><span data-stu-id="64ace-120">Get directoryRole</span></span>](../api/directoryrole-get.md) | [<span data-ttu-id="64ace-121">directoryRole</span><span class="sxs-lookup"><span data-stu-id="64ace-121">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="64ace-122">Считывание свойств и отношений объекта directoryRole.</span><span class="sxs-lookup"><span data-stu-id="64ace-122">Read properties and relationships of directoryRole object.</span></span> |
|[<span data-ttu-id="64ace-123">Перечисление объектов directoryRole</span><span class="sxs-lookup"><span data-stu-id="64ace-123">List directoryRoles</span></span>](../api/directoryrole-list.md) | <span data-ttu-id="64ace-124">Коллекция объектов [directoryRole](directoryrole.md)</span><span class="sxs-lookup"><span data-stu-id="64ace-124">[directoryRole](directoryrole.md) collection</span></span> | <span data-ttu-id="64ace-125">Перечисление ролей каталога, активированных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="64ace-125">List the directory roles that are activated in the tenant.</span></span> |
|[<span data-ttu-id="64ace-126">Добавление элемента</span><span class="sxs-lookup"><span data-stu-id="64ace-126">Add member</span></span>](../api/directoryrole-post-members.md) |[<span data-ttu-id="64ace-127">directoryObject</span><span class="sxs-lookup"><span data-stu-id="64ace-127">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="64ace-128">Добавление пользователя в роль каталога путем записи данных в свойство навигации members.</span><span class="sxs-lookup"><span data-stu-id="64ace-128">Add a user to the directory role by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="64ace-129">Список членов</span><span class="sxs-lookup"><span data-stu-id="64ace-129">List members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="64ace-130">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="64ace-130">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="64ace-131">Получение пользователей, которые относятся к членам роли каталога, из свойства навигации members.</span><span class="sxs-lookup"><span data-stu-id="64ace-131">Get the users that are members of the directory role from the members navigation property.</span></span>|
|[<span data-ttu-id="64ace-132">Удаление члена</span><span class="sxs-lookup"><span data-stu-id="64ace-132">Remove a member</span></span>](../api/directoryrole-delete-member.md) |[<span data-ttu-id="64ace-133">directoryObject</span><span class="sxs-lookup"><span data-stu-id="64ace-133">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="64ace-134">Удаление ресурса user из роли каталога.</span><span class="sxs-lookup"><span data-stu-id="64ace-134">Remove a user from the directory role.</span></span>|
|[<span data-ttu-id="64ace-135">Активация directoryRole</span><span class="sxs-lookup"><span data-stu-id="64ace-135">Activate directoryRole</span></span>](../api/directoryrole-post-directoryroles.md) |[<span data-ttu-id="64ace-136">directoryRole</span><span class="sxs-lookup"><span data-stu-id="64ace-136">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="64ace-137">Активация роли каталога.</span><span class="sxs-lookup"><span data-stu-id="64ace-137">Activate a directory role.</span></span>|
|[<span data-ttu-id="64ace-138">delta</span><span class="sxs-lookup"><span data-stu-id="64ace-138">delta</span></span>](../api/directoryrole-delta.md)|<span data-ttu-id="64ace-139">Коллекция объектов directoryRole</span><span class="sxs-lookup"><span data-stu-id="64ace-139">directoryRole collection</span></span>| <span data-ttu-id="64ace-140">Получение добавочных изменений для ролей каталога.</span><span class="sxs-lookup"><span data-stu-id="64ace-140">Get incremental changes for directory roles.</span></span> |

## <a name="properties"></a><span data-ttu-id="64ace-141">Свойства</span><span class="sxs-lookup"><span data-stu-id="64ace-141">Properties</span></span>
| <span data-ttu-id="64ace-142">Свойство</span><span class="sxs-lookup"><span data-stu-id="64ace-142">Property</span></span>   | <span data-ttu-id="64ace-143">Тип</span><span class="sxs-lookup"><span data-stu-id="64ace-143">Type</span></span> | <span data-ttu-id="64ace-144">Описание</span><span class="sxs-lookup"><span data-stu-id="64ace-144">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="64ace-145">description</span><span class="sxs-lookup"><span data-stu-id="64ace-145">description</span></span>|<span data-ttu-id="64ace-146">String</span><span class="sxs-lookup"><span data-stu-id="64ace-146">String</span></span>|<span data-ttu-id="64ace-p103">Описание роли каталога. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="64ace-p103">The description for the directory role. Read-only.</span></span> |
|<span data-ttu-id="64ace-149">displayName</span><span class="sxs-lookup"><span data-stu-id="64ace-149">displayName</span></span>|<span data-ttu-id="64ace-150">Строка</span><span class="sxs-lookup"><span data-stu-id="64ace-150">String</span></span>|<span data-ttu-id="64ace-p104">Отображаемое имя роли каталога. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="64ace-p104">The display name for the directory role. Read-only.</span></span> |
|<span data-ttu-id="64ace-153">id</span><span class="sxs-lookup"><span data-stu-id="64ace-153">id</span></span>|<span data-ttu-id="64ace-154">Строка</span><span class="sxs-lookup"><span data-stu-id="64ace-154">String</span></span>|<span data-ttu-id="64ace-p105">Уникальный идентификатор роли каталога. Наследуется из [directoryObject](directoryobject.md). Ключ, значение null не допускается, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="64ace-p105">The unique identifier for the directory role. Inherited from [directoryObject](directoryobject.md). Key, Not nullable, Read-only.</span></span>|
|<span data-ttu-id="64ace-158">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="64ace-158">roleTemplateId</span></span>|<span data-ttu-id="64ace-159">String</span><span class="sxs-lookup"><span data-stu-id="64ace-159">String</span></span>| <span data-ttu-id="64ace-p106">Свойство **id** ресурса [directoryRoleTemplate](directoryroletemplate.md), определяющего значения свойств для этой роли. При активации роли каталога на клиенте следует указать свойство с помощью операции POST. После активации роли каталога свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="64ace-p106">The **id** of the [directoryRoleTemplate](directoryroletemplate.md) that this role is based on. The property must be specified when activating a directory role in a tenant with a POST operation. After the directory role has been activated, the property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="64ace-163">Связи</span><span class="sxs-lookup"><span data-stu-id="64ace-163">Relationships</span></span>
| <span data-ttu-id="64ace-164">Отношение</span><span class="sxs-lookup"><span data-stu-id="64ace-164">Relationship</span></span> | <span data-ttu-id="64ace-165">Тип</span><span class="sxs-lookup"><span data-stu-id="64ace-165">Type</span></span> |<span data-ttu-id="64ace-166">Описание</span><span class="sxs-lookup"><span data-stu-id="64ace-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="64ace-167">members</span><span class="sxs-lookup"><span data-stu-id="64ace-167">members</span></span>|<span data-ttu-id="64ace-168">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="64ace-168">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="64ace-p107">Пользователи, которые относятся к членам этой роли каталога. Методы HTTP: GET, POST, DELETE. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="64ace-p107">Users that are members of this directory role. HTTP Methods: GET, POST, DELETE. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="64ace-173">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="64ace-173">JSON representation</span></span>

<span data-ttu-id="64ace-174">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="64ace-174">Here is a JSON representation of the resource</span></span>

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
