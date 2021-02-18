---
title: Тип ресурса appRole
description: Представляет роль приложения, которую может запросить клиентская приложение, вызывающую другое приложение, или которая может использоваться для назначения приложения пользователям или группам в указанной роли приложения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: ee38168920dee5c836be6801a7f63181df565eb5
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272501"
---
# <a name="approle-resource-type"></a><span data-ttu-id="35d9a-103">Тип ресурса appRole</span><span class="sxs-lookup"><span data-stu-id="35d9a-103">appRole resource type</span></span>

<span data-ttu-id="35d9a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35d9a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="35d9a-105">Представляет роль приложения, которую может запросить (и предоставить) клиентская приложение, или которую можно использовать для назначения приложения пользователям или группам в указанной роли.</span><span class="sxs-lookup"><span data-stu-id="35d9a-105">Represents an application role that can be requested by (and granted to) a client application, or that can be used to assign an application to users or groups in a specified role.</span></span> 

<span data-ttu-id="35d9a-106">Чтобы добавить, обновить или удалить роли приложения для [приложения,](../api/application-update.md) обновите приложение для приложения или службы.</span><span class="sxs-lookup"><span data-stu-id="35d9a-106">To add, update, or remove app roles for an application, [update the application](../api/application-update.md) for the app or service.</span></span> <span data-ttu-id="35d9a-107">Роли приложений в объекте приложения будут доступны во всех клиентах, где используется приложение.</span><span class="sxs-lookup"><span data-stu-id="35d9a-107">App roles on the application entity will be available in all tenants where the application is used.</span></span> <span data-ttu-id="35d9a-108">Чтобы определить роли приложения, применимые только в клиенте (например, роли приложения, представляющие настраиваемые [](../api/serviceprincipal-update.md) роли в экземпляре мультиантианого приложения), можно также обновить для приложения основной службы, чтобы добавить или обновить роли приложения в коллекцию **appRoles.**</span><span class="sxs-lookup"><span data-stu-id="35d9a-108">To define app roles that are only applicable in your tenant (for example, app roles representing custom roles in your instance of a multi-tenant application), you can also [update the service principal](../api/serviceprincipal-update.md) for the app, to add or update app roles to the **appRoles** collection.</span></span>

<span data-ttu-id="35d9a-109">С [помощью appRoleAssignments](approleassignment.md)роли приложений могут быть назначены пользователям, группам или другим участников-служб приложений.</span><span class="sxs-lookup"><span data-stu-id="35d9a-109">With [appRoleAssignments](approleassignment.md), app roles can be assigned to users, groups, or other applications' service principals.</span></span>

## <a name="properties"></a><span data-ttu-id="35d9a-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="35d9a-110">Properties</span></span>

| <span data-ttu-id="35d9a-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="35d9a-111">Property</span></span>   | <span data-ttu-id="35d9a-112">Тип</span><span class="sxs-lookup"><span data-stu-id="35d9a-112">Type</span></span> |<span data-ttu-id="35d9a-113">Описание</span><span class="sxs-lookup"><span data-stu-id="35d9a-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="35d9a-114">allowedMemberTypes</span><span class="sxs-lookup"><span data-stu-id="35d9a-114">allowedMemberTypes</span></span>|<span data-ttu-id="35d9a-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="35d9a-115">String collection</span></span>|<span data-ttu-id="35d9a-116">Указывает, может ли эта роль приложения быть назначена пользователям и группам (с помощью параметра "), другому приложению (с помощью параметра ", или и то, и другое( с помощью параметра `["User"]` `["Application"]` `["User", "Application"]` ").</span><span class="sxs-lookup"><span data-stu-id="35d9a-116">Specifies whether this app role can be assigned to users and groups (by setting to `["User"]`), to other application's (by setting to `["Application"]`, or both (by setting to `["User", "Application"]`).</span></span> <span data-ttu-id="35d9a-117">Роли приложений, поддерживающие назначение другим директорам-службам приложений, также [называются разрешениями приложений.](/graph/auth/auth-concepts#microsoft-graph-permissions)</span><span class="sxs-lookup"><span data-stu-id="35d9a-117">App roles supporting assignment to other applications' service principals are also known as [application permissions](/graph/auth/auth-concepts#microsoft-graph-permissions).</span></span> <span data-ttu-id="35d9a-118">Значение Application поддерживается только для ролей приложения, определенных в **сущностях** приложения.</span><span class="sxs-lookup"><span data-stu-id="35d9a-118">The "Application" value is only supported for app roles defined on **application** entities.</span></span>|
|<span data-ttu-id="35d9a-119">description</span><span class="sxs-lookup"><span data-stu-id="35d9a-119">description</span></span>|<span data-ttu-id="35d9a-120">String</span><span class="sxs-lookup"><span data-stu-id="35d9a-120">String</span></span>|<span data-ttu-id="35d9a-121">Описание роли приложения.</span><span class="sxs-lookup"><span data-stu-id="35d9a-121">The description for the app role.</span></span> <span data-ttu-id="35d9a-122">Это отображается при присвоении роли приложения и, если роль приложения функционирует как разрешение приложения, во время получения согласия.</span><span class="sxs-lookup"><span data-stu-id="35d9a-122">This is displayed when the app role is being assigned and, if the app role functions as an application permission, during  consent experiences.</span></span>|
|<span data-ttu-id="35d9a-123">displayName</span><span class="sxs-lookup"><span data-stu-id="35d9a-123">displayName</span></span>|<span data-ttu-id="35d9a-124">String</span><span class="sxs-lookup"><span data-stu-id="35d9a-124">String</span></span>|<span data-ttu-id="35d9a-125">Отображает имя разрешения, которое отображается в назначении роли приложения и при согласии.</span><span class="sxs-lookup"><span data-stu-id="35d9a-125">Display name for the permission that appears in the app role assignment and consent experiences.</span></span>|
|<span data-ttu-id="35d9a-126">id</span><span class="sxs-lookup"><span data-stu-id="35d9a-126">id</span></span>|<span data-ttu-id="35d9a-127">GUID</span><span class="sxs-lookup"><span data-stu-id="35d9a-127">Guid</span></span>|<span data-ttu-id="35d9a-128">Уникальный идентификатор роли в коллекции **appRoles.**</span><span class="sxs-lookup"><span data-stu-id="35d9a-128">Unique role identifier inside the **appRoles** collection.</span></span> <span data-ttu-id="35d9a-129">При создании новой роли приложения должен быть указан новый идентификатор Guid.</span><span class="sxs-lookup"><span data-stu-id="35d9a-129">When creating a new app role, a new Guid identifier must be provided.</span></span> |
|<span data-ttu-id="35d9a-130">isEnabled</span><span class="sxs-lookup"><span data-stu-id="35d9a-130">isEnabled</span></span>|<span data-ttu-id="35d9a-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="35d9a-131">Boolean</span></span>|<span data-ttu-id="35d9a-132">При создании или обновлении роли приложения необходимо установить значение **true** (это значение по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="35d9a-132">When creating or updating an app role, this must be set to **true** (which is the default).</span></span> <span data-ttu-id="35d9a-133">Чтобы удалить роль, сначала необходимо установить значение **false.**</span><span class="sxs-lookup"><span data-stu-id="35d9a-133">To delete a role, this must first be set to **false**.</span></span>  <span data-ttu-id="35d9a-134">На этом этапе в последующем вызове эта роль может быть удалена.</span><span class="sxs-lookup"><span data-stu-id="35d9a-134">At that point, in a subsequent call, this role may be removed.</span></span>|
|<span data-ttu-id="35d9a-135">origin</span><span class="sxs-lookup"><span data-stu-id="35d9a-135">origin</span></span>|<span data-ttu-id="35d9a-136">String</span><span class="sxs-lookup"><span data-stu-id="35d9a-136">String</span></span>| <span data-ttu-id="35d9a-137">Указывает, определена ли роль приложения в объекте [приложения](application.md) или [объекте servicePrincipal.](serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="35d9a-137">Specifies if the app role is defined on the [application](application.md) object or on the [servicePrincipal](serviceprincipal.md) entity.</span></span> <span data-ttu-id="35d9a-138">Не _должен_ включаться в запросы POST или PATCH.</span><span class="sxs-lookup"><span data-stu-id="35d9a-138">Must _not_ be included in any POST or PATCH requests.</span></span> <span data-ttu-id="35d9a-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="35d9a-139">Read-only.</span></span> |
|<span data-ttu-id="35d9a-140">value</span><span class="sxs-lookup"><span data-stu-id="35d9a-140">value</span></span>|<span data-ttu-id="35d9a-141">String</span><span class="sxs-lookup"><span data-stu-id="35d9a-141">String</span></span>|<span data-ttu-id="35d9a-142">Указывает значение, включающееся в утверждение в маркеры ID и маркеры доступа, которые аутентификация назначенного пользователя `roles` или основного пользователя службы.</span><span class="sxs-lookup"><span data-stu-id="35d9a-142">Specifies the value to include in the `roles` claim in ID tokens and access tokens authenticating an assigned user or service principal.</span></span> <span data-ttu-id="35d9a-143">Длина не должна превышать 120 символов.</span><span class="sxs-lookup"><span data-stu-id="35d9a-143">Must not exceed 120 characters in length.</span></span> <span data-ttu-id="35d9a-144">Допустимые `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~` символы: и символы в `0-9` диапазонах, `A-Z` и `a-z` .</span><span class="sxs-lookup"><span data-stu-id="35d9a-144">Allowed characters are `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~`, as well as characters in the ranges `0-9`, `A-Z` and `a-z`.</span></span> <span data-ttu-id="35d9a-145">Любые другие символы, включая пробелы, не допускаются.</span><span class="sxs-lookup"><span data-stu-id="35d9a-145">Any other character, including the space character, are not allowed.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="35d9a-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="35d9a-146">JSON representation</span></span>

<span data-ttu-id="35d9a-147">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="35d9a-147">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.appRole"
}-->

```json
{
  "allowedMemberTypes": ["string"],
  "description": "string",
  "displayName": "string",
  "id": "guid",
  "isEnabled": true,
  "origin": "string",
  "value": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "appRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

