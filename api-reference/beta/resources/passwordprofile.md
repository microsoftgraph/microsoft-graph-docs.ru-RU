---
title: Тип ресурса passwordProfile
description: Содержит профиль пароля, связанный с пользователем. Свойство **passwordProfile** объекта user является объектом **passwordProfile**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: users
author: eketo-msft
ms.openlocfilehash: a597b17d09414a839cb0c8d0ae3c944c255ae8ec
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208325"
---
# <a name="passwordprofile-resource-type"></a><span data-ttu-id="49a8c-104">Тип ресурса passwordProfile</span><span class="sxs-lookup"><span data-stu-id="49a8c-104">passwordProfile resource type</span></span>

<span data-ttu-id="49a8c-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49a8c-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49a8c-106">Содержит профиль пароля, связанный с пользователем.</span><span class="sxs-lookup"><span data-stu-id="49a8c-106">Contains the password profile associated with a user.</span></span> <span data-ttu-id="49a8c-107">Свойство **passwordProfile** объекта [user](user.md) является объектом **passwordProfile**.</span><span class="sxs-lookup"><span data-stu-id="49a8c-107">The **passwordProfile** property of the [user](user.md) entity is a **passwordProfile** object.</span></span> <span data-ttu-id="49a8c-108">См. пример [обновления passwordProfile пользователя.](../api/user-update.md#example-3-update-the-passwordprofile-of-a-user-to-reset-their-password)</span><span class="sxs-lookup"><span data-stu-id="49a8c-108">See an example to [Update the passwordProfile of a user](../api/user-update.md#example-3-update-the-passwordprofile-of-a-user-to-reset-their-password).</span></span>


## <a name="properties"></a><span data-ttu-id="49a8c-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="49a8c-109">Properties</span></span>
| <span data-ttu-id="49a8c-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="49a8c-110">Property</span></span>     | <span data-ttu-id="49a8c-111">Тип</span><span class="sxs-lookup"><span data-stu-id="49a8c-111">Type</span></span>   |<span data-ttu-id="49a8c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="49a8c-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="49a8c-113">forceChangePasswordNextSignIn</span><span class="sxs-lookup"><span data-stu-id="49a8c-113">forceChangePasswordNextSignIn</span></span>|<span data-ttu-id="49a8c-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="49a8c-114">Boolean</span></span>|  <span data-ttu-id="49a8c-115">Значение `true` указывает, что пользователь должен изменить свой пароль при следующем входе. В противном случае используется значение `false`.</span><span class="sxs-lookup"><span data-stu-id="49a8c-115">`true` if the user must change her password on the next login; otherwise `false`.</span></span> <span data-ttu-id="49a8c-116">Если значение не задано, по умолчанию используется `false`.</span><span class="sxs-lookup"><span data-stu-id="49a8c-116">If not set, default is `false`.</span></span> <span data-ttu-id="49a8c-117">**ПРИМЕЧАНИЕ.** Для клиентов Azure B2C присвойте значение `false` и вместо этого используйте настраиваемые политики и пользовательские потоки для принудительного сброса пароля при первом входе.</span><span class="sxs-lookup"><span data-stu-id="49a8c-117">**NOTE:**  For Azure B2C tenants, set to `false` and instead use custom policies and user flows to force password reset at first sign in.</span></span> <span data-ttu-id="49a8c-118">См. раздел [Принудительный сброс пароля при первом входе](https://github.com/azure-ad-b2c/samples/tree/master/policies/force-password-reset-first-logon).</span><span class="sxs-lookup"><span data-stu-id="49a8c-118">See [Force password reset at first logon](https://github.com/azure-ad-b2c/samples/tree/master/policies/force-password-reset-first-logon).</span></span> |
|<span data-ttu-id="49a8c-119">forceChangePasswordNextSignInWithMfa</span><span class="sxs-lookup"><span data-stu-id="49a8c-119">forceChangePasswordNextSignInWithMfa</span></span>|<span data-ttu-id="49a8c-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="49a8c-120">Boolean</span></span>| <span data-ttu-id="49a8c-121">Если присвоено значение `true`, при следующем входе пользователю необходимо выполнить многофакторную проверку подлинности (MFA) перед принудительной сменой пароля.</span><span class="sxs-lookup"><span data-stu-id="49a8c-121">If `true`, at next sign-in, the user must perform a multi-factor authentication (MFA) before being forced to change their password.</span></span> <span data-ttu-id="49a8c-122">Эта совпадает с действием свойства **forceChangePasswordNextSignIn**, с той разницей, что перед изменением пароля пользователю нужно выполнить многофакторную проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="49a8c-122">The behavior is identical to **forceChangePasswordNextSignIn** except that the user is required to first perform a multi-factor authentication before password change.</span></span> <span data-ttu-id="49a8c-123">После изменения пароля это свойство автоматически сбрасывается до значения `false`.</span><span class="sxs-lookup"><span data-stu-id="49a8c-123">After a password change, this property will be automatically reset to `false`.</span></span> <span data-ttu-id="49a8c-124">Если значение не задано, по умолчанию используется `false`.</span><span class="sxs-lookup"><span data-stu-id="49a8c-124">If not set, default is `false`.</span></span> |
|<span data-ttu-id="49a8c-125">password</span><span class="sxs-lookup"><span data-stu-id="49a8c-125">password</span></span>|<span data-ttu-id="49a8c-126">Строка</span><span class="sxs-lookup"><span data-stu-id="49a8c-126">String</span></span>|<span data-ttu-id="49a8c-p105">Пароль пользователя. Это свойство обязательно указывать при создании пользователя. Его можно обновить, но пользователю потребуется изменить пароль при следующем входе. Пароль должен соответствовать минимальным требованиям, указанным в свойстве **passwordPolicies** пользователя. По умолчанию требуется надежный пароль.</span><span class="sxs-lookup"><span data-stu-id="49a8c-p105">The password for the user. This property is required when a user is created. It can be updated, but the user will be required to change the password on the next login. The password must satisfy minimum requirements as specified by the user’s **passwordPolicies** property. By default, a strong password is required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="49a8c-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="49a8c-132">JSON representation</span></span>

<span data-ttu-id="49a8c-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="49a8c-133">Here is a JSON representation of the resource</span></span>

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


