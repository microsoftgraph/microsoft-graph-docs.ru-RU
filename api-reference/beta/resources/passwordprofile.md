---
title: Тип ресурса passwordProfile
description: Содержит профиль пароля, связанный с пользователем. Свойство **passwordProfile** объекта user является объектом **passwordProfile**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: users
author: eketo-msft
ms.openlocfilehash: 47c55261316f2d85d27a4c993b358676578e74fd
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911335"
---
# <a name="passwordprofile-resource-type"></a><span data-ttu-id="d8c21-104">Тип ресурса passwordProfile</span><span class="sxs-lookup"><span data-stu-id="d8c21-104">passwordProfile resource type</span></span>

<span data-ttu-id="d8c21-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8c21-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8c21-p102">Содержит профиль пароля, связанный с пользователем. Свойство **passwordProfile** объекта [user](user.md) является объектом **passwordProfile**.</span><span class="sxs-lookup"><span data-stu-id="d8c21-p102">Contains the password profile associated with a user. The **passwordProfile** property of the [user](user.md) entity is a **passwordProfile** object.</span></span>


## <a name="properties"></a><span data-ttu-id="d8c21-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d8c21-108">Properties</span></span>
| <span data-ttu-id="d8c21-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d8c21-109">Property</span></span>     | <span data-ttu-id="d8c21-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d8c21-110">Type</span></span>   |<span data-ttu-id="d8c21-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d8c21-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d8c21-112">forceChangePasswordNextSignIn</span><span class="sxs-lookup"><span data-stu-id="d8c21-112">forceChangePasswordNextSignIn</span></span>|<span data-ttu-id="d8c21-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8c21-113">Boolean</span></span>| <span data-ttu-id="d8c21-114">Если при следующем входе пользователь `true` должен изменить пароль.</span><span class="sxs-lookup"><span data-stu-id="d8c21-114">If `true`, at next sign-in, the user must change their password.</span></span> <span data-ttu-id="d8c21-115">После изменения пароля это свойство будет автоматически сброшено на \* `false` .</span><span class="sxs-lookup"><span data-stu-id="d8c21-115">After a password change, this property will be automatically reset to \*`false`.</span></span> <span data-ttu-id="d8c21-116">Если не установлено, по умолчанию `false` .</span><span class="sxs-lookup"><span data-stu-id="d8c21-116">If not set, default is `false`.</span></span> |
|<span data-ttu-id="d8c21-117">forceChangePasswordNextSignInWithMfa</span><span class="sxs-lookup"><span data-stu-id="d8c21-117">forceChangePasswordNextSignInWithMfa</span></span>|<span data-ttu-id="d8c21-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8c21-118">Boolean</span></span>| <span data-ttu-id="d8c21-119">Если при следующем входе пользователь должен выполнить многофакторную проверку подлинности (MFA), прежде чем его принудить `true` изменить пароль.</span><span class="sxs-lookup"><span data-stu-id="d8c21-119">If `true`, at next sign-in, the user must perform a multi-factor authentication (MFA) before being forced to change their password.</span></span> <span data-ttu-id="d8c21-120">Эта совпадает с действием свойства **forceChangePasswordNextSignIn**, с той разницей, что пользователю сначала нужно выполнить многофакторную проверку подлинности перед изменением пароля.</span><span class="sxs-lookup"><span data-stu-id="d8c21-120">The behavior is identical to **forceChangePasswordNextSignIn** except that the user is required to first perform a multi-factor authentication before password change.</span></span> <span data-ttu-id="d8c21-121">После изменения пароля это свойство будет автоматически сброшено на `false` .</span><span class="sxs-lookup"><span data-stu-id="d8c21-121">After a password change, this property will be automatically reset to `false`.</span></span> <span data-ttu-id="d8c21-122">Если не установлено, по умолчанию `false` .</span><span class="sxs-lookup"><span data-stu-id="d8c21-122">If not set, default is `false`.</span></span> |
|<span data-ttu-id="d8c21-123">password</span><span class="sxs-lookup"><span data-stu-id="d8c21-123">password</span></span>|<span data-ttu-id="d8c21-124">Строка</span><span class="sxs-lookup"><span data-stu-id="d8c21-124">String</span></span>|<span data-ttu-id="d8c21-p105">Пароль пользователя. Это свойство обязательно указывать при создании пользователя. Его можно обновить, но пользователю потребуется изменить пароль при следующем входе. Пароль должен соответствовать минимальным требованиям, указанным в свойстве **passwordPolicies** пользователя. По умолчанию требуется надежный пароль.</span><span class="sxs-lookup"><span data-stu-id="d8c21-p105">The password for the user. This property is required when a user is created. It can be updated, but the user will be required to change the password on the next login. The password must satisfy minimum requirements as specified by the user’s **passwordPolicies** property. By default, a strong password is required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d8c21-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d8c21-130">JSON representation</span></span>

<span data-ttu-id="d8c21-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d8c21-131">Here is a JSON representation of the resource</span></span>

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


