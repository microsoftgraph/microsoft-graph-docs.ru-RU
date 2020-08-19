---
title: Тип ресурса passwordProfile
description: Содержит профиль пароля, связанный с пользователем. Свойство **passwordProfile** объекта user является объектом **passwordProfile**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: eketo-msft
ms.openlocfilehash: 4fdc58e79487b9577685929bb06865e3aca6906f
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812487"
---
# <a name="passwordprofile-resource-type"></a><span data-ttu-id="c9659-104">Тип ресурса passwordProfile</span><span class="sxs-lookup"><span data-stu-id="c9659-104">passwordProfile resource type</span></span>

<span data-ttu-id="c9659-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9659-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9659-p102">Содержит профиль пароля, связанный с пользователем. Свойство **passwordProfile** объекта [user](user.md) является объектом **passwordProfile**.</span><span class="sxs-lookup"><span data-stu-id="c9659-p102">Contains the password profile associated with a user. The **passwordProfile** property of the [user](user.md) entity is a **passwordProfile** object.</span></span>


## <a name="properties"></a><span data-ttu-id="c9659-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c9659-108">Properties</span></span>
| <span data-ttu-id="c9659-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c9659-109">Property</span></span>     | <span data-ttu-id="c9659-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c9659-110">Type</span></span>   |<span data-ttu-id="c9659-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c9659-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9659-112">forceChangePasswordNextSignIn</span><span class="sxs-lookup"><span data-stu-id="c9659-112">forceChangePasswordNextSignIn</span></span>|<span data-ttu-id="c9659-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9659-113">Boolean</span></span>| <span data-ttu-id="c9659-114">Если задано **значение true**, при следующем входе пользователь должен изменить пароль.</span><span class="sxs-lookup"><span data-stu-id="c9659-114">If **true**, at next sign-in, the user must change their password.</span></span> <span data-ttu-id="c9659-115">После смены пароля этому свойству будет автоматически присвоено значение \***false**.</span><span class="sxs-lookup"><span data-stu-id="c9659-115">After a password change, this property will be automatically reset to \***false**.</span></span> <span data-ttu-id="c9659-116">Если не установлено, по умолчанию используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="c9659-116">If not set, default is **false**.</span></span> |
|<span data-ttu-id="c9659-117">forceChangePasswordNextSignInWithMfa</span><span class="sxs-lookup"><span data-stu-id="c9659-117">forceChangePasswordNextSignInWithMfa</span></span>|<span data-ttu-id="c9659-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9659-118">Boolean</span></span>| <span data-ttu-id="c9659-119">Если присвоено значение **true**, при следующем входе пользователю необходимо выполнить многофакторную проверку подлинности (MFA) перед принудительной сменой пароля.</span><span class="sxs-lookup"><span data-stu-id="c9659-119">If **true**, at next sign-in, the user must perform a multi-factor authentication (MFA) before being forced to change their password.</span></span> <span data-ttu-id="c9659-120">Эта совпадает с действием свойства **forceChangePasswordNextSignIn**, с той разницей, что пользователю сначала нужно выполнить многофакторную проверку подлинности перед изменением пароля.</span><span class="sxs-lookup"><span data-stu-id="c9659-120">The behavior is identical to **forceChangePasswordNextSignIn** except that the user is required to first perform a multi-factor authentication before password change.</span></span> <span data-ttu-id="c9659-121">После изменения пароля это свойство автоматически сбрасывается до значения **false**.</span><span class="sxs-lookup"><span data-stu-id="c9659-121">After a password change, this property will be automatically reset to **false**.</span></span> <span data-ttu-id="c9659-122">Если не установлено, по умолчанию используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="c9659-122">If not set, default is **false**.</span></span> |
|<span data-ttu-id="c9659-123">password</span><span class="sxs-lookup"><span data-stu-id="c9659-123">password</span></span>|<span data-ttu-id="c9659-124">Строка</span><span class="sxs-lookup"><span data-stu-id="c9659-124">String</span></span>|<span data-ttu-id="c9659-p105">Пароль пользователя. Это свойство обязательно указывать при создании пользователя. Его можно обновить, но пользователю потребуется изменить пароль при следующем входе. Пароль должен соответствовать минимальным требованиям, указанным в свойстве **passwordPolicies** пользователя. По умолчанию требуется надежный пароль.</span><span class="sxs-lookup"><span data-stu-id="c9659-p105">The password for the user. This property is required when a user is created. It can be updated, but the user will be required to change the password on the next login. The password must satisfy minimum requirements as specified by the user’s **passwordPolicies** property. By default, a strong password is required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c9659-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c9659-130">JSON representation</span></span>

<span data-ttu-id="c9659-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c9659-131">Here is a JSON representation of the resource</span></span>

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
