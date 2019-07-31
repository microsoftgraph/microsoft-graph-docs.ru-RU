---
title: Тип ресурса Аппроле
description: Представляет роль приложения, которая может быть запрошена клиентским приложением, вызывающей другое приложение, или которая может использоваться для назначения приложения пользователям или группам в указанной роли приложения. Свойство **appRoles** объекта servicePrincipal и сущности приложения является коллекцией **аппроле**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 35c26e52c5d7eb9529474d08a43b68fceddfc954
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013329"
---
# <a name="approle-resource-type"></a><span data-ttu-id="199de-104">Тип ресурса Аппроле</span><span class="sxs-lookup"><span data-stu-id="199de-104">appRole resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="199de-105">Представляет роль приложения, которая может быть запрошена клиентским приложением, вызывающей другое приложение, или которая может использоваться для назначения приложения пользователям или группам в указанной роли приложения.</span><span class="sxs-lookup"><span data-stu-id="199de-105">Represents an application role that may be requested by a client application calling another application or that may be used to assign an application to users or groups in a specified application role.</span></span> <span data-ttu-id="199de-106">Свойство **appRoles** объекта [servicePrincipal](serviceprincipal.md) и сущности [приложения](application.md) является коллекцией **аппроле**.</span><span class="sxs-lookup"><span data-stu-id="199de-106">The **appRoles** property of the [servicePrincipal](serviceprincipal.md) entity and of the [application](application.md) entity is a collection of **appRole**.</span></span>

> <span data-ttu-id="199de-107">Важно! эта функция отключена в текущем выпуске.</span><span class="sxs-lookup"><span data-stu-id="199de-107">Important: This functionality is disabled in the current release.</span></span>

## <a name="json-representation"></a><span data-ttu-id="199de-108">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="199de-108">JSON representation</span></span>

<span data-ttu-id="199de-109">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="199de-109">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="199de-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="199de-110">Properties</span></span>
| <span data-ttu-id="199de-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="199de-111">Property</span></span>     | <span data-ttu-id="199de-112">Тип</span><span class="sxs-lookup"><span data-stu-id="199de-112">Type</span></span>   |<span data-ttu-id="199de-113">Описание</span><span class="sxs-lookup"><span data-stu-id="199de-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="199de-114">Алловедмембертипес</span><span class="sxs-lookup"><span data-stu-id="199de-114">allowedMemberTypes</span></span>|<span data-ttu-id="199de-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="199de-115">String collection</span></span>|<span data-ttu-id="199de-116">Указывает, можно ли назначить это определение роли приложения пользователям и группам, задав для параметра значение "пользователь" или другие приложения (которые обращаются к этому приложению в сценариях службы демона), задав значение "Application" или как то, и другое.</span><span class="sxs-lookup"><span data-stu-id="199de-116">Specifies whether this app role definition can be assigned to users and groups by setting to "User", or to other applications (that are accessing this application in daemon service scenarios) by setting to "Application", or to both.</span></span>|
|<span data-ttu-id="199de-117">description</span><span class="sxs-lookup"><span data-stu-id="199de-117">description</span></span>|<span data-ttu-id="199de-118">String</span><span class="sxs-lookup"><span data-stu-id="199de-118">String</span></span>|<span data-ttu-id="199de-119">Текст справки по разрешениям, который отображается при назначении и согласии приложения администрирования.</span><span class="sxs-lookup"><span data-stu-id="199de-119">Permission help text that appears in the admin app assignment and consent experiences.</span></span>|
|<span data-ttu-id="199de-120">displayName</span><span class="sxs-lookup"><span data-stu-id="199de-120">displayName</span></span>|<span data-ttu-id="199de-121">Строка</span><span class="sxs-lookup"><span data-stu-id="199de-121">String</span></span>|<span data-ttu-id="199de-122">Отображаемое имя разрешения, которое отображается в качестве согласия администратора и взаимодействия с назначением приложений.</span><span class="sxs-lookup"><span data-stu-id="199de-122">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="199de-123">id</span><span class="sxs-lookup"><span data-stu-id="199de-123">id</span></span>|<span data-ttu-id="199de-124">GUID</span><span class="sxs-lookup"><span data-stu-id="199de-124">Guid</span></span>|<span data-ttu-id="199de-125">Уникальный идентификатор роли в семействе **appRoles** .</span><span class="sxs-lookup"><span data-stu-id="199de-125">Unique role identifier inside the **appRoles** collection.</span></span> <span data-ttu-id="199de-126">При создании новой роли приложения необходимо указать новый идентификатор GUID.</span><span class="sxs-lookup"><span data-stu-id="199de-126">When creating a new app role, a new Guid identifier must be provided.</span></span> |
|<span data-ttu-id="199de-127">isEnabled</span><span class="sxs-lookup"><span data-stu-id="199de-127">isEnabled</span></span>|<span data-ttu-id="199de-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="199de-128">Boolean</span></span>|<span data-ttu-id="199de-129">При создании или обновлении роли приложения должно быть задано **значение true** (значение по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="199de-129">When creating or updating an app role, this must be set to **true** (which is the default).</span></span> <span data-ttu-id="199de-130">Чтобы удалить роль, необходимо сначала задать значение **false**.</span><span class="sxs-lookup"><span data-stu-id="199de-130">To delete a role, this must first be set to **false**.</span></span>  <span data-ttu-id="199de-131">В этот момент эта роль может быть удалена в последующих вызовах.</span><span class="sxs-lookup"><span data-stu-id="199de-131">At that point, in a subsequent call, this role may be removed.</span></span>|
|<span data-ttu-id="199de-132">основания</span><span class="sxs-lookup"><span data-stu-id="199de-132">origin</span></span>|<span data-ttu-id="199de-133">String</span><span class="sxs-lookup"><span data-stu-id="199de-133">String</span></span>| <span data-ttu-id="199de-134">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="199de-134">Read-only.</span></span> <span data-ttu-id="199de-135">Указывает, определена ли роль приложения для объекта Application или объекта ServicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="199de-135">Specifies if the app role is defined on the Application object or on the ServicePrincipal object.</span></span> <span data-ttu-id="199de-136">_Не_ следует включать в запросы POST или patch.</span><span class="sxs-lookup"><span data-stu-id="199de-136">Must _not_ be included in any POST or PATCH requests.</span></span> |
|<span data-ttu-id="199de-137">value</span><span class="sxs-lookup"><span data-stu-id="199de-137">value</span></span>|<span data-ttu-id="199de-138">String</span><span class="sxs-lookup"><span data-stu-id="199de-138">String</span></span>|<span data-ttu-id="199de-139">Указывает значение, которое будет включено в `roles` заявку для проверки подлинности и маркеров доступа.</span><span class="sxs-lookup"><span data-stu-id="199de-139">Specifies the value which will be included in the `roles` claim in authentication and access tokens.</span></span> <span data-ttu-id="199de-140">Длина не должна превышать 120 символов.</span><span class="sxs-lookup"><span data-stu-id="199de-140">Must not exceed 120 characters in length.</span></span> <span data-ttu-id="199de-141">Допустимые `:` `!` `#` `$` символы `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `A-Z` также символы в диапазонах `a-z`и. `0-9` `^` `@` `[` `]` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~`</span><span class="sxs-lookup"><span data-stu-id="199de-141">Allowed characters are `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~`, as well as characters in the ranges `0-9`, `A-Z` and `a-z`.</span></span> <span data-ttu-id="199de-142">Любой другой символ, в том числе символ пробела, не допускается.</span><span class="sxs-lookup"><span data-stu-id="199de-142">Any other character, including the space character, are not allowed.</span></span>  |


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
