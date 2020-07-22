---
title: Тип ресурса Ентитлементманажементсеттингс
description: Представляет параметры на уровне клиента для управления обслуживанием Azure AD.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b183466b102b480913c3841585ea3349e7ac2386
ms.sourcegitcommit: 0545b031585e605dc3a0fde481015f51f79819c4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/22/2020
ms.locfileid: "45225091"
---
# <a name="entitlementmanagementsettings-resource-type"></a><span data-ttu-id="d30a4-103">Тип ресурса Ентитлементманажементсеттингс</span><span class="sxs-lookup"><span data-stu-id="d30a4-103">entitlementManagementSettings resource type</span></span>

<span data-ttu-id="d30a4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d30a4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d30a4-105">Представляет параметры, управляющие поведением [управления обслуживанием Azure AD](entitlementmanagement-root.md).</span><span class="sxs-lookup"><span data-stu-id="d30a4-105">Represents settings that control the behavior of [Azure AD entitlement management](entitlementmanagement-root.md).</span></span>

## <a name="methods"></a><span data-ttu-id="d30a4-106">Методы</span><span class="sxs-lookup"><span data-stu-id="d30a4-106">Methods</span></span>

| <span data-ttu-id="d30a4-107">Метод</span><span class="sxs-lookup"><span data-stu-id="d30a4-107">Method</span></span>       | <span data-ttu-id="d30a4-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d30a4-108">Return Type</span></span> | <span data-ttu-id="d30a4-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d30a4-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="d30a4-110">[получение](../api/entitlementmanagementsettings-get.md);</span><span class="sxs-lookup"><span data-stu-id="d30a4-110">[Get](../api/entitlementmanagementsettings-get.md)</span></span> | [<span data-ttu-id="d30a4-111">ентитлементманажементсеттингс</span><span class="sxs-lookup"><span data-stu-id="d30a4-111">entitlementManagementSettings</span></span>](entitlementmanagementsettings.md) | <span data-ttu-id="d30a4-112">Чтение свойств объекта **ентитлементманажементсеттингс** .</span><span class="sxs-lookup"><span data-stu-id="d30a4-112">Read the properties of an **entitlementManagementSettings** object.</span></span> |
| <span data-ttu-id="d30a4-113">[обновление](../api/entitlementmanagementsettings-update.md).</span><span class="sxs-lookup"><span data-stu-id="d30a4-113">[Update](../api/entitlementmanagementsettings-update.md)</span></span> | [<span data-ttu-id="d30a4-114">ентитлементманажементсеттингс</span><span class="sxs-lookup"><span data-stu-id="d30a4-114">entitlementManagementSettings</span></span>](entitlementmanagementsettings.md) | <span data-ttu-id="d30a4-115">Обновление свойств объекта **ентитлементманажементсеттингс** .</span><span class="sxs-lookup"><span data-stu-id="d30a4-115">Update the properties of an **entitlementManagementSettings** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d30a4-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="d30a4-116">Properties</span></span>

| <span data-ttu-id="d30a4-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="d30a4-117">Property</span></span>     | <span data-ttu-id="d30a4-118">Тип</span><span class="sxs-lookup"><span data-stu-id="d30a4-118">Type</span></span>        | <span data-ttu-id="d30a4-119">Описание</span><span class="sxs-lookup"><span data-stu-id="d30a4-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d30a4-120">екстерналусерлифециклеактион</span><span class="sxs-lookup"><span data-stu-id="d30a4-120">externalUserLifecycleAction</span></span>|<span data-ttu-id="d30a4-121">Строка</span><span class="sxs-lookup"><span data-stu-id="d30a4-121">String</span></span>|<span data-ttu-id="d30a4-122">Один из `None` , `BlockSignIn` или `BlockSignInAndDelete` .</span><span class="sxs-lookup"><span data-stu-id="d30a4-122">One of `None`, `BlockSignIn`, or `BlockSignInAndDelete`.</span></span> |
|<span data-ttu-id="d30a4-123">дайсунтилекстерналусерделетедафтерблоккед</span><span class="sxs-lookup"><span data-stu-id="d30a4-123">daysUntilExternalUserDeletedAfterBlocked</span></span>|<span data-ttu-id="d30a4-124">Int64</span><span class="sxs-lookup"><span data-stu-id="d30a4-124">Int64</span></span>|<span data-ttu-id="d30a4-125">Если `externalUserLifecycleAction` задано `BlockSignInAndDelete` , то количество дней после блокирования входа от внешнего пользователя до удаления учетной записи.</span><span class="sxs-lookup"><span data-stu-id="d30a4-125">If `externalUserLifecycleAction` is `BlockSignInAndDelete`, the number of days after an external user is blocked from sign in before their account is deleted.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d30a4-126">Связи</span><span class="sxs-lookup"><span data-stu-id="d30a4-126">Relationships</span></span>

<span data-ttu-id="d30a4-127">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d30a4-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d30a4-128">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d30a4-128">JSON representation</span></span>

<span data-ttu-id="d30a4-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d30a4-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.entitlementManagementSettings",
  "baseType": "",
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
