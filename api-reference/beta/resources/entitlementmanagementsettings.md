---
title: тип ресурса entitlementManagementSettings
description: Представляет параметры для управления правами Azure AD для всех клиентов.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d34a04d0f8eb3bdff16befd43870b75d473a8d0c
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2021
ms.locfileid: "53350980"
---
# <a name="entitlementmanagementsettings-resource-type"></a><span data-ttu-id="85351-103">тип ресурса entitlementManagementSettings</span><span class="sxs-lookup"><span data-stu-id="85351-103">entitlementManagementSettings resource type</span></span>

<span data-ttu-id="85351-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85351-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85351-105">Представляет параметры, которые контролируют поведение управления правами [Azure AD.](entitlementmanagement-root.md)</span><span class="sxs-lookup"><span data-stu-id="85351-105">Represents settings that control the behavior of [Azure AD entitlement management](entitlementmanagement-root.md).</span></span>  <span data-ttu-id="85351-106">Этот ресурс не включает параметр создателей каталога; чтобы просмотреть или изменить членство создателей каталога в роли, используйте [API](unifiedroleassignment.md) назначений ролей с поставщиком RBAC управления правами.</span><span class="sxs-lookup"><span data-stu-id="85351-106">This resource does not include the catalog creators setting; to view or change the catalog creators role membership, use the [role assignments](unifiedroleassignment.md) API with the entitlement management RBAC provider.</span></span>

## <a name="methods"></a><span data-ttu-id="85351-107">Методы</span><span class="sxs-lookup"><span data-stu-id="85351-107">Methods</span></span>

| <span data-ttu-id="85351-108">Метод</span><span class="sxs-lookup"><span data-stu-id="85351-108">Method</span></span>       | <span data-ttu-id="85351-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="85351-109">Return Type</span></span> | <span data-ttu-id="85351-110">Описание</span><span class="sxs-lookup"><span data-stu-id="85351-110">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="85351-111">[получение](../api/entitlementmanagementsettings-get.md);</span><span class="sxs-lookup"><span data-stu-id="85351-111">[Get](../api/entitlementmanagementsettings-get.md)</span></span> | [<span data-ttu-id="85351-112">entitlementManagementSettings</span><span class="sxs-lookup"><span data-stu-id="85351-112">entitlementManagementSettings</span></span>](entitlementmanagementsettings.md) | <span data-ttu-id="85351-113">Ознакомьтесь с свойствами объекта **entitlementManagementSettings.**</span><span class="sxs-lookup"><span data-stu-id="85351-113">Read the properties of an **entitlementManagementSettings** object.</span></span> |
| [<span data-ttu-id="85351-114">Обновление</span><span class="sxs-lookup"><span data-stu-id="85351-114">Update</span></span>](../api/entitlementmanagementsettings-update.md) | [<span data-ttu-id="85351-115">entitlementManagementSettings</span><span class="sxs-lookup"><span data-stu-id="85351-115">entitlementManagementSettings</span></span>](entitlementmanagementsettings.md) | <span data-ttu-id="85351-116">Обновление свойств объекта **entitlementManagementSettings.**</span><span class="sxs-lookup"><span data-stu-id="85351-116">Update the properties of an **entitlementManagementSettings** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="85351-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="85351-117">Properties</span></span>

| <span data-ttu-id="85351-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="85351-118">Property</span></span>     | <span data-ttu-id="85351-119">Тип</span><span class="sxs-lookup"><span data-stu-id="85351-119">Type</span></span>        | <span data-ttu-id="85351-120">Описание</span><span class="sxs-lookup"><span data-stu-id="85351-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="85351-121">externalUserLifecycleAction</span><span class="sxs-lookup"><span data-stu-id="85351-121">externalUserLifecycleAction</span></span>|<span data-ttu-id="85351-122">Строка</span><span class="sxs-lookup"><span data-stu-id="85351-122">String</span></span>|<span data-ttu-id="85351-123">Один `None` из `BlockSignIn` , или `BlockSignInAndDelete` .</span><span class="sxs-lookup"><span data-stu-id="85351-123">One of `None`, `BlockSignIn`, or `BlockSignInAndDelete`.</span></span> |
|<span data-ttu-id="85351-124">daysUntilExternalUserDeletedAfterBlocked</span><span class="sxs-lookup"><span data-stu-id="85351-124">daysUntilExternalUserDeletedAfterBlocked</span></span>|<span data-ttu-id="85351-125">Int64</span><span class="sxs-lookup"><span data-stu-id="85351-125">Int64</span></span>|<span data-ttu-id="85351-126">Если **externalUserLifecycleAction** — количество дней после блокировки внешнего пользователя до удаления `BlockSignInAndDelete` учетной записи.</span><span class="sxs-lookup"><span data-stu-id="85351-126">If **externalUserLifecycleAction** is `BlockSignInAndDelete`, the number of days after an external user is blocked from sign in before their account is deleted.</span></span>|

## <a name="relationships"></a><span data-ttu-id="85351-127">Связи</span><span class="sxs-lookup"><span data-stu-id="85351-127">Relationships</span></span>

<span data-ttu-id="85351-128">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="85351-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="85351-129">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="85351-129">JSON representation</span></span>

<span data-ttu-id="85351-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="85351-130">The following is a JSON representation of the resource.</span></span>

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


