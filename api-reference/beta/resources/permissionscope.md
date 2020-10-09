---
title: Тип ресурса permissionScope
description: Представляет определение делегированного разрешения, которое иногда называют разрешением OAuth 2,0 или областью OAuth 2,0. После определения делегированное разрешение может быть запрошено клиентским приложением.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: ea3205139bffa11ff8fbe67d1ab6abb426bc65ca
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48406179"
---
# <a name="permissionscope-resource-type"></a><span data-ttu-id="47143-104">Тип ресурса permissionScope</span><span class="sxs-lookup"><span data-stu-id="47143-104">permissionScope resource type</span></span>

<span data-ttu-id="47143-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47143-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47143-106">Представляет определение [делегированного разрешения](/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span><span class="sxs-lookup"><span data-stu-id="47143-106">Represents the definition of a [delegated permission](/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span></span>

<span data-ttu-id="47143-107">Делегированные разрешения могут запрашиваться клиентскими приложениями, которым необходим маркер доступа к API, в котором определены разрешения.</span><span class="sxs-lookup"><span data-stu-id="47143-107">Delegated permissions can be requested by client applications needing an access token to the API which defined the permissions.</span></span> <span data-ttu-id="47143-108">Делегированные разрешения можно запрашивать [динамически](/azure/active-directory/develop/v2-permissions-and-consent#requesting-individual-user-consent), используя `scopes` параметр в запросе на авторизацию для платформы идентификации Майкрософт или [статически](/azure/active-directory/develop/v2-permissions-and-consent#the-default-scope), с помощью коллекции **рекуиредресаурцеакцесс** для объекта [Application](application.md) .</span><span class="sxs-lookup"><span data-stu-id="47143-108">Delegated permissions can be requested [dynamically](/azure/active-directory/develop/v2-permissions-and-consent#requesting-individual-user-consent), using the `scopes` parameter in an authorization request to the Microsoft identity platform, or [statically](/azure/active-directory/develop/v2-permissions-and-consent#the-default-scope), through the **requiredResourceAccess** collection on the [application](application.md) object.</span></span>

## <a name="properties"></a><span data-ttu-id="47143-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="47143-109">Properties</span></span>

| <span data-ttu-id="47143-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="47143-110">Property</span></span> | <span data-ttu-id="47143-111">Тип</span><span class="sxs-lookup"><span data-stu-id="47143-111">Type</span></span> | <span data-ttu-id="47143-112">Описание</span><span class="sxs-lookup"><span data-stu-id="47143-112">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="47143-113">админконсентдескриптион</span><span class="sxs-lookup"><span data-stu-id="47143-113">adminConsentDescription</span></span>|<span data-ttu-id="47143-114">String</span><span class="sxs-lookup"><span data-stu-id="47143-114">String</span></span>|<span data-ttu-id="47143-115">Описание делегированных разрешений, которое должно быть прочитано администратором, предоставляя разрешение от имени всех пользователей.</span><span class="sxs-lookup"><span data-stu-id="47143-115">A description of the delegated permissions, intended to be read by an administrator granting the permission on behalf of all users.</span></span> <span data-ttu-id="47143-116">Этот текст отображается в диалоговом окне согласия администратора на уровне клиента.</span><span class="sxs-lookup"><span data-stu-id="47143-116">This text appears in tenant-wide admin consent experiences.</span></span>|
|<span data-ttu-id="47143-117">админконсентдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="47143-117">adminConsentDisplayName</span></span>|<span data-ttu-id="47143-118">String</span><span class="sxs-lookup"><span data-stu-id="47143-118">String</span></span>|<span data-ttu-id="47143-119">Заголовок разрешения, предназначенный для чтения администратором, предоставляя разрешение от имени всех пользователей.</span><span class="sxs-lookup"><span data-stu-id="47143-119">The permission's title, intended to be read by an administrator granting the permission on behalf of all users.</span></span>|
|<span data-ttu-id="47143-120">id</span><span class="sxs-lookup"><span data-stu-id="47143-120">id</span></span>|<span data-ttu-id="47143-121">GUID</span><span class="sxs-lookup"><span data-stu-id="47143-121">Guid</span></span>|<span data-ttu-id="47143-122">Уникальный идентификатор делегированного разрешения в коллекции делегированных разрешений, определенных для приложения ресурсов.</span><span class="sxs-lookup"><span data-stu-id="47143-122">Unique delegated permission identifier inside the collection of delegated permissions defined for a resource application.</span></span>|
|<span data-ttu-id="47143-123">isEnabled</span><span class="sxs-lookup"><span data-stu-id="47143-123">isEnabled</span></span>|<span data-ttu-id="47143-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="47143-124">Boolean</span></span>|<span data-ttu-id="47143-125">При создании или обновлении разрешения для этого свойства должно быть задано **значение true** (значение по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="47143-125">When creating or updating a permission, this property must be set to **true** (which is the default).</span></span> <span data-ttu-id="47143-126">Чтобы удалить разрешение, необходимо сначала задать для этого свойства значение **false**.</span><span class="sxs-lookup"><span data-stu-id="47143-126">To delete a permission, this property must first be set to **false**.</span></span>  <span data-ttu-id="47143-127">В этот момент разрешение может быть удалено из последующего вызова.</span><span class="sxs-lookup"><span data-stu-id="47143-127">At that point, in a subsequent call, the permission may be removed.</span></span>|
|<span data-ttu-id="47143-128">type</span><span class="sxs-lookup"><span data-stu-id="47143-128">type</span></span>|<span data-ttu-id="47143-129">String</span><span class="sxs-lookup"><span data-stu-id="47143-129">String</span></span>|<span data-ttu-id="47143-130">Указывает, следует ли считать это делегированное разрешение небезопасным для пользователей, не являющихся администраторами, согласия от собственного имени, а также от того, требуется ли администратору разрешение на предоставление разрешений.</span><span class="sxs-lookup"><span data-stu-id="47143-130">Specifies whether this delegated permission should be considered safe for non-admin users to consent to on behalf of themselves, or whether an administrator should be required for consent to the permissions.</span></span> <span data-ttu-id="47143-131">Это будет поведением по умолчанию, но каждый пользователь может выбрать настройку поведения в Организации (путем разрешения, ограничения или ограничения согласия пользователя на делегированное разрешение).</span><span class="sxs-lookup"><span data-stu-id="47143-131">This will be the default behavior, but each customer can choose to customize the behavior in their organization (by allowing, restricting or limiting user consent to this delegated permission.)</span></span>|
|<span data-ttu-id="47143-132">усерконсентдескриптион</span><span class="sxs-lookup"><span data-stu-id="47143-132">userConsentDescription</span></span>|<span data-ttu-id="47143-133">String</span><span class="sxs-lookup"><span data-stu-id="47143-133">String</span></span>|<span data-ttu-id="47143-134">Описание делегированных разрешений, предназначенное для чтения пользователем, предоставляя разрешение от их имени.</span><span class="sxs-lookup"><span data-stu-id="47143-134">A description of the delegated permissions, intended to be read by a user granting the permission on their own behalf.</span></span> <span data-ttu-id="47143-135">Этот текст отображается в диалоговом окне разрешения, когда пользователь отправляется только от чужого имени.</span><span class="sxs-lookup"><span data-stu-id="47143-135">This text appears in consent experiences where the user is consenting only on behalf of themselves.</span></span>|
|<span data-ttu-id="47143-136">усерконсентдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="47143-136">userConsentDisplayName</span></span>|<span data-ttu-id="47143-137">String</span><span class="sxs-lookup"><span data-stu-id="47143-137">String</span></span>|<span data-ttu-id="47143-138">Название разрешения, которое должно быть прочитано пользователем, предоставляя разрешение от его имени.</span><span class="sxs-lookup"><span data-stu-id="47143-138">A title for the permission, intended to be read by a user granting the permission on their own behalf.</span></span> <span data-ttu-id="47143-139">Этот текст отображается в диалоговом окне разрешения, когда пользователь отправляется только от чужого имени.</span><span class="sxs-lookup"><span data-stu-id="47143-139">This text appears in consent experiences where the user is consenting only on behalf of themselves.</span></span>|
|<span data-ttu-id="47143-140">value</span><span class="sxs-lookup"><span data-stu-id="47143-140">value</span></span>|<span data-ttu-id="47143-141">String</span><span class="sxs-lookup"><span data-stu-id="47143-141">String</span></span>|<span data-ttu-id="47143-142">Указывает значение, которое необходимо включить в `scp` утверждение (область) в маркерах доступа.</span><span class="sxs-lookup"><span data-stu-id="47143-142">Specifies the value to include in the `scp` (scope) claim in access tokens.</span></span> <span data-ttu-id="47143-143">Длина не должна превышать 120 символов.</span><span class="sxs-lookup"><span data-stu-id="47143-143">Must not exceed 120 characters in length.</span></span> <span data-ttu-id="47143-144">Допустимые знаки `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~` , а также символы в диапазонах `0-9` `A-Z` и `a-z` .</span><span class="sxs-lookup"><span data-stu-id="47143-144">Allowed characters are `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~`, as well as characters in the ranges `0-9`, `A-Z` and `a-z`.</span></span> <span data-ttu-id="47143-145">Любой другой символ, в том числе символ пробела, не допускается.</span><span class="sxs-lookup"><span data-stu-id="47143-145">Any other character, including the space character, are not allowed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="47143-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="47143-146">JSON representation</span></span>

<span data-ttu-id="47143-147">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="47143-147">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.permissionScope"
}-->

```json
{
  "id": "guid",
  "adminConsentDisplayName": "string",
  "adminConsentDescription": "string",
  "userConsentDisplayName": "string",
  "userConsentDescription": "string",
  "value": "string",
  "type": "string",
  "isEnabled": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oAuth2Permission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->