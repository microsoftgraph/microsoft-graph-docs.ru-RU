---
title: Тип ресурса passwordProfile
description: Содержит профиль пароля, связанный с пользователем. Свойство **passwordProfile** объекта user является объектом **passwordProfile**.
localization_priority: Priority
ms.openlocfilehash: cea8dcc114cb599a2d857ced67ac25c9eb275497
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462503"
---
# <a name="passwordprofile-resource-type"></a><span data-ttu-id="24f74-104">Тип ресурса passwordProfile</span><span class="sxs-lookup"><span data-stu-id="24f74-104">passwordProfile resource type</span></span>

<span data-ttu-id="24f74-p102">Содержит профиль пароля, связанный с пользователем. Свойство **passwordProfile** объекта [user](user.md) является объектом **passwordProfile**.</span><span class="sxs-lookup"><span data-stu-id="24f74-p102">Contains the password profile associated with a user. The **passwordProfile** property of the [user](user.md) entity is a **passwordProfile** object.</span></span>


## <a name="properties"></a><span data-ttu-id="24f74-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="24f74-107">Properties</span></span>
| <span data-ttu-id="24f74-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="24f74-108">Property</span></span>     | <span data-ttu-id="24f74-109">Тип</span><span class="sxs-lookup"><span data-stu-id="24f74-109">Type</span></span>   |<span data-ttu-id="24f74-110">Описание</span><span class="sxs-lookup"><span data-stu-id="24f74-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="24f74-111">forceChangePasswordNextSignIn</span><span class="sxs-lookup"><span data-stu-id="24f74-111">forceChangePasswordNextSignIn</span></span>|<span data-ttu-id="24f74-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="24f74-112">Boolean</span></span>| <span data-ttu-id="24f74-113">Значение **true** указывает, что пользователь должен изменить свой пароль при следующем входе. В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="24f74-113">**true** if the user must change her password on the next login; otherwise **false**.</span></span> |
|<span data-ttu-id="24f74-114">forceChangePasswordNextSignInWithMfa</span><span class="sxs-lookup"><span data-stu-id="24f74-114">forceChangePasswordNextSignInWithMfa</span></span>|<span data-ttu-id="24f74-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="24f74-115">Boolean</span></span>| <span data-ttu-id="24f74-116">Если присвоено значение **true**, при следующем входе пользователю необходимо выполнить многофакторную проверку подлинности (MFA) перед принудительной сменой пароля.</span><span class="sxs-lookup"><span data-stu-id="24f74-116">If **true**, at next sign-in, the user must perform a multi-factor authentication (MFA) before being forced to change their password.</span></span> <span data-ttu-id="24f74-117">Эта совпадает с действием свойства **forceChangePasswordNextSignIn**, с той разницей, что пользователю сначала нужно выполнить многофакторную проверку подлинности перед изменением пароля.</span><span class="sxs-lookup"><span data-stu-id="24f74-117">The behavior is identical to **forceChangePasswordNextSignIn** except that the user is required to first perform a multi-factor authentication before password change.</span></span> <span data-ttu-id="24f74-118">После изменения пароля это свойство автоматически сбрасывается до значения **false**.</span><span class="sxs-lookup"><span data-stu-id="24f74-118">After a password change, this property will be automatically reset to **false**.</span></span> <span data-ttu-id="24f74-119">Если не установлено, по умолчанию используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="24f74-119">If not set, default is **false**.</span></span> |
|<span data-ttu-id="24f74-120">password</span><span class="sxs-lookup"><span data-stu-id="24f74-120">password</span></span>|<span data-ttu-id="24f74-121">Строка</span><span class="sxs-lookup"><span data-stu-id="24f74-121">String</span></span>|<span data-ttu-id="24f74-p104">Пароль пользователя. Это свойство обязательно указывать при создании пользователя. Его можно обновить, но пользователю потребуется изменить пароль при следующем входе. Пароль должен соответствовать минимальным требованиям, указанным в свойстве **passwordPolicies** пользователя. По умолчанию требуется надежный пароль.</span><span class="sxs-lookup"><span data-stu-id="24f74-p104">The password for the user. This property is required when a user is created. It can be updated, but the user will be required to change the password on the next login. The password must satisfy minimum requirements as specified by the user’s **passwordPolicies** property. By default, a strong password is required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="24f74-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="24f74-127">JSON representation</span></span>

<span data-ttu-id="24f74-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="24f74-128">Here is a JSON representation of the resource</span></span>

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
