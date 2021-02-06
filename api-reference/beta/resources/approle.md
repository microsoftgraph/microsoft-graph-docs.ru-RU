---
title: Тип ресурса appRole
description: Представляет роль приложения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: ff659cb8e149d952b1a27fdcbc1154b0fda49841
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136292"
---
# <a name="approle-resource-type"></a><span data-ttu-id="f9f0e-103">Тип ресурса appRole</span><span class="sxs-lookup"><span data-stu-id="f9f0e-103">appRole resource type</span></span>

<span data-ttu-id="f9f0e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9f0e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9f0e-105">Представляет роль приложения, которую может запросить (и предоставить) клиентская приложение, или которую можно использовать для назначения приложения пользователям или группам в указанной роли.</span><span class="sxs-lookup"><span data-stu-id="f9f0e-105">Represents an application role that can be requested by (and granted to) a client application, or that can be used to assign an application to users or groups in a specified role.</span></span> 

<span data-ttu-id="f9f0e-106">Свойство **appRoles** объектов [application](application.md) и [servicePrincipal](serviceprincipal.md) — это коллекция **appRole.**</span><span class="sxs-lookup"><span data-stu-id="f9f0e-106">The **appRoles** property of the [application](application.md) and [servicePrincipal](serviceprincipal.md) entities are a collection of **appRole**.</span></span> 

<span data-ttu-id="f9f0e-107">С [помощью appRoleAssignments](approleassignment.md)роли приложений могут быть назначены пользователям, группам или другим участников-служб приложений.</span><span class="sxs-lookup"><span data-stu-id="f9f0e-107">With [appRoleAssignments](approleassignment.md), app roles can be assigned to users, groups, or other applications' service principals.</span></span>

## <a name="properties"></a><span data-ttu-id="f9f0e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f9f0e-108">Properties</span></span>

| <span data-ttu-id="f9f0e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f9f0e-109">Property</span></span>   | <span data-ttu-id="f9f0e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f9f0e-110">Type</span></span> |<span data-ttu-id="f9f0e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f9f0e-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f9f0e-112">allowedMemberTypes</span><span class="sxs-lookup"><span data-stu-id="f9f0e-112">allowedMemberTypes</span></span>|<span data-ttu-id="f9f0e-113">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="f9f0e-113">String collection</span></span>|<span data-ttu-id="f9f0e-114">Указывает, может ли эта роль приложения быть назначена пользователям и группам (с помощью параметра "), другому приложению (с помощью параметра " `["User"]` `["Application"]` или "оба" (задав значение `["User", "Application"]` ).</span><span class="sxs-lookup"><span data-stu-id="f9f0e-114">Specifies whether this app role can be assigned to users and groups (by setting to `["User"]`), to other application's (by setting to `["Application"]`, or both (by setting to `["User", "Application"]`).</span></span> <span data-ttu-id="f9f0e-115">Роли приложений, поддерживающие назначение другим директорам-службам приложений, также [называются разрешениями приложений.](/graph/auth/auth-concepts#microsoft-graph-permissions)</span><span class="sxs-lookup"><span data-stu-id="f9f0e-115">App roles supporting assignment to other applications' service principals are also known as [application permissions](/graph/auth/auth-concepts#microsoft-graph-permissions).</span></span> <span data-ttu-id="f9f0e-116">Значение Application поддерживается только для ролей приложения, определенных в **сущностях** приложения.</span><span class="sxs-lookup"><span data-stu-id="f9f0e-116">The "Application" value is only supported for app roles defined on **application** entities.</span></span> |
|<span data-ttu-id="f9f0e-117">description</span><span class="sxs-lookup"><span data-stu-id="f9f0e-117">description</span></span>|<span data-ttu-id="f9f0e-118">Строка</span><span class="sxs-lookup"><span data-stu-id="f9f0e-118">String</span></span>|<span data-ttu-id="f9f0e-119">Описание роли приложения.</span><span class="sxs-lookup"><span data-stu-id="f9f0e-119">The description for the app role.</span></span> <span data-ttu-id="f9f0e-120">Это отображается при присвоении роли приложения и, если роль приложения функционирует как разрешение приложения, во время получения согласия.</span><span class="sxs-lookup"><span data-stu-id="f9f0e-120">This is displayed when the app role is being assigned and, if the app role functions as an application permission, during  consent experiences.</span></span>|
|<span data-ttu-id="f9f0e-121">displayName</span><span class="sxs-lookup"><span data-stu-id="f9f0e-121">displayName</span></span>|<span data-ttu-id="f9f0e-122">Строка</span><span class="sxs-lookup"><span data-stu-id="f9f0e-122">String</span></span>|<span data-ttu-id="f9f0e-123">Отображает имя разрешения, которое отображается в назначении роли приложения и при согласии.</span><span class="sxs-lookup"><span data-stu-id="f9f0e-123">Display name for the permission that appears in the app role assignment and consent experiences.</span></span>|
|<span data-ttu-id="f9f0e-124">id</span><span class="sxs-lookup"><span data-stu-id="f9f0e-124">id</span></span>|<span data-ttu-id="f9f0e-125">GUID</span><span class="sxs-lookup"><span data-stu-id="f9f0e-125">Guid</span></span>|<span data-ttu-id="f9f0e-126">Уникальный идентификатор роли в коллекции **appRoles.**</span><span class="sxs-lookup"><span data-stu-id="f9f0e-126">Unique role identifier inside the **appRoles** collection.</span></span> <span data-ttu-id="f9f0e-127">При создании новой роли приложения должен быть указан новый идентификатор Guid.</span><span class="sxs-lookup"><span data-stu-id="f9f0e-127">When creating a new app role, a new Guid identifier must be provided.</span></span> |
|<span data-ttu-id="f9f0e-128">isEnabled</span><span class="sxs-lookup"><span data-stu-id="f9f0e-128">isEnabled</span></span>|<span data-ttu-id="f9f0e-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="f9f0e-129">Boolean</span></span>|<span data-ttu-id="f9f0e-130">При создании или обновлении роли приложения необходимо установить значение **true** (это значение по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="f9f0e-130">When creating or updating an app role, this must be set to **true** (which is the default).</span></span> <span data-ttu-id="f9f0e-131">Чтобы удалить роль, сначала необходимо установить значение **false.**</span><span class="sxs-lookup"><span data-stu-id="f9f0e-131">To delete a role, this must first be set to **false**.</span></span>  <span data-ttu-id="f9f0e-132">На этом этапе в последующем вызове эта роль может быть удалена.</span><span class="sxs-lookup"><span data-stu-id="f9f0e-132">At that point, in a subsequent call, this role may be removed.</span></span>|
|<span data-ttu-id="f9f0e-133">origin</span><span class="sxs-lookup"><span data-stu-id="f9f0e-133">origin</span></span>|<span data-ttu-id="f9f0e-134">Строка</span><span class="sxs-lookup"><span data-stu-id="f9f0e-134">String</span></span>| <span data-ttu-id="f9f0e-135">Указывает, определена ли роль приложения в объекте [приложения](application.md) или [объекте servicePrincipal.](serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="f9f0e-135">Specifies if the app role is defined on the [application](application.md) object or on the [servicePrincipal](serviceprincipal.md) entity.</span></span> <span data-ttu-id="f9f0e-136">Не _должен_ включаться в запросы POST или PATCH.</span><span class="sxs-lookup"><span data-stu-id="f9f0e-136">Must _not_ be included in any POST or PATCH requests.</span></span> <span data-ttu-id="f9f0e-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f9f0e-137">Read-only.</span></span> |
|<span data-ttu-id="f9f0e-138">value</span><span class="sxs-lookup"><span data-stu-id="f9f0e-138">value</span></span>|<span data-ttu-id="f9f0e-139">String</span><span class="sxs-lookup"><span data-stu-id="f9f0e-139">String</span></span>|<span data-ttu-id="f9f0e-140">Указывает значение, включающееся в утверждение в маркеры ID и маркеры доступа, которые аутентификация назначенного пользователя `roles` или основного пользователя службы.</span><span class="sxs-lookup"><span data-stu-id="f9f0e-140">Specifies the value to include in the `roles` claim in ID tokens and access tokens authenticating an assigned user or service principal.</span></span> <span data-ttu-id="f9f0e-141">Длина не должна превышать 120 символов.</span><span class="sxs-lookup"><span data-stu-id="f9f0e-141">Must not exceed 120 characters in length.</span></span> <span data-ttu-id="f9f0e-142">Допустимые `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~` символы: и символы в `0-9` диапазонах, `A-Z` и `a-z` .</span><span class="sxs-lookup"><span data-stu-id="f9f0e-142">Allowed characters are `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~`, as well as characters in the ranges `0-9`, `A-Z` and `a-z`.</span></span> <span data-ttu-id="f9f0e-143">Любые другие символы, включая пробелы, не допускаются.</span><span class="sxs-lookup"><span data-stu-id="f9f0e-143">Any other character, including the space character, are not allowed.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="f9f0e-144">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f9f0e-144">JSON representation</span></span>

<span data-ttu-id="f9f0e-145">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f9f0e-145">The following is a JSON representation of the resource.</span></span>

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


