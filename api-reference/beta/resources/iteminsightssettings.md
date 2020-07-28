---
title: Тип ресурса Итеминсигхтссеттингс
description: Представляет параметры конфиденциальности для Итеминсигхтс.
localization_priority: Normal
author: simonhult
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 3be5fa87fd6c2623126437fccb1ea43b7bc275f2
ms.sourcegitcommit: 20b951f8bd245bb3a2bc7d3f5533e8619e9db084
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/27/2020
ms.locfileid: "45427550"
---
# <a name="iteminsightssettings-resource-type"></a><span data-ttu-id="22b2b-103">Тип ресурса Итеминсигхтссеттингс</span><span class="sxs-lookup"><span data-stu-id="22b2b-103">itemInsightsSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22b2b-104">Представляет параметры конфиденциальности для [итеминсигхтс](iteminsights.md), которые настраивают видимость аналитических данных, полученных от Microsoft Graph, между пользователями и другими элементами (например, документами или сайтами) в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="22b2b-104">Represents privacy settings for [itemInsights](iteminsights.md), which configure the visibility of insights derived from Microsoft Graph, between users and other items (such as documents or sites) in Microsoft 365.</span></span>

## <a name="methods"></a><span data-ttu-id="22b2b-105">Методы</span><span class="sxs-lookup"><span data-stu-id="22b2b-105">Methods</span></span>

| <span data-ttu-id="22b2b-106">Метод</span><span class="sxs-lookup"><span data-stu-id="22b2b-106">Method</span></span>       | <span data-ttu-id="22b2b-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="22b2b-107">Return Type</span></span> | <span data-ttu-id="22b2b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="22b2b-108">Description</span></span> |
|:-------------------------------------------------------------|:----------------------------------------------|:-----------------------------------------------------------------|
| <span data-ttu-id="22b2b-109">[получение](../api/iteminsightssettings-get.md);</span><span class="sxs-lookup"><span data-stu-id="22b2b-109">[Get](../api/iteminsightssettings-get.md)</span></span>| [<span data-ttu-id="22b2b-110">итеминсигхтссеттингс</span><span class="sxs-lookup"><span data-stu-id="22b2b-110">itemInsightsSettings</span></span>](iteminsightssettings.md) | <span data-ttu-id="22b2b-111">Чтение свойств объекта **итеминсигхтссеттингс** .</span><span class="sxs-lookup"><span data-stu-id="22b2b-111">Read the properties of an **itemInsightsSettings** object.</span></span> |
| <span data-ttu-id="22b2b-112">[обновление](../api/iteminsightssettings-update.md).</span><span class="sxs-lookup"><span data-stu-id="22b2b-112">[Update](../api/iteminsightssettings-update.md)</span></span>| [<span data-ttu-id="22b2b-113">итеминсигхтссеттингс</span><span class="sxs-lookup"><span data-stu-id="22b2b-113">itemInsightsSettings</span></span>](iteminsightssettings.md) | <span data-ttu-id="22b2b-114">Обновление объекта **итеминсигхтссеттингс** .</span><span class="sxs-lookup"><span data-stu-id="22b2b-114">Update an **itemInsightsSettings** object.</span></span>|


## <a name="properties"></a><span data-ttu-id="22b2b-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="22b2b-115">Properties</span></span>
| <span data-ttu-id="22b2b-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="22b2b-116">Property</span></span>   | <span data-ttu-id="22b2b-117">Тип</span><span class="sxs-lookup"><span data-stu-id="22b2b-117">Type</span></span>|<span data-ttu-id="22b2b-118">Описание</span><span class="sxs-lookup"><span data-stu-id="22b2b-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="22b2b-119">исенаблединорганизатион</span><span class="sxs-lookup"><span data-stu-id="22b2b-119">isEnabledInOrganization</span></span>|<span data-ttu-id="22b2b-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="22b2b-120">Boolean</span></span>| <span data-ttu-id="22b2b-121">`true`, если аналитика элемента организации включена; `false`Если аналитика элемента Организации отключена для всех пользователей без исключений.</span><span class="sxs-lookup"><span data-stu-id="22b2b-121">`true` if organization item insights are enabled; `false` if organization item insights are disabled for all users without exceptions.</span></span> <span data-ttu-id="22b2b-122">Значение по умолчанию: `true`.</span><span class="sxs-lookup"><span data-stu-id="22b2b-122">Default is `true`.</span></span> <span data-ttu-id="22b2b-123">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="22b2b-123">Optional.</span></span>|
|<span data-ttu-id="22b2b-124">дисабледфорграуп</span><span class="sxs-lookup"><span data-stu-id="22b2b-124">disabledForGroup</span></span>|<span data-ttu-id="22b2b-125">String</span><span class="sxs-lookup"><span data-stu-id="22b2b-125">String</span></span>| <span data-ttu-id="22b2b-126">Идентификатор группы Azure AD, для которой отключается аналитика элемента "участники".</span><span class="sxs-lookup"><span data-stu-id="22b2b-126">The ID of an Azure AD group, of which the members' item insights are disabled.</span></span> <span data-ttu-id="22b2b-127">Значение по умолчанию: `empty`.</span><span class="sxs-lookup"><span data-stu-id="22b2b-127">Default is `empty`.</span></span> <span data-ttu-id="22b2b-128">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="22b2b-128">Optional.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="22b2b-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="22b2b-129">JSON representation</span></span>

<span data-ttu-id="22b2b-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="22b2b-130">Here is a JSON representation of the resource</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.itemInsightsSettings"
}-->

```json
{
  "isEnabledInOrganization": "Boolean",
  "disabledForGroup": "String"
}
```
