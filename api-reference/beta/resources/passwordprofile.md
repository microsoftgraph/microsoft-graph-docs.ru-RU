---
title: Тип ресурса passwordProfile
description: Содержит профиль пароля, связанный с пользователем. Свойство **passwordProfile** объекта user является объектом **passwordProfile**.
localization_priority: Normal
ms.openlocfilehash: 11930b046fafaf89f8db751891b9b7f2f72fd99d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839006"
---
# <a name="passwordprofile-resource-type"></a><span data-ttu-id="e2d13-104">Тип ресурса passwordProfile</span><span class="sxs-lookup"><span data-stu-id="e2d13-104">passwordProfile resource type</span></span>

> <span data-ttu-id="e2d13-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e2d13-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e2d13-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2d13-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e2d13-p103">Содержит профиль пароля, связанный с пользователем. Свойство **passwordProfile** объекта [user](user.md) является объектом **passwordProfile**.</span><span class="sxs-lookup"><span data-stu-id="e2d13-p103">Contains the password profile associated with a user. The **passwordProfile** property of the [user](user.md) entity is a **passwordProfile** object.</span></span>


## <a name="properties"></a><span data-ttu-id="e2d13-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="e2d13-109">Properties</span></span>
| <span data-ttu-id="e2d13-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="e2d13-110">Property</span></span>     | <span data-ttu-id="e2d13-111">Тип</span><span class="sxs-lookup"><span data-stu-id="e2d13-111">Type</span></span>   |<span data-ttu-id="e2d13-112">Описание</span><span class="sxs-lookup"><span data-stu-id="e2d13-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e2d13-113">forceChangePasswordNextSignIn</span><span class="sxs-lookup"><span data-stu-id="e2d13-113">forceChangePasswordNextSignIn</span></span>|<span data-ttu-id="e2d13-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2d13-114">Boolean</span></span>| <span data-ttu-id="e2d13-115">Если **значение true**, при следующем входе на, пользователь должен изменить пароль.</span><span class="sxs-lookup"><span data-stu-id="e2d13-115">If **true**, at next sign-in, the user must change their password.</span></span> <span data-ttu-id="e2d13-116">После изменения пароля, это свойство будет автоматически изменено на \***значение false**.</span><span class="sxs-lookup"><span data-stu-id="e2d13-116">After a password change, this property will be automatically reset to \***false**.</span></span> <span data-ttu-id="e2d13-117">Если не задан, по умолчанию — **false**.</span><span class="sxs-lookup"><span data-stu-id="e2d13-117">If not set, default is **false**.</span></span> |
|<span data-ttu-id="e2d13-118">forceChangePasswordNextSignInWithMfa</span><span class="sxs-lookup"><span data-stu-id="e2d13-118">forceChangePasswordNextSignInWithMfa</span></span>|<span data-ttu-id="e2d13-119">Логический</span><span class="sxs-lookup"><span data-stu-id="e2d13-119">Boolean</span></span>| <span data-ttu-id="e2d13-120">Если **значение true**, при следующем входе на, пользователь должен выполнить многофакторная проверка подлинности (многофакторной проверкой Подлинности) перед принудительно изменять свои пароли.</span><span class="sxs-lookup"><span data-stu-id="e2d13-120">If **true**, at next sign-in, the user must perform a multi-factor authentication (MFA) before being forced to change their password.</span></span> <span data-ttu-id="e2d13-121">Поведение идентично **forceChangePasswordNextSignIn** , за исключением того, что пользователь необходимо сначала выполнить многофакторной проверки подлинности до изменения пароля.</span><span class="sxs-lookup"><span data-stu-id="e2d13-121">The behavior is identical to **forceChangePasswordNextSignIn** except that the user is required to first perform a multi-factor authentication before password change.</span></span> <span data-ttu-id="e2d13-122">После изменения пароля это свойство будет автоматически задано **значение false**.</span><span class="sxs-lookup"><span data-stu-id="e2d13-122">After a password change, this property will be automatically reset to **false**.</span></span> <span data-ttu-id="e2d13-123">Если не задан, по умолчанию — **false**.</span><span class="sxs-lookup"><span data-stu-id="e2d13-123">If not set, default is **false**.</span></span> |
|<span data-ttu-id="e2d13-124">password</span><span class="sxs-lookup"><span data-stu-id="e2d13-124">password</span></span>|<span data-ttu-id="e2d13-125">Строка</span><span class="sxs-lookup"><span data-stu-id="e2d13-125">String</span></span>|<span data-ttu-id="e2d13-p106">Пароль пользователя. Это свойство обязательно указывать при создании пользователя. Его можно обновить, но пользователю потребуется изменить пароль при следующем входе. Пароль должен соответствовать минимальным требованиям, указанным в свойстве **passwordPolicies** пользователя. По умолчанию требуется надежный пароль.</span><span class="sxs-lookup"><span data-stu-id="e2d13-p106">The password for the user. This property is required when a user is created. It can be updated, but the user will be required to change the password on the next login. The password must satisfy minimum requirements as specified by the user’s **passwordPolicies** property. By default, a strong password is required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e2d13-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e2d13-131">JSON representation</span></span>

<span data-ttu-id="e2d13-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e2d13-132">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordprofile"
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
