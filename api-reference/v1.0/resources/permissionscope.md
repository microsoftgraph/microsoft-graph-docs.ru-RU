---
title: Тип ресурса permissionScope
description: Представляет определение делегированного разрешения, иногда именуемого разрешением OAuth 2.0 или областью OAuth 2.0. После определения делегирование разрешения может быть запророшо клиентской приложением.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 661b94ce8f349d65d44ed1ad1c7e235feb8ad7ff
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135746"
---
# <a name="permissionscope-resource-type"></a><span data-ttu-id="fc720-104">Тип ресурса permissionScope</span><span class="sxs-lookup"><span data-stu-id="fc720-104">permissionScope resource type</span></span>

<span data-ttu-id="fc720-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc720-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fc720-106">Представляет определение [делегированного разрешения.](/azure/active-directory/develop/v2-permissions-and-consent#permission-types)</span><span class="sxs-lookup"><span data-stu-id="fc720-106">Represents the definition of a [delegated permission](/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span></span>

<span data-ttu-id="fc720-107">Клиентские приложения, которым требуется маркер доступа к API, определяющий разрешения, могут запрашивать делегирование разрешений.</span><span class="sxs-lookup"><span data-stu-id="fc720-107">Delegated permissions can be requested by client applications needing an access token to the API which defined the permissions.</span></span> <span data-ttu-id="fc720-108">Делегировать разрешения можно динамически [с](/azure/active-directory/develop/v2-permissions-and-consent#requesting-individual-user-consent)помощью параметра в запросе на авторизацию платформы удостоверений Майкрософт или статически с помощью коллекции `scopes` **requiredResourceAccess** объекта приложения. [](/azure/active-directory/develop/v2-permissions-and-consent#the-default-scope) [](application.md)</span><span class="sxs-lookup"><span data-stu-id="fc720-108">Delegated permissions can be requested [dynamically](/azure/active-directory/develop/v2-permissions-and-consent#requesting-individual-user-consent), using the `scopes` parameter in an authorization request to the Microsoft identity platform, or [statically](/azure/active-directory/develop/v2-permissions-and-consent#the-default-scope), through the **requiredResourceAccess** collection on the [application](application.md) object.</span></span>

## <a name="properties"></a><span data-ttu-id="fc720-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="fc720-109">Properties</span></span>

| <span data-ttu-id="fc720-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="fc720-110">Property</span></span> | <span data-ttu-id="fc720-111">Тип</span><span class="sxs-lookup"><span data-stu-id="fc720-111">Type</span></span> | <span data-ttu-id="fc720-112">Описание</span><span class="sxs-lookup"><span data-stu-id="fc720-112">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="fc720-113">adminConsentDescription</span><span class="sxs-lookup"><span data-stu-id="fc720-113">adminConsentDescription</span></span>|<span data-ttu-id="fc720-114">String</span><span class="sxs-lookup"><span data-stu-id="fc720-114">String</span></span>|<span data-ttu-id="fc720-115">Описание делегирования разрешений, предназначенных для чтения администратором, который предоставляет разрешение от имени всех пользователей.</span><span class="sxs-lookup"><span data-stu-id="fc720-115">A description of the delegated permissions, intended to be read by an administrator granting the permission on behalf of all users.</span></span> <span data-ttu-id="fc720-116">Этот текст отображается в интерфейсах согласия администратора на весь клиент.</span><span class="sxs-lookup"><span data-stu-id="fc720-116">This text appears in tenant-wide admin consent experiences.</span></span>|
|<span data-ttu-id="fc720-117">adminConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="fc720-117">adminConsentDisplayName</span></span>|<span data-ttu-id="fc720-118">String</span><span class="sxs-lookup"><span data-stu-id="fc720-118">String</span></span>|<span data-ttu-id="fc720-119">Название разрешения, предназначенное для чтения администратором, который предоставил разрешение от имени всех пользователей.</span><span class="sxs-lookup"><span data-stu-id="fc720-119">The permission's title, intended to be read by an administrator granting the permission on behalf of all users.</span></span>|
|<span data-ttu-id="fc720-120">id</span><span class="sxs-lookup"><span data-stu-id="fc720-120">id</span></span>|<span data-ttu-id="fc720-121">GUID</span><span class="sxs-lookup"><span data-stu-id="fc720-121">Guid</span></span>|<span data-ttu-id="fc720-122">Уникальный идентификатор делегирования разрешений внутри коллекции делегных разрешений, определенных для приложения ресурса.</span><span class="sxs-lookup"><span data-stu-id="fc720-122">Unique delegated permission identifier inside the collection of delegated permissions defined for a resource application.</span></span>|
|<span data-ttu-id="fc720-123">isEnabled</span><span class="sxs-lookup"><span data-stu-id="fc720-123">isEnabled</span></span>|<span data-ttu-id="fc720-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc720-124">Boolean</span></span>|<span data-ttu-id="fc720-125">При создании или обновлении разрешения для этого свойства должно быть установлено значение **true** (что является значением по умолчанию).</span><span class="sxs-lookup"><span data-stu-id="fc720-125">When creating or updating a permission, this property must be set to **true** (which is the default).</span></span> <span data-ttu-id="fc720-126">Чтобы удалить разрешение, для этого свойства сначала необходимо установить **false.**</span><span class="sxs-lookup"><span data-stu-id="fc720-126">To delete a permission, this property must first be set to **false**.</span></span>  <span data-ttu-id="fc720-127">На этом этапе в последующем вызове разрешение может быть удалено.</span><span class="sxs-lookup"><span data-stu-id="fc720-127">At that point, in a subsequent call, the permission may be removed.</span></span>|
|<span data-ttu-id="fc720-128">type</span><span class="sxs-lookup"><span data-stu-id="fc720-128">type</span></span>|<span data-ttu-id="fc720-129">String</span><span class="sxs-lookup"><span data-stu-id="fc720-129">String</span></span>|<span data-ttu-id="fc720-130">Указывает, следует ли считать это делегированное разрешение безопасным для пользователей, не управляющего, на согласие от имени себя или необходимо ли администратору для получения согласия на разрешения.</span><span class="sxs-lookup"><span data-stu-id="fc720-130">Specifies whether this delegated permission should be considered safe for non-admin users to consent to on behalf of themselves, or whether an administrator should be required for consent to the permissions.</span></span> <span data-ttu-id="fc720-131">Это будет поведение по умолчанию, но каждый клиент может настроить поведение в своей организации (разрешив, ограничив или ограничив согласие пользователя этим делегированным разрешением.)</span><span class="sxs-lookup"><span data-stu-id="fc720-131">This will be the default behavior, but each customer can choose to customize the behavior in their organization (by allowing, restricting or limiting user consent to this delegated permission.)</span></span>|
|<span data-ttu-id="fc720-132">userConsentDescription</span><span class="sxs-lookup"><span data-stu-id="fc720-132">userConsentDescription</span></span>|<span data-ttu-id="fc720-133">String</span><span class="sxs-lookup"><span data-stu-id="fc720-133">String</span></span>|<span data-ttu-id="fc720-134">Описание делегирования разрешений, предназначенных для чтения пользователем, который предоставляет разрешение от своего имени.</span><span class="sxs-lookup"><span data-stu-id="fc720-134">A description of the delegated permissions, intended to be read by a user granting the permission on their own behalf.</span></span> <span data-ttu-id="fc720-135">Этот текст отображается в интерфейсах согласия, когда пользователь дает согласие только от имени себя.</span><span class="sxs-lookup"><span data-stu-id="fc720-135">This text appears in consent experiences where the user is consenting only on behalf of themselves.</span></span>|
|<span data-ttu-id="fc720-136">userConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="fc720-136">userConsentDisplayName</span></span>|<span data-ttu-id="fc720-137">String</span><span class="sxs-lookup"><span data-stu-id="fc720-137">String</span></span>|<span data-ttu-id="fc720-138">Заголовок разрешения, предназначенный для чтения пользователем, который предоставил разрешение от своего имени.</span><span class="sxs-lookup"><span data-stu-id="fc720-138">A title for the permission, intended to be read by a user granting the permission on their own behalf.</span></span> <span data-ttu-id="fc720-139">Этот текст отображается в интерфейсах согласия, когда пользователь дает согласие только от имени себя.</span><span class="sxs-lookup"><span data-stu-id="fc720-139">This text appears in consent experiences where the user is consenting only on behalf of themselves.</span></span>|
|<span data-ttu-id="fc720-140">value</span><span class="sxs-lookup"><span data-stu-id="fc720-140">value</span></span>|<span data-ttu-id="fc720-141">String</span><span class="sxs-lookup"><span data-stu-id="fc720-141">String</span></span>|<span data-ttu-id="fc720-142">Указывает значение, включаемого в `scp` утверждение (область) в маркеры доступа.</span><span class="sxs-lookup"><span data-stu-id="fc720-142">Specifies the value to include in the `scp` (scope) claim in access tokens.</span></span> <span data-ttu-id="fc720-143">Длина не должна превышать 120 символов.</span><span class="sxs-lookup"><span data-stu-id="fc720-143">Must not exceed 120 characters in length.</span></span> <span data-ttu-id="fc720-144">Допустимые `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~` символы: и символы в `0-9` диапазонах, `A-Z` и `a-z` .</span><span class="sxs-lookup"><span data-stu-id="fc720-144">Allowed characters are `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~`, as well as characters in the ranges `0-9`, `A-Z` and `a-z`.</span></span> <span data-ttu-id="fc720-145">Любые другие символы, включая пробелы, не допускаются.</span><span class="sxs-lookup"><span data-stu-id="fc720-145">Any other character, including the space character, are not allowed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fc720-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fc720-146">JSON representation</span></span>

<span data-ttu-id="fc720-147">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fc720-147">Here is a JSON representation of the resource</span></span>

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
