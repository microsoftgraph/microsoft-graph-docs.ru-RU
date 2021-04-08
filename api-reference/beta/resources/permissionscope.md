---
title: Тип ресурса permissionScope
description: Представляет определение делегирования разрешения, иногда именуемого разрешением OAuth 2.0 или областью OAuth 2.0. После определения делегированная разрешения может запрашиваться клиентской заявкой.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 0d5d09599108b7753ee60012337e393c6bc79905
ms.sourcegitcommit: aa18eb8a9965f99cc97680808abba8df46f31ba5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2021
ms.locfileid: "51638860"
---
# <a name="permissionscope-resource-type"></a><span data-ttu-id="863be-104">Тип ресурса permissionScope</span><span class="sxs-lookup"><span data-stu-id="863be-104">permissionScope resource type</span></span>

<span data-ttu-id="863be-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="863be-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="863be-106">Представляет определение [делегирования разрешения.](/azure/active-directory/develop/v2-permissions-and-consent#permission-types)</span><span class="sxs-lookup"><span data-stu-id="863be-106">Represents the definition of a [delegated permission](/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span></span>

<span data-ttu-id="863be-107">Делегировать разрешения могут клиентские приложения, которым требуется маркер доступа к API, определяющий разрешения.</span><span class="sxs-lookup"><span data-stu-id="863be-107">Delegated permissions can be requested by client applications needing an access token to the API which defined the permissions.</span></span> <span data-ttu-id="863be-108">Делегирование разрешений можно [](/azure/active-directory/develop/v2-permissions-and-consent#requesting-individual-user-consent)запрашивать динамически, используя параметр в запросе на авторизацию платформы удостоверений Майкрософт, или статически, через коллекцию `scopes` **requiredResourceAccess на** объекте приложения. [](/azure/active-directory/develop/v2-permissions-and-consent#the-default-scope) [](application.md)</span><span class="sxs-lookup"><span data-stu-id="863be-108">Delegated permissions can be requested [dynamically](/azure/active-directory/develop/v2-permissions-and-consent#requesting-individual-user-consent), using the `scopes` parameter in an authorization request to the Microsoft identity platform, or [statically](/azure/active-directory/develop/v2-permissions-and-consent#the-default-scope), through the **requiredResourceAccess** collection on the [application](application.md) object.</span></span>

## <a name="properties"></a><span data-ttu-id="863be-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="863be-109">Properties</span></span>

| <span data-ttu-id="863be-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="863be-110">Property</span></span> | <span data-ttu-id="863be-111">Тип</span><span class="sxs-lookup"><span data-stu-id="863be-111">Type</span></span> | <span data-ttu-id="863be-112">Описание</span><span class="sxs-lookup"><span data-stu-id="863be-112">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="863be-113">adminConsentDescription</span><span class="sxs-lookup"><span data-stu-id="863be-113">adminConsentDescription</span></span>|<span data-ttu-id="863be-114">String</span><span class="sxs-lookup"><span data-stu-id="863be-114">String</span></span>|<span data-ttu-id="863be-115">Описание делегирования разрешений, которые должен прочитать администратор, дающий разрешение от имени всех пользователей.</span><span class="sxs-lookup"><span data-stu-id="863be-115">A description of the delegated permissions, intended to be read by an administrator granting the permission on behalf of all users.</span></span> <span data-ttu-id="863be-116">Этот текст отображается в интерфейсе согласия администратора для всего клиента.</span><span class="sxs-lookup"><span data-stu-id="863be-116">This text appears in tenant-wide admin consent experiences.</span></span>|
|<span data-ttu-id="863be-117">adminConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="863be-117">adminConsentDisplayName</span></span>|<span data-ttu-id="863be-118">String</span><span class="sxs-lookup"><span data-stu-id="863be-118">String</span></span>|<span data-ttu-id="863be-119">Название разрешения, предназначенное для чтения администратором, дающим разрешение от имени всех пользователей.</span><span class="sxs-lookup"><span data-stu-id="863be-119">The permission's title, intended to be read by an administrator granting the permission on behalf of all users.</span></span>|
|<span data-ttu-id="863be-120">id</span><span class="sxs-lookup"><span data-stu-id="863be-120">id</span></span>|<span data-ttu-id="863be-121">GUID</span><span class="sxs-lookup"><span data-stu-id="863be-121">Guid</span></span>|<span data-ttu-id="863be-122">Уникальный идентификатор делегирования разрешений внутри коллекции делегированных разрешений, определенных для приложения-ресурса.</span><span class="sxs-lookup"><span data-stu-id="863be-122">Unique delegated permission identifier inside the collection of delegated permissions defined for a resource application.</span></span>|
|<span data-ttu-id="863be-123">isEnabled</span><span class="sxs-lookup"><span data-stu-id="863be-123">isEnabled</span></span>|<span data-ttu-id="863be-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="863be-124">Boolean</span></span>|<span data-ttu-id="863be-125">При создании или обновлении разрешения это свойство должно быть заданной значение **true** (по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="863be-125">When creating or updating a permission, this property must be set to **true** (which is the default).</span></span> <span data-ttu-id="863be-126">Чтобы удалить разрешение, это свойство сначала должно быть настроено **как** false .</span><span class="sxs-lookup"><span data-stu-id="863be-126">To delete a permission, this property must first be set to **false**.</span></span>  <span data-ttu-id="863be-127">В этот момент при последующем вызове разрешение может быть удалено.</span><span class="sxs-lookup"><span data-stu-id="863be-127">At that point, in a subsequent call, the permission may be removed.</span></span>|
|<span data-ttu-id="863be-128">type</span><span class="sxs-lookup"><span data-stu-id="863be-128">type</span></span>|<span data-ttu-id="863be-129">String</span><span class="sxs-lookup"><span data-stu-id="863be-129">String</span></span>|<span data-ttu-id="863be-130">Указывает, следует ли считать это делегированное разрешение безопасным для неадминистрирования пользователей, чтобы дать согласие от имени самих себя, или необходимо ли администратору для согласия на разрешения.</span><span class="sxs-lookup"><span data-stu-id="863be-130">Specifies whether this delegated permission should be considered safe for non-admin users to consent to on behalf of themselves, or whether an administrator should be required for consent to the permissions.</span></span> <span data-ttu-id="863be-131">Это будет поведение по умолчанию, но каждый клиент может настроить поведение в своей организации (разрешив, ограничив или ограничив согласие пользователя этим делегированным разрешением.)</span><span class="sxs-lookup"><span data-stu-id="863be-131">This will be the default behavior, but each customer can choose to customize the behavior in their organization (by allowing, restricting or limiting user consent to this delegated permission.)</span></span>|
|<span data-ttu-id="863be-132">userConsentDescription</span><span class="sxs-lookup"><span data-stu-id="863be-132">userConsentDescription</span></span>|<span data-ttu-id="863be-133">String</span><span class="sxs-lookup"><span data-stu-id="863be-133">String</span></span>|<span data-ttu-id="863be-134">Описание делегирования разрешений, предназначенных для чтения пользователем, выдающим разрешение от своего имени.</span><span class="sxs-lookup"><span data-stu-id="863be-134">A description of the delegated permissions, intended to be read by a user granting the permission on their own behalf.</span></span> <span data-ttu-id="863be-135">Этот текст отображается в случаях согласия, когда пользователь соглашается только от имени себя.</span><span class="sxs-lookup"><span data-stu-id="863be-135">This text appears in consent experiences where the user is consenting only on behalf of themselves.</span></span>|
|<span data-ttu-id="863be-136">userConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="863be-136">userConsentDisplayName</span></span>|<span data-ttu-id="863be-137">String</span><span class="sxs-lookup"><span data-stu-id="863be-137">String</span></span>|<span data-ttu-id="863be-138">Название разрешения, предназначенное для чтения пользователем, выдающим разрешение от своего имени.</span><span class="sxs-lookup"><span data-stu-id="863be-138">A title for the permission, intended to be read by a user granting the permission on their own behalf.</span></span> <span data-ttu-id="863be-139">Этот текст отображается в случаях согласия, когда пользователь соглашается только от имени себя.</span><span class="sxs-lookup"><span data-stu-id="863be-139">This text appears in consent experiences where the user is consenting only on behalf of themselves.</span></span>|
|<span data-ttu-id="863be-140">value</span><span class="sxs-lookup"><span data-stu-id="863be-140">value</span></span>|<span data-ttu-id="863be-141">String</span><span class="sxs-lookup"><span data-stu-id="863be-141">String</span></span>|<span data-ttu-id="863be-142">Указывает значение, необходимое для включаемого `scp` в (область) утверждения в маркерах доступа.</span><span class="sxs-lookup"><span data-stu-id="863be-142">Specifies the value to include in the `scp` (scope) claim in access tokens.</span></span> <span data-ttu-id="863be-143">Длина не должна превышать 120 символов.</span><span class="sxs-lookup"><span data-stu-id="863be-143">Must not exceed 120 characters in length.</span></span> <span data-ttu-id="863be-144">Разрешены `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~` символы, а также символы в диапазонах `0-9` и `A-Z` `a-z` .</span><span class="sxs-lookup"><span data-stu-id="863be-144">Allowed characters are `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~`, as well as characters in the ranges `0-9`, `A-Z` and `a-z`.</span></span> <span data-ttu-id="863be-145">Любой другой символ, включая символ пространства, не допускается.</span><span class="sxs-lookup"><span data-stu-id="863be-145">Any other character, including the space character, are not allowed.</span></span> <span data-ttu-id="863be-146">Может не `.` начинаться с .</span><span class="sxs-lookup"><span data-stu-id="863be-146">May not begin with `.`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="863be-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="863be-147">JSON representation</span></span>

<span data-ttu-id="863be-148">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="863be-148">Here is a JSON representation of the resource</span></span>

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
