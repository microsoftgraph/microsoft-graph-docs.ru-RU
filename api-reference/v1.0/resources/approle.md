---
title: Тип ресурса Аппроле
description: Представляет роль приложения, которая может быть запрошена клиентским приложением для вызова другого приложения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 2bda5d65d71873c1427ae99ded550962ad135433
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533144"
---
# <a name="approle-resource-type"></a><span data-ttu-id="ea6f1-103">Тип ресурса Аппроле</span><span class="sxs-lookup"><span data-stu-id="ea6f1-103">appRole resource type</span></span>

<span data-ttu-id="ea6f1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea6f1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ea6f1-105">Представляет роль приложения, которая может быть запрошена клиентским приложением, вызывающей другое приложение, или которая может использоваться для назначения приложения пользователям или группам в указанной роли приложения.</span><span class="sxs-lookup"><span data-stu-id="ea6f1-105">Represents an application role that may be requested by a client application calling another application or that may be used to assign an application to users or groups in a specified application role.</span></span> <span data-ttu-id="ea6f1-106">Свойство **appRoles**</span><span class="sxs-lookup"><span data-stu-id="ea6f1-106">The **appRoles** property</span></span> <!-- of the [servicePrincipal](serviceprincipal.md) entity and --> <span data-ttu-id="ea6f1-107">объекта [Application](application.md) — коллекция **аппроле**.</span><span class="sxs-lookup"><span data-stu-id="ea6f1-107">of the [application](application.md) entity is a collection of **appRole**.</span></span>

## <a name="properties"></a><span data-ttu-id="ea6f1-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ea6f1-108">Properties</span></span>
| <span data-ttu-id="ea6f1-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ea6f1-109">Property</span></span>     | <span data-ttu-id="ea6f1-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ea6f1-110">Type</span></span>   |<span data-ttu-id="ea6f1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ea6f1-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ea6f1-112">алловедмембертипес</span><span class="sxs-lookup"><span data-stu-id="ea6f1-112">allowedMemberTypes</span></span>|<span data-ttu-id="ea6f1-113">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ea6f1-113">String collection</span></span>|<span data-ttu-id="ea6f1-114">Указывает, можно ли назначить это определение роли приложения пользователям и группам, задав для параметра значение "пользователь" или другие приложения (которые обращаются к этому приложению в сценариях службы демона), задав значение "Application" или как то, и другое.</span><span class="sxs-lookup"><span data-stu-id="ea6f1-114">Specifies whether this app role definition can be assigned to users and groups by setting to "User", or to other applications (that are accessing this application in daemon service scenarios) by setting to "Application", or to both.</span></span>|
|<span data-ttu-id="ea6f1-115">description</span><span class="sxs-lookup"><span data-stu-id="ea6f1-115">description</span></span>|<span data-ttu-id="ea6f1-116">String</span><span class="sxs-lookup"><span data-stu-id="ea6f1-116">String</span></span>|<span data-ttu-id="ea6f1-117">Текст справки по разрешениям, который отображается при назначении и согласии приложения администрирования.</span><span class="sxs-lookup"><span data-stu-id="ea6f1-117">Permission help text that appears in the admin app assignment and consent experiences.</span></span>|
|<span data-ttu-id="ea6f1-118">displayName</span><span class="sxs-lookup"><span data-stu-id="ea6f1-118">displayName</span></span>|<span data-ttu-id="ea6f1-119">Строка</span><span class="sxs-lookup"><span data-stu-id="ea6f1-119">String</span></span>|<span data-ttu-id="ea6f1-120">Отображаемое имя разрешения, которое отображается в качестве согласия администратора и взаимодействия с назначением приложений.</span><span class="sxs-lookup"><span data-stu-id="ea6f1-120">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="ea6f1-121">id</span><span class="sxs-lookup"><span data-stu-id="ea6f1-121">id</span></span>|<span data-ttu-id="ea6f1-122">GUID</span><span class="sxs-lookup"><span data-stu-id="ea6f1-122">Guid</span></span>|<span data-ttu-id="ea6f1-123">Уникальный идентификатор роли в семействе **appRoles** .</span><span class="sxs-lookup"><span data-stu-id="ea6f1-123">Unique role identifier inside the **appRoles** collection.</span></span> <span data-ttu-id="ea6f1-124">При создании новой роли приложения необходимо указать новый идентификатор GUID.</span><span class="sxs-lookup"><span data-stu-id="ea6f1-124">When creating a new app role, a new Guid identifier must be provided.</span></span> |
|<span data-ttu-id="ea6f1-125">isEnabled</span><span class="sxs-lookup"><span data-stu-id="ea6f1-125">isEnabled</span></span>|<span data-ttu-id="ea6f1-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea6f1-126">Boolean</span></span>|<span data-ttu-id="ea6f1-127">При создании или обновлении роли приложения должно быть задано **значение true** (значение по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="ea6f1-127">When creating or updating an app role, this must be set to **true** (which is the default).</span></span> <span data-ttu-id="ea6f1-128">Чтобы удалить роль, необходимо сначала задать значение **false**.</span><span class="sxs-lookup"><span data-stu-id="ea6f1-128">To delete a role, this must first be set to **false**.</span></span>  <span data-ttu-id="ea6f1-129">В этот момент эта роль может быть удалена в последующих вызовах.</span><span class="sxs-lookup"><span data-stu-id="ea6f1-129">At that point, in a subsequent call, this role may be removed.</span></span>|
|<span data-ttu-id="ea6f1-130">основания</span><span class="sxs-lookup"><span data-stu-id="ea6f1-130">origin</span></span>|<span data-ttu-id="ea6f1-131">String</span><span class="sxs-lookup"><span data-stu-id="ea6f1-131">String</span></span>| <span data-ttu-id="ea6f1-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ea6f1-132">Read-only.</span></span> <span data-ttu-id="ea6f1-133">Указывает, определена ли роль приложения для объекта Application.</span><span class="sxs-lookup"><span data-stu-id="ea6f1-133">Specifies if the app role is defined on the Application object</span></span> <!-- or on the ServicePrincipal object --><span data-ttu-id="ea6f1-134">.</span><span class="sxs-lookup"><span data-stu-id="ea6f1-134">.</span></span> <span data-ttu-id="ea6f1-135">_Не_ следует включать в запросы POST или patch.</span><span class="sxs-lookup"><span data-stu-id="ea6f1-135">Must _not_ be included in any POST or PATCH requests.</span></span> |
|<span data-ttu-id="ea6f1-136">value</span><span class="sxs-lookup"><span data-stu-id="ea6f1-136">value</span></span>|<span data-ttu-id="ea6f1-137">String</span><span class="sxs-lookup"><span data-stu-id="ea6f1-137">String</span></span>|<span data-ttu-id="ea6f1-138">Указывает значение, которое будет включено в `roles` заявку для проверки подлинности и маркеров доступа.</span><span class="sxs-lookup"><span data-stu-id="ea6f1-138">Specifies the value which will be included in the `roles` claim in authentication and access tokens.</span></span> <span data-ttu-id="ea6f1-139">Длина не должна превышать 120 символов.</span><span class="sxs-lookup"><span data-stu-id="ea6f1-139">Must not exceed 120 characters in length.</span></span> <span data-ttu-id="ea6f1-140">`:` `!` `#` `$` Допустимые знаки `%` `0-9` `A-Z` `a-z`, а также символы в диапазонах и. `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~`</span><span class="sxs-lookup"><span data-stu-id="ea6f1-140">Allowed characters are `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~`, as well as characters in the ranges `0-9`, `A-Z` and `a-z`.</span></span> <span data-ttu-id="ea6f1-141">Любой другой символ, в том числе символ пробела, не допускается.</span><span class="sxs-lookup"><span data-stu-id="ea6f1-141">Any other character, including the space character, are not allowed.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="ea6f1-142">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ea6f1-142">JSON representation</span></span>

<span data-ttu-id="ea6f1-143">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ea6f1-143">Here is a JSON representation of the resource</span></span>

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
