---
title: Тип ресурса passwordProfile
description: Содержит профиль пароля, связанный с пользователем. Свойство **passwordProfile** объекта user является объектом **passwordProfile**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: users
author: eketo-msft
ms.openlocfilehash: 7c0f31310227753caf3949a32046f067b4117770
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030868"
---
# <a name="passwordprofile-resource-type"></a><span data-ttu-id="8fe46-104">Тип ресурса passwordProfile</span><span class="sxs-lookup"><span data-stu-id="8fe46-104">passwordProfile resource type</span></span>

<span data-ttu-id="8fe46-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8fe46-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8fe46-p102">Содержит профиль пароля, связанный с пользователем. Свойство **passwordProfile** объекта [user](user.md) является объектом **passwordProfile**.</span><span class="sxs-lookup"><span data-stu-id="8fe46-p102">Contains the password profile associated with a user. The **passwordProfile** property of the [user](user.md) entity is a **passwordProfile** object.</span></span>


## <a name="properties"></a><span data-ttu-id="8fe46-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="8fe46-108">Properties</span></span>
| <span data-ttu-id="8fe46-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="8fe46-109">Property</span></span>     | <span data-ttu-id="8fe46-110">Тип</span><span class="sxs-lookup"><span data-stu-id="8fe46-110">Type</span></span>   |<span data-ttu-id="8fe46-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8fe46-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8fe46-112">forceChangePasswordNextSignIn</span><span class="sxs-lookup"><span data-stu-id="8fe46-112">forceChangePasswordNextSignIn</span></span>|<span data-ttu-id="8fe46-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fe46-113">Boolean</span></span>|  <span data-ttu-id="8fe46-114">Значение `true` указывает, что пользователь должен изменить свой пароль при следующем входе. В противном случае используется значение `false`.</span><span class="sxs-lookup"><span data-stu-id="8fe46-114">`true` if the user must change her password on the next login; otherwise `false`.</span></span> <span data-ttu-id="8fe46-115">Если значение не задано, по умолчанию используется `false`.</span><span class="sxs-lookup"><span data-stu-id="8fe46-115">If not set, default is `false`.</span></span> <span data-ttu-id="8fe46-116">**ПРИМЕЧАНИЕ:**  Для клиентов Azure B2C установите настраиваемые политики и потоки пользователей для принудительного сброса пароля при `false` первом входе.</span><span class="sxs-lookup"><span data-stu-id="8fe46-116">**NOTE:**  For Azure B2C tenants, set to `false` and instead use custom policies and user flows to force password reset at first sign in.</span></span> <span data-ttu-id="8fe46-117">См. раздел [Принудительный сброс пароля при первом входе](https://github.com/azure-ad-b2c/samples/tree/master/policies/force-password-reset-first-logon).</span><span class="sxs-lookup"><span data-stu-id="8fe46-117">See [Force password reset at first logon](https://github.com/azure-ad-b2c/samples/tree/master/policies/force-password-reset-first-logon).</span></span> |
|<span data-ttu-id="8fe46-118">forceChangePasswordNextSignInWithMfa</span><span class="sxs-lookup"><span data-stu-id="8fe46-118">forceChangePasswordNextSignInWithMfa</span></span>|<span data-ttu-id="8fe46-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="8fe46-119">Boolean</span></span>| <span data-ttu-id="8fe46-120">Если присвоено значение `true`, при следующем входе пользователю необходимо выполнить многофакторную проверку подлинности (MFA) перед принудительной сменой пароля.</span><span class="sxs-lookup"><span data-stu-id="8fe46-120">If `true`, at next sign-in, the user must perform a multi-factor authentication (MFA) before being forced to change their password.</span></span> <span data-ttu-id="8fe46-121">Эта совпадает с действием свойства **forceChangePasswordNextSignIn**, с той разницей, что перед изменением пароля пользователю нужно выполнить многофакторную проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="8fe46-121">The behavior is identical to **forceChangePasswordNextSignIn** except that the user is required to first perform a multi-factor authentication before password change.</span></span> <span data-ttu-id="8fe46-122">После изменения пароля это свойство автоматически сбрасывается до значения `false`.</span><span class="sxs-lookup"><span data-stu-id="8fe46-122">After a password change, this property will be automatically reset to `false`.</span></span> <span data-ttu-id="8fe46-123">Если значение не задано, по умолчанию используется `false`.</span><span class="sxs-lookup"><span data-stu-id="8fe46-123">If not set, default is `false`.</span></span> |
|<span data-ttu-id="8fe46-124">password</span><span class="sxs-lookup"><span data-stu-id="8fe46-124">password</span></span>|<span data-ttu-id="8fe46-125">Строка</span><span class="sxs-lookup"><span data-stu-id="8fe46-125">String</span></span>|<span data-ttu-id="8fe46-p105">Пароль пользователя. Это свойство обязательно указывать при создании пользователя. Его можно обновить, но пользователю потребуется изменить пароль при следующем входе. Пароль должен соответствовать минимальным требованиям, указанным в свойстве **passwordPolicies** пользователя. По умолчанию требуется надежный пароль.</span><span class="sxs-lookup"><span data-stu-id="8fe46-p105">The password for the user. This property is required when a user is created. It can be updated, but the user will be required to change the password on the next login. The password must satisfy minimum requirements as specified by the user’s **passwordPolicies** property. By default, a strong password is required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8fe46-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8fe46-131">JSON representation</span></span>

<span data-ttu-id="8fe46-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8fe46-132">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "passwordProfile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


