---
title: Тип ресурса passwordProfile
description: Содержит профиль пароля, связанный с пользователем. Свойство **passwordProfile** объекта user является объектом **passwordProfile**.
ms.openlocfilehash: ee933b75b3dc536cbfcb33502cdda0d63680174c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027164"
---
# <a name="passwordprofile-resource-type"></a><span data-ttu-id="c914a-104">Тип ресурса passwordProfile</span><span class="sxs-lookup"><span data-stu-id="c914a-104">passwordProfile resource type</span></span>

<span data-ttu-id="c914a-p102">Содержит профиль пароля, связанный с пользователем. Свойство **passwordProfile** объекта [user](user.md) является объектом **passwordProfile**.</span><span class="sxs-lookup"><span data-stu-id="c914a-p102">Contains the password profile associated with a user. The **passwordProfile** property of the [user](user.md) entity is a **passwordProfile** object.</span></span>


## <a name="properties"></a><span data-ttu-id="c914a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c914a-107">Properties</span></span>
| <span data-ttu-id="c914a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c914a-108">Property</span></span>     | <span data-ttu-id="c914a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c914a-109">Type</span></span>   |<span data-ttu-id="c914a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c914a-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c914a-111">forceChangePasswordNextSignIn</span><span class="sxs-lookup"><span data-stu-id="c914a-111">forceChangePasswordNextSignIn</span></span>|<span data-ttu-id="c914a-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="c914a-112">Boolean</span></span>| <span data-ttu-id="c914a-113">Значение **true** указывает, что пользователь должен изменить свой пароль при следующем входе. В противном случае используется значение **false**.</span><span class="sxs-lookup"><span data-stu-id="c914a-113">**true** if the user must change her password on the next login; otherwise **false**.</span></span> |
|<span data-ttu-id="c914a-114">password</span><span class="sxs-lookup"><span data-stu-id="c914a-114">password</span></span>|<span data-ttu-id="c914a-115">Строка</span><span class="sxs-lookup"><span data-stu-id="c914a-115">String</span></span>|<span data-ttu-id="c914a-p103">Пароль пользователя. Это свойство обязательно указывать при создании пользователя. Его можно обновить, но пользователю потребуется изменить пароль при следующем входе. Пароль должен соответствовать минимальным требованиям, указанным в свойстве **passwordPolicies** пользователя. По умолчанию требуется надежный пароль.</span><span class="sxs-lookup"><span data-stu-id="c914a-p103">The password for the user. This property is required when a user is created. It can be updated, but the user will be required to change the password on the next login. The password must satisfy minimum requirements as specified by the user’s **passwordPolicies** property. By default, a strong password is required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c914a-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c914a-121">JSON representation</span></span>

<span data-ttu-id="c914a-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c914a-122">Here is a JSON representation of the resource</span></span>

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