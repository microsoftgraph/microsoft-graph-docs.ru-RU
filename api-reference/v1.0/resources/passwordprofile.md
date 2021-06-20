---
title: Тип ресурса passwordProfile
description: Содержит профиль пароля, связанный с пользователем. Свойство **passwordProfile** объекта user является объектом **passwordProfile**.
localization_priority: Priority
author: eketo-msft
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 9caae60a2eb82acd82101f3ee9c723b8c0545e39
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030959"
---
# <a name="passwordprofile-resource-type"></a><span data-ttu-id="75645-104">Тип ресурса passwordProfile</span><span class="sxs-lookup"><span data-stu-id="75645-104">passwordProfile resource type</span></span>

<span data-ttu-id="75645-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75645-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="75645-p102">Содержит профиль пароля, связанный с пользователем. Свойство **passwordProfile** объекта [user](user.md) является объектом **passwordProfile**.</span><span class="sxs-lookup"><span data-stu-id="75645-p102">Contains the password profile associated with a user. The **passwordProfile** property of the [user](user.md) entity is a **passwordProfile** object.</span></span>


## <a name="properties"></a><span data-ttu-id="75645-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="75645-108">Properties</span></span>
| <span data-ttu-id="75645-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="75645-109">Property</span></span>     | <span data-ttu-id="75645-110">Тип</span><span class="sxs-lookup"><span data-stu-id="75645-110">Type</span></span>   |<span data-ttu-id="75645-111">Описание</span><span class="sxs-lookup"><span data-stu-id="75645-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="75645-112">forceChangePasswordNextSignIn</span><span class="sxs-lookup"><span data-stu-id="75645-112">forceChangePasswordNextSignIn</span></span>|<span data-ttu-id="75645-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="75645-113">Boolean</span></span>| <span data-ttu-id="75645-114">Значение `true` указывает, что пользователь должен изменить свой пароль при следующем входе. В противном случае используется значение `false`.</span><span class="sxs-lookup"><span data-stu-id="75645-114">`true` if the user must change her password on the next login; otherwise `false`.</span></span> <span data-ttu-id="75645-115">Если значение не задано, по умолчанию используется `false`.</span><span class="sxs-lookup"><span data-stu-id="75645-115">If not set, default is `false`.</span></span> <span data-ttu-id="75645-116">**ПРИМЕЧАНИЕ.** Для клиентов Azure B2C присвойте значение `false` и вместо этого используйте настраиваемые политики и пользовательские потоки для принудительного сброса пароля при первом входе.</span><span class="sxs-lookup"><span data-stu-id="75645-116">**NOTE:**  For Azure B2C tenants, set to `false` and instead use custom policies and user flows to force password reset at first sign in.</span></span> <span data-ttu-id="75645-117">См. раздел [Принудительный сброс пароля при первом входе](https://github.com/azure-ad-b2c/samples/tree/master/policies/force-password-reset-first-logon).</span><span class="sxs-lookup"><span data-stu-id="75645-117">See [Force password reset at first logon](https://github.com/azure-ad-b2c/samples/tree/master/policies/force-password-reset-first-logon).</span></span>|
|<span data-ttu-id="75645-118">forceChangePasswordNextSignInWithMfa</span><span class="sxs-lookup"><span data-stu-id="75645-118">forceChangePasswordNextSignInWithMfa</span></span>|<span data-ttu-id="75645-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="75645-119">Boolean</span></span>| <span data-ttu-id="75645-120">Если присвоено значение `true`, при следующем входе пользователю необходимо выполнить многофакторную проверку подлинности (MFA) перед принудительной сменой пароля.</span><span class="sxs-lookup"><span data-stu-id="75645-120">If `true`, at next sign-in, the user must perform a multi-factor authentication (MFA) before being forced to change their password.</span></span> <span data-ttu-id="75645-121">Эта совпадает с действием свойства **forceChangePasswordNextSignIn**, с той разницей, что перед изменением пароля пользователю нужно выполнить многофакторную проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="75645-121">The behavior is identical to **forceChangePasswordNextSignIn** except that the user is required to first perform a multi-factor authentication before password change.</span></span> <span data-ttu-id="75645-122">После изменения пароля это свойство автоматически сбрасывается до значения `false`.</span><span class="sxs-lookup"><span data-stu-id="75645-122">After a password change, this property will be automatically reset to `false`.</span></span> <span data-ttu-id="75645-123">Если значение не задано, по умолчанию используется `false`.</span><span class="sxs-lookup"><span data-stu-id="75645-123">If not set, default is `false`.</span></span> |
|<span data-ttu-id="75645-124">password</span><span class="sxs-lookup"><span data-stu-id="75645-124">password</span></span>|<span data-ttu-id="75645-125">Строка</span><span class="sxs-lookup"><span data-stu-id="75645-125">String</span></span>|<span data-ttu-id="75645-p105">Пароль пользователя. Это свойство обязательно указывать при создании пользователя. Его можно обновить, но пользователю потребуется изменить пароль при следующем входе. Пароль должен соответствовать минимальным требованиям, указанным в свойстве **passwordPolicies** пользователя. По умолчанию требуется надежный пароль.</span><span class="sxs-lookup"><span data-stu-id="75645-p105">The password for the user. This property is required when a user is created. It can be updated, but the user will be required to change the password on the next login. The password must satisfy minimum requirements as specified by the user’s **passwordPolicies** property. By default, a strong password is required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="75645-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="75645-131">JSON representation</span></span>

<span data-ttu-id="75645-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="75645-132">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordProfile"
}-->

```json
{
  "forceChangePasswordNextSignIn": true,
  "forceChangePasswordNextSignInWithMfa": false,
  "password": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordProfile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

