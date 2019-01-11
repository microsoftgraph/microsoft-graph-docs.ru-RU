---
title: Тип ресурса passwordProfile
description: Содержит профиль пароля, связанный с пользователем. Свойство **passwordProfile** объекта user является объектом **passwordProfile**.
localization_priority: Priority
ms.openlocfilehash: 80d774906fb4897f57b943af827cfbc32e90511f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819665"
---
# <a name="passwordprofile-resource-type"></a><span data-ttu-id="d61e4-104">Тип ресурса passwordProfile</span><span class="sxs-lookup"><span data-stu-id="d61e4-104">passwordProfile resource type</span></span>

<span data-ttu-id="d61e4-p102">Содержит профиль пароля, связанный с пользователем. Свойство **passwordProfile** объекта [user](user.md) является объектом **passwordProfile**.</span><span class="sxs-lookup"><span data-stu-id="d61e4-p102">Contains the password profile associated with a user. The **passwordProfile** property of the [user](user.md) entity is a **passwordProfile** object.</span></span>


## <a name="properties"></a><span data-ttu-id="d61e4-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d61e4-107">Properties</span></span>
| <span data-ttu-id="d61e4-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d61e4-108">Property</span></span>     | <span data-ttu-id="d61e4-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d61e4-109">Type</span></span>   |<span data-ttu-id="d61e4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d61e4-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d61e4-111">forceChangePasswordNextSignIn</span><span class="sxs-lookup"><span data-stu-id="d61e4-111">forceChangePasswordNextSignIn</span></span>|<span data-ttu-id="d61e4-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="d61e4-112">Boolean</span></span>| <span data-ttu-id="d61e4-113">Значение **true** указывает, что пользователь должен изменить свой пароль при следующем входе. В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="d61e4-113">**true** if the user must change her password on the next login; otherwise **false**.</span></span> |
|<span data-ttu-id="d61e4-114">password</span><span class="sxs-lookup"><span data-stu-id="d61e4-114">password</span></span>|<span data-ttu-id="d61e4-115">Строка</span><span class="sxs-lookup"><span data-stu-id="d61e4-115">String</span></span>|<span data-ttu-id="d61e4-p103">Пароль пользователя. Это свойство обязательно указывать при создании пользователя. Его можно обновить, но пользователю потребуется изменить пароль при следующем входе. Пароль должен соответствовать минимальным требованиям, указанным в свойстве **passwordPolicies** пользователя. По умолчанию требуется надежный пароль.</span><span class="sxs-lookup"><span data-stu-id="d61e4-p103">The password for the user. This property is required when a user is created. It can be updated, but the user will be required to change the password on the next login. The password must satisfy minimum requirements as specified by the user’s **passwordPolicies** property. By default, a strong password is required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d61e4-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d61e4-121">JSON representation</span></span>

<span data-ttu-id="d61e4-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d61e4-122">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordProfile"
}-->

```json
{
  "forceChangePasswordNextSignIn": true,
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
