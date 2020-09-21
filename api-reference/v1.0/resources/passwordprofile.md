---
title: Тип ресурса passwordProfile
description: Содержит профиль пароля, связанный с пользователем. Свойство **passwordProfile** объекта user является объектом **passwordProfile**.
localization_priority: Priority
author: eketo-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 5f5df66e664bac8dd873166d2f970ac0a0308faa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47967326"
---
# <a name="passwordprofile-resource-type"></a><span data-ttu-id="33466-104">Тип ресурса passwordProfile</span><span class="sxs-lookup"><span data-stu-id="33466-104">passwordProfile resource type</span></span>

<span data-ttu-id="33466-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33466-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="33466-p102">Содержит профиль пароля, связанный с пользователем. Свойство **passwordProfile** объекта [user](user.md) является объектом **passwordProfile**.</span><span class="sxs-lookup"><span data-stu-id="33466-p102">Contains the password profile associated with a user. The **passwordProfile** property of the [user](user.md) entity is a **passwordProfile** object.</span></span>


## <a name="properties"></a><span data-ttu-id="33466-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="33466-108">Properties</span></span>
| <span data-ttu-id="33466-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="33466-109">Property</span></span>     | <span data-ttu-id="33466-110">Тип</span><span class="sxs-lookup"><span data-stu-id="33466-110">Type</span></span>   |<span data-ttu-id="33466-111">Описание</span><span class="sxs-lookup"><span data-stu-id="33466-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="33466-112">forceChangePasswordNextSignIn</span><span class="sxs-lookup"><span data-stu-id="33466-112">forceChangePasswordNextSignIn</span></span>|<span data-ttu-id="33466-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="33466-113">Boolean</span></span>| <span data-ttu-id="33466-114">Значение **true** указывает, что пользователь должен изменить свой пароль при следующем входе. В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="33466-114">**true** if the user must change her password on the next login; otherwise **false**.</span></span> |
|<span data-ttu-id="33466-115">forceChangePasswordNextSignInWithMfa</span><span class="sxs-lookup"><span data-stu-id="33466-115">forceChangePasswordNextSignInWithMfa</span></span>|<span data-ttu-id="33466-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="33466-116">Boolean</span></span>| <span data-ttu-id="33466-117">Если присвоено значение **true**, при следующем входе пользователю необходимо выполнить многофакторную проверку подлинности (MFA) перед принудительной сменой пароля.</span><span class="sxs-lookup"><span data-stu-id="33466-117">If **true**, at next sign-in, the user must perform a multi-factor authentication (MFA) before being forced to change their password.</span></span> <span data-ttu-id="33466-118">Эта совпадает с действием свойства **forceChangePasswordNextSignIn**, с той разницей, что пользователю сначала нужно выполнить многофакторную проверку подлинности перед изменением пароля.</span><span class="sxs-lookup"><span data-stu-id="33466-118">The behavior is identical to **forceChangePasswordNextSignIn** except that the user is required to first perform a multi-factor authentication before password change.</span></span> <span data-ttu-id="33466-119">После изменения пароля это свойство автоматически сбрасывается до значения **false**.</span><span class="sxs-lookup"><span data-stu-id="33466-119">After a password change, this property will be automatically reset to **false**.</span></span> <span data-ttu-id="33466-120">Если не установлено, по умолчанию используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="33466-120">If not set, default is **false**.</span></span> |
|<span data-ttu-id="33466-121">password</span><span class="sxs-lookup"><span data-stu-id="33466-121">password</span></span>|<span data-ttu-id="33466-122">Строка</span><span class="sxs-lookup"><span data-stu-id="33466-122">String</span></span>|<span data-ttu-id="33466-p104">Пароль пользователя. Это свойство обязательно указывать при создании пользователя. Его можно обновить, но пользователю потребуется изменить пароль при следующем входе. Пароль должен соответствовать минимальным требованиям, указанным в свойстве **passwordPolicies** пользователя. По умолчанию требуется надежный пароль.</span><span class="sxs-lookup"><span data-stu-id="33466-p104">The password for the user. This property is required when a user is created. It can be updated, but the user will be required to change the password on the next login. The password must satisfy minimum requirements as specified by the user’s **passwordPolicies** property. By default, a strong password is required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="33466-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="33466-128">JSON representation</span></span>

<span data-ttu-id="33466-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="33466-129">Here is a JSON representation of the resource</span></span>

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

