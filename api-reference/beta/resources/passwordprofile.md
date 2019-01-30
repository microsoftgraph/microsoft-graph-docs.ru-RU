---
title: Тип ресурса passwordProfile
description: Содержит профиль пароля, связанный с пользователем. Свойство **passwordProfile** объекта user является объектом **passwordProfile**.
localization_priority: Normal
ms.openlocfilehash: 3caff59c8fd0838b91f9fdfb79bdbb154aa83b9f
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642900"
---
# <a name="passwordprofile-resource-type"></a><span data-ttu-id="33968-104">Тип ресурса passwordProfile</span><span class="sxs-lookup"><span data-stu-id="33968-104">passwordProfile resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33968-p102">Содержит профиль пароля, связанный с пользователем. Свойство **passwordProfile** объекта [user](user.md) является объектом **passwordProfile**.</span><span class="sxs-lookup"><span data-stu-id="33968-p102">Contains the password profile associated with a user. The **passwordProfile** property of the [user](user.md) entity is a **passwordProfile** object.</span></span>


## <a name="properties"></a><span data-ttu-id="33968-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="33968-107">Properties</span></span>
| <span data-ttu-id="33968-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="33968-108">Property</span></span>     | <span data-ttu-id="33968-109">Тип</span><span class="sxs-lookup"><span data-stu-id="33968-109">Type</span></span>   |<span data-ttu-id="33968-110">Описание</span><span class="sxs-lookup"><span data-stu-id="33968-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="33968-111">forceChangePasswordNextSignIn</span><span class="sxs-lookup"><span data-stu-id="33968-111">forceChangePasswordNextSignIn</span></span>|<span data-ttu-id="33968-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="33968-112">Boolean</span></span>| <span data-ttu-id="33968-113">Если **значение true**, при следующем входе на, пользователь должен изменить пароль.</span><span class="sxs-lookup"><span data-stu-id="33968-113">If **true**, at next sign-in, the user must change their password.</span></span> <span data-ttu-id="33968-114">После изменения пароля, это свойство будет автоматически изменено на \***значение false**.</span><span class="sxs-lookup"><span data-stu-id="33968-114">After a password change, this property will be automatically reset to \***false**.</span></span> <span data-ttu-id="33968-115">Если не установлено, по умолчанию используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="33968-115">If not set, default is **false**.</span></span> |
|<span data-ttu-id="33968-116">forceChangePasswordNextSignInWithMfa</span><span class="sxs-lookup"><span data-stu-id="33968-116">forceChangePasswordNextSignInWithMfa</span></span>|<span data-ttu-id="33968-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="33968-117">Boolean</span></span>| <span data-ttu-id="33968-118">Если присвоено значение **true**, при следующем входе пользователю необходимо выполнить многофакторную проверку подлинности (MFA) перед принудительной сменой пароля.</span><span class="sxs-lookup"><span data-stu-id="33968-118">If **true**, at next sign-in, the user must perform a multi-factor authentication (MFA) before being forced to change their password.</span></span> <span data-ttu-id="33968-119">Эта совпадает с действием свойства **forceChangePasswordNextSignIn**, с той разницей, что пользователю сначала нужно выполнить многофакторную проверку подлинности перед изменением пароля.</span><span class="sxs-lookup"><span data-stu-id="33968-119">The behavior is identical to **forceChangePasswordNextSignIn** except that the user is required to first perform a multi-factor authentication before password change.</span></span> <span data-ttu-id="33968-120">После изменения пароля это свойство автоматически сбрасывается до значения **false**.</span><span class="sxs-lookup"><span data-stu-id="33968-120">After a password change, this property will be automatically reset to **false**.</span></span> <span data-ttu-id="33968-121">Если не установлено, по умолчанию используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="33968-121">If not set, default is **false**.</span></span> |
|<span data-ttu-id="33968-122">password</span><span class="sxs-lookup"><span data-stu-id="33968-122">password</span></span>|<span data-ttu-id="33968-123">Строка</span><span class="sxs-lookup"><span data-stu-id="33968-123">String</span></span>|<span data-ttu-id="33968-p105">Пароль пользователя. Это свойство обязательно указывать при создании пользователя. Его можно обновить, но пользователю потребуется изменить пароль при следующем входе. Пароль должен соответствовать минимальным требованиям, указанным в свойстве **passwordPolicies** пользователя. По умолчанию требуется надежный пароль.</span><span class="sxs-lookup"><span data-stu-id="33968-p105">The password for the user. This property is required when a user is created. It can be updated, but the user will be required to change the password on the next login. The password must satisfy minimum requirements as specified by the user’s **passwordPolicies** property. By default, a strong password is required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="33968-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="33968-129">JSON representation</span></span>

<span data-ttu-id="33968-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="33968-130">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "passwordProfile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/passwordprofile.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
