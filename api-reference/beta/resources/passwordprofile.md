---
title: Тип ресурса passwordProfile
description: Содержит профиль пароля, связанный с пользователем. Свойство **passwordProfile** объекта user является объектом **passwordProfile**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: ea3f3daa4807fd56e39930a059d69221e141879c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966237"
---
# <a name="passwordprofile-resource-type"></a><span data-ttu-id="bb18a-104">Тип ресурса passwordProfile</span><span class="sxs-lookup"><span data-stu-id="bb18a-104">passwordProfile resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb18a-p102">Содержит профиль пароля, связанный с пользователем. Свойство **passwordProfile** объекта [user](user.md) является объектом **passwordProfile**.</span><span class="sxs-lookup"><span data-stu-id="bb18a-p102">Contains the password profile associated with a user. The **passwordProfile** property of the [user](user.md) entity is a **passwordProfile** object.</span></span>


## <a name="properties"></a><span data-ttu-id="bb18a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="bb18a-107">Properties</span></span>
| <span data-ttu-id="bb18a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="bb18a-108">Property</span></span>     | <span data-ttu-id="bb18a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="bb18a-109">Type</span></span>   |<span data-ttu-id="bb18a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bb18a-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bb18a-111">forceChangePasswordNextSignIn</span><span class="sxs-lookup"><span data-stu-id="bb18a-111">forceChangePasswordNextSignIn</span></span>|<span data-ttu-id="bb18a-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb18a-112">Boolean</span></span>| <span data-ttu-id="bb18a-113">Если задано **значение true**, при следующем входе пользователь должен изменить пароль.</span><span class="sxs-lookup"><span data-stu-id="bb18a-113">If **true**, at next sign-in, the user must change their password.</span></span> <span data-ttu-id="bb18a-114">После смены пароля этому свойству будет автоматически присвоено значение \***false**.</span><span class="sxs-lookup"><span data-stu-id="bb18a-114">After a password change, this property will be automatically reset to \***false**.</span></span> <span data-ttu-id="bb18a-115">Если не установлено, по умолчанию используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="bb18a-115">If not set, default is **false**.</span></span> |
|<span data-ttu-id="bb18a-116">forceChangePasswordNextSignInWithMfa</span><span class="sxs-lookup"><span data-stu-id="bb18a-116">forceChangePasswordNextSignInWithMfa</span></span>|<span data-ttu-id="bb18a-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="bb18a-117">Boolean</span></span>| <span data-ttu-id="bb18a-118">Если присвоено значение **true**, при следующем входе пользователю необходимо выполнить многофакторную проверку подлинности (MFA) перед принудительной сменой пароля.</span><span class="sxs-lookup"><span data-stu-id="bb18a-118">If **true**, at next sign-in, the user must perform a multi-factor authentication (MFA) before being forced to change their password.</span></span> <span data-ttu-id="bb18a-119">Эта совпадает с действием свойства **forceChangePasswordNextSignIn**, с той разницей, что пользователю сначала нужно выполнить многофакторную проверку подлинности перед изменением пароля.</span><span class="sxs-lookup"><span data-stu-id="bb18a-119">The behavior is identical to **forceChangePasswordNextSignIn** except that the user is required to first perform a multi-factor authentication before password change.</span></span> <span data-ttu-id="bb18a-120">После изменения пароля это свойство автоматически сбрасывается до значения **false**.</span><span class="sxs-lookup"><span data-stu-id="bb18a-120">After a password change, this property will be automatically reset to **false**.</span></span> <span data-ttu-id="bb18a-121">Если не установлено, по умолчанию используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="bb18a-121">If not set, default is **false**.</span></span> |
|<span data-ttu-id="bb18a-122">password</span><span class="sxs-lookup"><span data-stu-id="bb18a-122">password</span></span>|<span data-ttu-id="bb18a-123">Строка</span><span class="sxs-lookup"><span data-stu-id="bb18a-123">String</span></span>|<span data-ttu-id="bb18a-p105">Пароль пользователя. Это свойство обязательно указывать при создании пользователя. Его можно обновить, но пользователю потребуется изменить пароль при следующем входе. Пароль должен соответствовать минимальным требованиям, указанным в свойстве **passwordPolicies** пользователя. По умолчанию требуется надежный пароль.</span><span class="sxs-lookup"><span data-stu-id="bb18a-p105">The password for the user. This property is required when a user is created. It can be updated, but the user will be required to change the password on the next login. The password must satisfy minimum requirements as specified by the user’s **passwordPolicies** property. By default, a strong password is required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bb18a-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bb18a-129">JSON representation</span></span>

<span data-ttu-id="bb18a-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bb18a-130">Here is a JSON representation of the resource</span></span>

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
