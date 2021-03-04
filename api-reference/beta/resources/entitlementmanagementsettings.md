---
title: тип ресурса entitlementManagementSettings
description: Представляет параметры для управления правами Azure AD для всех клиентов.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b4b6ee584e671e070955eb7c065c59cb8481c375
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440355"
---
# <a name="entitlementmanagementsettings-resource-type"></a><span data-ttu-id="b6565-103">тип ресурса entitlementManagementSettings</span><span class="sxs-lookup"><span data-stu-id="b6565-103">entitlementManagementSettings resource type</span></span>

<span data-ttu-id="b6565-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6565-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6565-105">Представляет параметры, которые контролируют поведение управления правами [Azure AD.](entitlementmanagement-root.md)</span><span class="sxs-lookup"><span data-stu-id="b6565-105">Represents settings that control the behavior of [Azure AD entitlement management](entitlementmanagement-root.md).</span></span>

## <a name="methods"></a><span data-ttu-id="b6565-106">Методы</span><span class="sxs-lookup"><span data-stu-id="b6565-106">Methods</span></span>

| <span data-ttu-id="b6565-107">Метод</span><span class="sxs-lookup"><span data-stu-id="b6565-107">Method</span></span>       | <span data-ttu-id="b6565-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b6565-108">Return Type</span></span> | <span data-ttu-id="b6565-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b6565-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="b6565-110">[получение](../api/entitlementmanagementsettings-get.md);</span><span class="sxs-lookup"><span data-stu-id="b6565-110">[Get](../api/entitlementmanagementsettings-get.md)</span></span> | [<span data-ttu-id="b6565-111">entitlementManagementSettings</span><span class="sxs-lookup"><span data-stu-id="b6565-111">entitlementManagementSettings</span></span>](entitlementmanagementsettings.md) | <span data-ttu-id="b6565-112">Ознакомьтесь с свойствами объекта **entitlementManagementSettings.**</span><span class="sxs-lookup"><span data-stu-id="b6565-112">Read the properties of an **entitlementManagementSettings** object.</span></span> |
| [<span data-ttu-id="b6565-113">Обновление</span><span class="sxs-lookup"><span data-stu-id="b6565-113">Update</span></span>](../api/entitlementmanagementsettings-update.md) | [<span data-ttu-id="b6565-114">entitlementManagementSettings</span><span class="sxs-lookup"><span data-stu-id="b6565-114">entitlementManagementSettings</span></span>](entitlementmanagementsettings.md) | <span data-ttu-id="b6565-115">Обновление свойств объекта **entitlementManagementSettings.**</span><span class="sxs-lookup"><span data-stu-id="b6565-115">Update the properties of an **entitlementManagementSettings** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b6565-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="b6565-116">Properties</span></span>

| <span data-ttu-id="b6565-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="b6565-117">Property</span></span>     | <span data-ttu-id="b6565-118">Тип</span><span class="sxs-lookup"><span data-stu-id="b6565-118">Type</span></span>        | <span data-ttu-id="b6565-119">Описание</span><span class="sxs-lookup"><span data-stu-id="b6565-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b6565-120">externalUserLifecycleAction</span><span class="sxs-lookup"><span data-stu-id="b6565-120">externalUserLifecycleAction</span></span>|<span data-ttu-id="b6565-121">String</span><span class="sxs-lookup"><span data-stu-id="b6565-121">String</span></span>|<span data-ttu-id="b6565-122">Один `None` из `BlockSignIn` , или `BlockSignInAndDelete` .</span><span class="sxs-lookup"><span data-stu-id="b6565-122">One of `None`, `BlockSignIn`, or `BlockSignInAndDelete`.</span></span> |
|<span data-ttu-id="b6565-123">daysUntilExternalUserDeletedAfterBlocked</span><span class="sxs-lookup"><span data-stu-id="b6565-123">daysUntilExternalUserDeletedAfterBlocked</span></span>|<span data-ttu-id="b6565-124">Int64</span><span class="sxs-lookup"><span data-stu-id="b6565-124">Int64</span></span>|<span data-ttu-id="b6565-125">Если это так, то количество дней после блокировки внешнего пользователя при входе до удаления `externalUserLifecycleAction` `BlockSignInAndDelete` учетной записи.</span><span class="sxs-lookup"><span data-stu-id="b6565-125">If `externalUserLifecycleAction` is `BlockSignInAndDelete`, the number of days after an external user is blocked from sign in before their account is deleted.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b6565-126">Связи</span><span class="sxs-lookup"><span data-stu-id="b6565-126">Relationships</span></span>

<span data-ttu-id="b6565-127">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b6565-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b6565-128">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b6565-128">JSON representation</span></span>

<span data-ttu-id="b6565-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b6565-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.entitlementManagementSettings",
  "keyProperty": ""
}-->

```json
{
  "externalUserLifecycleAction": "String",
  "daysUntilExternalUserDeletedAfterBlocked": 1
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "entitlementManagementSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


