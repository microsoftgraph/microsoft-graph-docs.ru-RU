---
title: Тип ресурса entitlementManagementSettings
description: Представляет параметры для всего клиента для управления правами Azure AD.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9d5cc340837f173924802196bf12c9a63f26949a
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159124"
---
# <a name="entitlementmanagementsettings-resource-type"></a><span data-ttu-id="40f9a-103">Тип ресурса entitlementManagementSettings</span><span class="sxs-lookup"><span data-stu-id="40f9a-103">entitlementManagementSettings resource type</span></span>

<span data-ttu-id="40f9a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40f9a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40f9a-105">Представляет параметры, управляющие поведением управления [правами Azure AD.](entitlementmanagement-root.md)</span><span class="sxs-lookup"><span data-stu-id="40f9a-105">Represents settings that control the behavior of [Azure AD entitlement management](entitlementmanagement-root.md).</span></span>

## <a name="methods"></a><span data-ttu-id="40f9a-106">Методы</span><span class="sxs-lookup"><span data-stu-id="40f9a-106">Methods</span></span>

| <span data-ttu-id="40f9a-107">Метод</span><span class="sxs-lookup"><span data-stu-id="40f9a-107">Method</span></span>       | <span data-ttu-id="40f9a-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="40f9a-108">Return Type</span></span> | <span data-ttu-id="40f9a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="40f9a-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="40f9a-110">Получение</span><span class="sxs-lookup"><span data-stu-id="40f9a-110">Get</span></span>](../api/entitlementmanagementsettings-get.md) | [<span data-ttu-id="40f9a-111">entitlementManagementSettings</span><span class="sxs-lookup"><span data-stu-id="40f9a-111">entitlementManagementSettings</span></span>](entitlementmanagementsettings.md) | <span data-ttu-id="40f9a-112">Чтение свойств объекта **entitlementManagementSettings.**</span><span class="sxs-lookup"><span data-stu-id="40f9a-112">Read the properties of an **entitlementManagementSettings** object.</span></span> |
| [<span data-ttu-id="40f9a-113">Обновление</span><span class="sxs-lookup"><span data-stu-id="40f9a-113">Update</span></span>](../api/entitlementmanagementsettings-update.md) | [<span data-ttu-id="40f9a-114">entitlementManagementSettings</span><span class="sxs-lookup"><span data-stu-id="40f9a-114">entitlementManagementSettings</span></span>](entitlementmanagementsettings.md) | <span data-ttu-id="40f9a-115">Обновление свойств объекта **entitlementManagementSettings.**</span><span class="sxs-lookup"><span data-stu-id="40f9a-115">Update the properties of an **entitlementManagementSettings** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="40f9a-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="40f9a-116">Properties</span></span>

| <span data-ttu-id="40f9a-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="40f9a-117">Property</span></span>     | <span data-ttu-id="40f9a-118">Тип</span><span class="sxs-lookup"><span data-stu-id="40f9a-118">Type</span></span>        | <span data-ttu-id="40f9a-119">Описание</span><span class="sxs-lookup"><span data-stu-id="40f9a-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="40f9a-120">externalUserLifecycleAction</span><span class="sxs-lookup"><span data-stu-id="40f9a-120">externalUserLifecycleAction</span></span>|<span data-ttu-id="40f9a-121">String</span><span class="sxs-lookup"><span data-stu-id="40f9a-121">String</span></span>|<span data-ttu-id="40f9a-122">Один из `None` `BlockSignIn` , или `BlockSignInAndDelete` .</span><span class="sxs-lookup"><span data-stu-id="40f9a-122">One of `None`, `BlockSignIn`, or `BlockSignInAndDelete`.</span></span> |
|<span data-ttu-id="40f9a-123">daysUntilExternalUserDeletedAfterBlocked</span><span class="sxs-lookup"><span data-stu-id="40f9a-123">daysUntilExternalUserDeletedAfterBlocked</span></span>|<span data-ttu-id="40f9a-124">Int64</span><span class="sxs-lookup"><span data-stu-id="40f9a-124">Int64</span></span>|<span data-ttu-id="40f9a-125">Если это так, то количество дней после блокировки внешнего пользователя на вход до удаления его `externalUserLifecycleAction` `BlockSignInAndDelete` учетной записи.</span><span class="sxs-lookup"><span data-stu-id="40f9a-125">If `externalUserLifecycleAction` is `BlockSignInAndDelete`, the number of days after an external user is blocked from sign in before their account is deleted.</span></span>|

## <a name="relationships"></a><span data-ttu-id="40f9a-126">Связи</span><span class="sxs-lookup"><span data-stu-id="40f9a-126">Relationships</span></span>

<span data-ttu-id="40f9a-127">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="40f9a-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="40f9a-128">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="40f9a-128">JSON representation</span></span>

<span data-ttu-id="40f9a-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="40f9a-129">The following is a JSON representation of the resource.</span></span>

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


