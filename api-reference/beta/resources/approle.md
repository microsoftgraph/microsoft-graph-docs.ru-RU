---
title: тип ресурса appRole
description: Представляет роль приложения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: 06a5f97048be74388b49a79c8661b49043ddf727
ms.sourcegitcommit: aa18eb8a9965f99cc97680808abba8df46f31ba5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2021
ms.locfileid: "51638845"
---
# <a name="approle-resource-type"></a><span data-ttu-id="93a84-103">тип ресурса appRole</span><span class="sxs-lookup"><span data-stu-id="93a84-103">appRole resource type</span></span>

<span data-ttu-id="93a84-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93a84-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93a84-105">Представляет роль приложения, которую может запрашивать (и предоставлять) клиентская заявка или которую можно использовать для назначения приложения пользователям или группам в указанной роли.</span><span class="sxs-lookup"><span data-stu-id="93a84-105">Represents an application role that can be requested by (and granted to) a client application, or that can be used to assign an application to users or groups in a specified role.</span></span> 

<span data-ttu-id="93a84-106">Чтобы добавить, обновить или удалить роли приложений для приложения, [обновите](../api/application-update.md) приложение для приложения или службы.</span><span class="sxs-lookup"><span data-stu-id="93a84-106">To add, update, or remove app roles for an application, [update the application](../api/application-update.md) for the app or service.</span></span> <span data-ttu-id="93a84-107">Роли приложений в сущности приложения будут доступны всем арендаторам, где используется приложение.</span><span class="sxs-lookup"><span data-stu-id="93a84-107">App roles on the application entity will be available in all tenants where the application is used.</span></span> <span data-ttu-id="93a84-108">Чтобы определить роли приложений, применимые только в клиенте (например, роли приложений, представляющие настраиваемые [](../api/serviceprincipal-update.md) роли в экземпляре приложения с несколькими клиентами), можно также обновить главу службы для приложения, добавить или обновить роли приложений в коллекцию **appRoles.**</span><span class="sxs-lookup"><span data-stu-id="93a84-108">To define app roles that are only applicable in your tenant (for example, app roles representing custom roles in your instance of a multi-tenant application), you can also [update the service principal](../api/serviceprincipal-update.md) for the app, to add or update app roles to the **appRoles** collection.</span></span>

<span data-ttu-id="93a84-109">С [помощью appRoleAssignments](approleassignment.md)роли приложений могут быть назначены пользователям, группам или другим главам служб приложений.</span><span class="sxs-lookup"><span data-stu-id="93a84-109">With [appRoleAssignments](approleassignment.md), app roles can be assigned to users, groups, or other applications' service principals.</span></span>

## <a name="properties"></a><span data-ttu-id="93a84-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="93a84-110">Properties</span></span>

| <span data-ttu-id="93a84-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="93a84-111">Property</span></span>   | <span data-ttu-id="93a84-112">Тип</span><span class="sxs-lookup"><span data-stu-id="93a84-112">Type</span></span> |<span data-ttu-id="93a84-113">Описание</span><span class="sxs-lookup"><span data-stu-id="93a84-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="93a84-114">allowedMemberTypes</span><span class="sxs-lookup"><span data-stu-id="93a84-114">allowedMemberTypes</span></span>|<span data-ttu-id="93a84-115">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="93a84-115">String collection</span></span>|<span data-ttu-id="93a84-116">Указывает, может ли эта роль приложения быть назначена пользователям и группам (путем настройки ), другому приложению (путем настройки или обоих `["User"]` `["Application"]` (путем `["User", "Application"]` установки).</span><span class="sxs-lookup"><span data-stu-id="93a84-116">Specifies whether this app role can be assigned to users and groups (by setting to `["User"]`), to other application's (by setting to `["Application"]`, or both (by setting to `["User", "Application"]`).</span></span> <span data-ttu-id="93a84-117">Роли приложений, поддерживающие назначение для директоров служб других приложений, также [называются разрешениями приложений.](/graph/auth/auth-concepts#microsoft-graph-permissions)</span><span class="sxs-lookup"><span data-stu-id="93a84-117">App roles supporting assignment to other applications' service principals are also known as [application permissions](/graph/auth/auth-concepts#microsoft-graph-permissions).</span></span> <span data-ttu-id="93a84-118">Значение "Приложение" поддерживается только для ролей приложений, определенных для **сущностях** приложений.</span><span class="sxs-lookup"><span data-stu-id="93a84-118">The "Application" value is only supported for app roles defined on **application** entities.</span></span> |
|<span data-ttu-id="93a84-119">description</span><span class="sxs-lookup"><span data-stu-id="93a84-119">description</span></span>|<span data-ttu-id="93a84-120">String</span><span class="sxs-lookup"><span data-stu-id="93a84-120">String</span></span>|<span data-ttu-id="93a84-121">Описание роли приложения.</span><span class="sxs-lookup"><span data-stu-id="93a84-121">The description for the app role.</span></span> <span data-ttu-id="93a84-122">Это отображается при присвоении роли приложения и, если роль приложения выполняет функции разрешения приложения, во время получения согласия.</span><span class="sxs-lookup"><span data-stu-id="93a84-122">This is displayed when the app role is being assigned and, if the app role functions as an application permission, during  consent experiences.</span></span>|
|<span data-ttu-id="93a84-123">displayName</span><span class="sxs-lookup"><span data-stu-id="93a84-123">displayName</span></span>|<span data-ttu-id="93a84-124">String</span><span class="sxs-lookup"><span data-stu-id="93a84-124">String</span></span>|<span data-ttu-id="93a84-125">Отображение имени разрешения, которое отображается в задании роли приложения и опыте согласия.</span><span class="sxs-lookup"><span data-stu-id="93a84-125">Display name for the permission that appears in the app role assignment and consent experiences.</span></span>|
|<span data-ttu-id="93a84-126">id</span><span class="sxs-lookup"><span data-stu-id="93a84-126">id</span></span>|<span data-ttu-id="93a84-127">GUID</span><span class="sxs-lookup"><span data-stu-id="93a84-127">Guid</span></span>|<span data-ttu-id="93a84-128">Уникальный идентификатор роли в **коллекции appRoles.**</span><span class="sxs-lookup"><span data-stu-id="93a84-128">Unique role identifier inside the **appRoles** collection.</span></span> <span data-ttu-id="93a84-129">При создании новой роли приложения необходимо предоставлять новый идентификатор Guid.</span><span class="sxs-lookup"><span data-stu-id="93a84-129">When creating a new app role, a new Guid identifier must be provided.</span></span> |
|<span data-ttu-id="93a84-130">isEnabled</span><span class="sxs-lookup"><span data-stu-id="93a84-130">isEnabled</span></span>|<span data-ttu-id="93a84-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="93a84-131">Boolean</span></span>|<span data-ttu-id="93a84-132">При создании или обновлении роли приложения необходимо установить значение **true** (которое является по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="93a84-132">When creating or updating an app role, this must be set to **true** (which is the default).</span></span> <span data-ttu-id="93a84-133">Чтобы удалить роль, сначала необходимо установить значение **false**.</span><span class="sxs-lookup"><span data-stu-id="93a84-133">To delete a role, this must first be set to **false**.</span></span>  <span data-ttu-id="93a84-134">В этом случае при последующем вызове эта роль может быть удалена.</span><span class="sxs-lookup"><span data-stu-id="93a84-134">At that point, in a subsequent call, this role may be removed.</span></span>|
|<span data-ttu-id="93a84-135">происхождение</span><span class="sxs-lookup"><span data-stu-id="93a84-135">origin</span></span>|<span data-ttu-id="93a84-136">String</span><span class="sxs-lookup"><span data-stu-id="93a84-136">String</span></span>| <span data-ttu-id="93a84-137">Указывает, определяется ли роль приложения [](application.md) в объекте приложения или [объекте servicePrincipal.](serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="93a84-137">Specifies if the app role is defined on the [application](application.md) object or on the [servicePrincipal](serviceprincipal.md) entity.</span></span> <span data-ttu-id="93a84-138">Не _следует_ включать в запросы POST или PATCH.</span><span class="sxs-lookup"><span data-stu-id="93a84-138">Must _not_ be included in any POST or PATCH requests.</span></span> <span data-ttu-id="93a84-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="93a84-139">Read-only.</span></span> |
|<span data-ttu-id="93a84-140">value</span><span class="sxs-lookup"><span data-stu-id="93a84-140">value</span></span>|<span data-ttu-id="93a84-141">String</span><span class="sxs-lookup"><span data-stu-id="93a84-141">String</span></span>|<span data-ttu-id="93a84-142">Указывает значение, включающееся в утверждение в маркеры ID и маркеры доступа к проверке подлинности назначенного пользователя `roles` или директора службы.</span><span class="sxs-lookup"><span data-stu-id="93a84-142">Specifies the value to include in the `roles` claim in ID tokens and access tokens authenticating an assigned user or service principal.</span></span> <span data-ttu-id="93a84-143">Длина не должна превышать 120 символов.</span><span class="sxs-lookup"><span data-stu-id="93a84-143">Must not exceed 120 characters in length.</span></span> <span data-ttu-id="93a84-144">Разрешены `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~` символы, а также символы в диапазонах `0-9` и `A-Z` `a-z` .</span><span class="sxs-lookup"><span data-stu-id="93a84-144">Allowed characters are `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~`, as well as characters in the ranges `0-9`, `A-Z` and `a-z`.</span></span> <span data-ttu-id="93a84-145">Любой другой символ, включая символ пространства, не допускается.</span><span class="sxs-lookup"><span data-stu-id="93a84-145">Any other character, including the space character, are not allowed.</span></span> <span data-ttu-id="93a84-146">Может не `.` начинаться с .</span><span class="sxs-lookup"><span data-stu-id="93a84-146">May not begin with `.`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="93a84-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="93a84-147">JSON representation</span></span>

<span data-ttu-id="93a84-148">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="93a84-148">The following is a JSON representation of the resource.</span></span>

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


