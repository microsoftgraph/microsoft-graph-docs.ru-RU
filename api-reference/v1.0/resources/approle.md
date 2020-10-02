---
title: Тип ресурса Аппроле
description: Представляет роль приложения, которая может быть запрошена клиентским приложением, вызывающей другое приложение, или которая может использоваться для назначения приложения пользователям или группам в указанной роли приложения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: d094a91ca7e8b923322853fbdabcf63e65e2082d
ms.sourcegitcommit: 7370fb65d11d1347123a3f6d320d2c6d36f34224
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2020
ms.locfileid: "48338167"
---
# <a name="approle-resource-type"></a><span data-ttu-id="7fb51-103">Тип ресурса Аппроле</span><span class="sxs-lookup"><span data-stu-id="7fb51-103">appRole resource type</span></span>

<span data-ttu-id="7fb51-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7fb51-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7fb51-105">Представляет роль приложения, которая может быть запрошена клиентским приложением (и предоставлена ей), или с помощью которой можно назначить приложение пользователям или группам в указанной роли.</span><span class="sxs-lookup"><span data-stu-id="7fb51-105">Represents an application role that can be requested by (and granted to) a client application, or that can be used to assign an application to users or groups in a specified role.</span></span> 

<span data-ttu-id="7fb51-106">Свойство **appRoles** сущностей [Application](application.md) и [servicePrincipal](serviceprincipal.md) является коллекцией **аппроле**.</span><span class="sxs-lookup"><span data-stu-id="7fb51-106">The **appRoles** property of the [application](application.md) and [servicePrincipal](serviceprincipal.md) entities are a collection of **appRole**.</span></span> 

<span data-ttu-id="7fb51-107">С помощью [аппролеассигнментс](approleassignment.md)роли приложений могут быть назначены пользователям, группам или субъектам служб других приложений.</span><span class="sxs-lookup"><span data-stu-id="7fb51-107">With [appRoleAssignments](approleassignment.md), app roles can be assigned to users, groups, or other applications' service principals.</span></span>

## <a name="properties"></a><span data-ttu-id="7fb51-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="7fb51-108">Properties</span></span>

| <span data-ttu-id="7fb51-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="7fb51-109">Property</span></span>   | <span data-ttu-id="7fb51-110">Тип</span><span class="sxs-lookup"><span data-stu-id="7fb51-110">Type</span></span> |<span data-ttu-id="7fb51-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7fb51-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7fb51-112">алловедмембертипес</span><span class="sxs-lookup"><span data-stu-id="7fb51-112">allowedMemberTypes</span></span>|<span data-ttu-id="7fb51-113">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="7fb51-113">String collection</span></span>|<span data-ttu-id="7fb51-114">Указывает, может ли эта роль приложения назначаться пользователям и группам (с помощью параметра `["User"]` ), другим приложениям (по значению `["Application"]` или обоим `["User", "Application"]` ).</span><span class="sxs-lookup"><span data-stu-id="7fb51-114">Specifies whether this app role can be assigned to users and groups (by setting to `["User"]`), to other application's (by setting to `["Application"]`, or both (by setting to `["User", "Application"]`).</span></span> <span data-ttu-id="7fb51-115">Роли приложений, поддерживающие назначение для других субъектов служб приложений, также называются [разрешениями приложений](/graph/auth/auth-concepts#microsoft-graph-permissions).</span><span class="sxs-lookup"><span data-stu-id="7fb51-115">App roles supporting assignment to other applications' service principals are also known as [application permissions](/graph/auth/auth-concepts#microsoft-graph-permissions).</span></span> <span data-ttu-id="7fb51-116">Значение Application поддерживается только для ролей приложения, определенных для сущностей **приложения** .</span><span class="sxs-lookup"><span data-stu-id="7fb51-116">The "Application" value is only supported for app roles defined on **application** entities.</span></span>|
|<span data-ttu-id="7fb51-117">description</span><span class="sxs-lookup"><span data-stu-id="7fb51-117">description</span></span>|<span data-ttu-id="7fb51-118">Строка</span><span class="sxs-lookup"><span data-stu-id="7fb51-118">String</span></span>|<span data-ttu-id="7fb51-119">Описание роли приложения.</span><span class="sxs-lookup"><span data-stu-id="7fb51-119">The description for the app role.</span></span> <span data-ttu-id="7fb51-120">Он отображается при назначении роли приложения и, если роль приложения работает как разрешение приложения, во время предоставления согласия.</span><span class="sxs-lookup"><span data-stu-id="7fb51-120">This is displayed when the app role is being assigned and, if the app role functions as an application permission, during  consent experiences.</span></span>|
|<span data-ttu-id="7fb51-121">displayName</span><span class="sxs-lookup"><span data-stu-id="7fb51-121">displayName</span></span>|<span data-ttu-id="7fb51-122">Строка</span><span class="sxs-lookup"><span data-stu-id="7fb51-122">String</span></span>|<span data-ttu-id="7fb51-123">Отображаемое имя разрешения, которое отображается при назначении роли приложения и согласия пользователя.</span><span class="sxs-lookup"><span data-stu-id="7fb51-123">Display name for the permission that appears in the app role assignment and consent experiences.</span></span>|
|<span data-ttu-id="7fb51-124">id</span><span class="sxs-lookup"><span data-stu-id="7fb51-124">id</span></span>|<span data-ttu-id="7fb51-125">GUID</span><span class="sxs-lookup"><span data-stu-id="7fb51-125">Guid</span></span>|<span data-ttu-id="7fb51-126">Уникальный идентификатор роли в семействе **appRoles** .</span><span class="sxs-lookup"><span data-stu-id="7fb51-126">Unique role identifier inside the **appRoles** collection.</span></span> <span data-ttu-id="7fb51-127">При создании новой роли приложения необходимо указать новый идентификатор GUID.</span><span class="sxs-lookup"><span data-stu-id="7fb51-127">When creating a new app role, a new Guid identifier must be provided.</span></span> |
|<span data-ttu-id="7fb51-128">isEnabled</span><span class="sxs-lookup"><span data-stu-id="7fb51-128">isEnabled</span></span>|<span data-ttu-id="7fb51-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="7fb51-129">Boolean</span></span>|<span data-ttu-id="7fb51-130">При создании или обновлении роли приложения должно быть задано **значение true** (значение по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="7fb51-130">When creating or updating an app role, this must be set to **true** (which is the default).</span></span> <span data-ttu-id="7fb51-131">Чтобы удалить роль, необходимо сначала задать значение **false**.</span><span class="sxs-lookup"><span data-stu-id="7fb51-131">To delete a role, this must first be set to **false**.</span></span>  <span data-ttu-id="7fb51-132">В этот момент эта роль может быть удалена в последующих вызовах.</span><span class="sxs-lookup"><span data-stu-id="7fb51-132">At that point, in a subsequent call, this role may be removed.</span></span>|
|<span data-ttu-id="7fb51-133">основания</span><span class="sxs-lookup"><span data-stu-id="7fb51-133">origin</span></span>|<span data-ttu-id="7fb51-134">Строка</span><span class="sxs-lookup"><span data-stu-id="7fb51-134">String</span></span>| <span data-ttu-id="7fb51-135">Указывает, определена ли роль приложения для объекта [Application](application.md) или объекта [servicePrincipal](serviceprincipal.md) .</span><span class="sxs-lookup"><span data-stu-id="7fb51-135">Specifies if the app role is defined on the [application](application.md) object or on the [servicePrincipal](serviceprincipal.md) entity.</span></span> <span data-ttu-id="7fb51-136">_Не_ следует включать в запросы POST или patch.</span><span class="sxs-lookup"><span data-stu-id="7fb51-136">Must _not_ be included in any POST or PATCH requests.</span></span> <span data-ttu-id="7fb51-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7fb51-137">Read-only.</span></span> |
|<span data-ttu-id="7fb51-138">value</span><span class="sxs-lookup"><span data-stu-id="7fb51-138">value</span></span>|<span data-ttu-id="7fb51-139">String</span><span class="sxs-lookup"><span data-stu-id="7fb51-139">String</span></span>|<span data-ttu-id="7fb51-140">Указывает значение, которое будет включено в `roles` утверждения маркеров идентификаторов и маркеров доступа, которые проходят проверку подлинности назначенного пользователя или участника службы.</span><span class="sxs-lookup"><span data-stu-id="7fb51-140">Specifies the value to include in the `roles` claim in ID tokens and access tokens authenticating an assigned user or service principal.</span></span> <span data-ttu-id="7fb51-141">Длина не должна превышать 120 символов.</span><span class="sxs-lookup"><span data-stu-id="7fb51-141">Must not exceed 120 characters in length.</span></span> <span data-ttu-id="7fb51-142">Допустимые знаки `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~` , а также символы в диапазонах `0-9` `A-Z` и `a-z` .</span><span class="sxs-lookup"><span data-stu-id="7fb51-142">Allowed characters are `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~`, as well as characters in the ranges `0-9`, `A-Z` and `a-z`.</span></span> <span data-ttu-id="7fb51-143">Любой другой символ, в том числе символ пробела, не допускается.</span><span class="sxs-lookup"><span data-stu-id="7fb51-143">Any other character, including the space character, are not allowed.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="7fb51-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7fb51-144">JSON representation</span></span>

<span data-ttu-id="7fb51-145">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7fb51-145">The following is a JSON representation of the resource.</span></span>

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

