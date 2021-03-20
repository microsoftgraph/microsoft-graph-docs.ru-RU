---
title: тип ресурса entitlementManagementSettings
description: Представляет параметры для управления правами Azure AD для всех клиентов.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 1b6138bc52e5686af94a94cfa13762b71a6242c4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945692"
---
# <a name="entitlementmanagementsettings-resource-type"></a><span data-ttu-id="6538b-103">тип ресурса entitlementManagementSettings</span><span class="sxs-lookup"><span data-stu-id="6538b-103">entitlementManagementSettings resource type</span></span>

<span data-ttu-id="6538b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6538b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6538b-105">Представляет параметры, которые контролируют поведение управления правами [Azure AD.](entitlementmanagement-root.md)</span><span class="sxs-lookup"><span data-stu-id="6538b-105">Represents settings that control the behavior of [Azure AD entitlement management](entitlementmanagement-root.md).</span></span>

## <a name="methods"></a><span data-ttu-id="6538b-106">Методы</span><span class="sxs-lookup"><span data-stu-id="6538b-106">Methods</span></span>

| <span data-ttu-id="6538b-107">Метод</span><span class="sxs-lookup"><span data-stu-id="6538b-107">Method</span></span>       | <span data-ttu-id="6538b-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6538b-108">Return Type</span></span> | <span data-ttu-id="6538b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6538b-109">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="6538b-110">[получение](../api/entitlementmanagementsettings-get.md);</span><span class="sxs-lookup"><span data-stu-id="6538b-110">[Get](../api/entitlementmanagementsettings-get.md)</span></span> | [<span data-ttu-id="6538b-111">entitlementManagementSettings</span><span class="sxs-lookup"><span data-stu-id="6538b-111">entitlementManagementSettings</span></span>](entitlementmanagementsettings.md) | <span data-ttu-id="6538b-112">Ознакомьтесь с свойствами объекта **entitlementManagementSettings.**</span><span class="sxs-lookup"><span data-stu-id="6538b-112">Read the properties of an **entitlementManagementSettings** object.</span></span> |
| [<span data-ttu-id="6538b-113">Обновление</span><span class="sxs-lookup"><span data-stu-id="6538b-113">Update</span></span>](../api/entitlementmanagementsettings-update.md) | [<span data-ttu-id="6538b-114">entitlementManagementSettings</span><span class="sxs-lookup"><span data-stu-id="6538b-114">entitlementManagementSettings</span></span>](entitlementmanagementsettings.md) | <span data-ttu-id="6538b-115">Обновление свойств объекта **entitlementManagementSettings.**</span><span class="sxs-lookup"><span data-stu-id="6538b-115">Update the properties of an **entitlementManagementSettings** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="6538b-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="6538b-116">Properties</span></span>

| <span data-ttu-id="6538b-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="6538b-117">Property</span></span>     | <span data-ttu-id="6538b-118">Тип</span><span class="sxs-lookup"><span data-stu-id="6538b-118">Type</span></span>        | <span data-ttu-id="6538b-119">Описание</span><span class="sxs-lookup"><span data-stu-id="6538b-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6538b-120">externalUserLifecycleAction</span><span class="sxs-lookup"><span data-stu-id="6538b-120">externalUserLifecycleAction</span></span>|<span data-ttu-id="6538b-121">Строка</span><span class="sxs-lookup"><span data-stu-id="6538b-121">String</span></span>|<span data-ttu-id="6538b-122">Один `None` из `BlockSignIn` , или `BlockSignInAndDelete` .</span><span class="sxs-lookup"><span data-stu-id="6538b-122">One of `None`, `BlockSignIn`, or `BlockSignInAndDelete`.</span></span> |
|<span data-ttu-id="6538b-123">daysUntilExternalUserDeletedAfterBlocked</span><span class="sxs-lookup"><span data-stu-id="6538b-123">daysUntilExternalUserDeletedAfterBlocked</span></span>|<span data-ttu-id="6538b-124">Int64</span><span class="sxs-lookup"><span data-stu-id="6538b-124">Int64</span></span>|<span data-ttu-id="6538b-125">Если **externalUserLifecycleAction** — количество дней после блокировки внешнего пользователя до удаления `BlockSignInAndDelete` учетной записи.</span><span class="sxs-lookup"><span data-stu-id="6538b-125">If **externalUserLifecycleAction** is `BlockSignInAndDelete`, the number of days after an external user is blocked from sign in before their account is deleted.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6538b-126">Связи</span><span class="sxs-lookup"><span data-stu-id="6538b-126">Relationships</span></span>

<span data-ttu-id="6538b-127">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="6538b-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6538b-128">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="6538b-128">JSON representation</span></span>

<span data-ttu-id="6538b-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6538b-129">The following is a JSON representation of the resource.</span></span>

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


