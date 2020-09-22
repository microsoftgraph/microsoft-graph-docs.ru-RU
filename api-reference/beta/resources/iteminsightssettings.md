---
title: Тип ресурса Итеминсигхтссеттингс
description: Представляет параметры конфиденциальности для Итеминсигхтс.
localization_priority: Normal
author: simonhult
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 5d05a9fdf3a901fcddd55207bec373a3a0736afa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48089331"
---
# <a name="iteminsightssettings-resource-type"></a><span data-ttu-id="4598a-103">Тип ресурса Итеминсигхтссеттингс</span><span class="sxs-lookup"><span data-stu-id="4598a-103">itemInsightsSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4598a-104">Представляет параметры конфиденциальности для [итеминсигхтс](iteminsights.md), которые настраивают видимость аналитических данных, полученных от Microsoft Graph, между пользователями и другими элементами (например, документами или сайтами) в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="4598a-104">Represents privacy settings for [itemInsights](iteminsights.md), which configure the visibility of insights derived from Microsoft Graph, between users and other items (such as documents or sites) in Microsoft 365.</span></span>

## <a name="methods"></a><span data-ttu-id="4598a-105">Методы</span><span class="sxs-lookup"><span data-stu-id="4598a-105">Methods</span></span>

| <span data-ttu-id="4598a-106">Метод</span><span class="sxs-lookup"><span data-stu-id="4598a-106">Method</span></span>       | <span data-ttu-id="4598a-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4598a-107">Return Type</span></span> | <span data-ttu-id="4598a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="4598a-108">Description</span></span> |
|:-------------------------------------------------------------|:----------------------------------------------|:-----------------------------------------------------------------|
| [<span data-ttu-id="4598a-109">Получение</span><span class="sxs-lookup"><span data-stu-id="4598a-109">Get</span></span>](../api/iteminsightssettings-get.md)| [<span data-ttu-id="4598a-110">итеминсигхтссеттингс</span><span class="sxs-lookup"><span data-stu-id="4598a-110">itemInsightsSettings</span></span>](iteminsightssettings.md) | <span data-ttu-id="4598a-111">Чтение свойств объекта **итеминсигхтссеттингс** .</span><span class="sxs-lookup"><span data-stu-id="4598a-111">Read the properties of an **itemInsightsSettings** object.</span></span> |
| [<span data-ttu-id="4598a-112">Обновление</span><span class="sxs-lookup"><span data-stu-id="4598a-112">Update</span></span>](../api/iteminsightssettings-update.md)| [<span data-ttu-id="4598a-113">итеминсигхтссеттингс</span><span class="sxs-lookup"><span data-stu-id="4598a-113">itemInsightsSettings</span></span>](iteminsightssettings.md) | <span data-ttu-id="4598a-114">Обновление объекта **итеминсигхтссеттингс** .</span><span class="sxs-lookup"><span data-stu-id="4598a-114">Update an **itemInsightsSettings** object.</span></span>|


## <a name="properties"></a><span data-ttu-id="4598a-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="4598a-115">Properties</span></span>
| <span data-ttu-id="4598a-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="4598a-116">Property</span></span>   | <span data-ttu-id="4598a-117">Тип</span><span class="sxs-lookup"><span data-stu-id="4598a-117">Type</span></span>|<span data-ttu-id="4598a-118">Описание</span><span class="sxs-lookup"><span data-stu-id="4598a-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4598a-119">isEnabledInOrganization</span><span class="sxs-lookup"><span data-stu-id="4598a-119">isEnabledInOrganization</span></span>|<span data-ttu-id="4598a-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="4598a-120">Boolean</span></span>| <span data-ttu-id="4598a-121">`true` , если аналитика элемента организации включена; `false` Если аналитика элемента Организации отключена для всех пользователей без исключений.</span><span class="sxs-lookup"><span data-stu-id="4598a-121">`true` if organization item insights are enabled; `false` if organization item insights are disabled for all users without exceptions.</span></span> <span data-ttu-id="4598a-122">Значение по умолчанию: `true`.</span><span class="sxs-lookup"><span data-stu-id="4598a-122">Default is `true`.</span></span> <span data-ttu-id="4598a-123">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="4598a-123">Optional.</span></span>|
|<span data-ttu-id="4598a-124">disabledForGroup</span><span class="sxs-lookup"><span data-stu-id="4598a-124">disabledForGroup</span></span>|<span data-ttu-id="4598a-125">Строка</span><span class="sxs-lookup"><span data-stu-id="4598a-125">String</span></span>| <span data-ttu-id="4598a-126">Идентификатор группы Azure AD, для которой отключается аналитика элемента "участники".</span><span class="sxs-lookup"><span data-stu-id="4598a-126">The ID of an Azure AD group, of which the members' item insights are disabled.</span></span> <span data-ttu-id="4598a-127">Значение по умолчанию: `empty`.</span><span class="sxs-lookup"><span data-stu-id="4598a-127">Default is `empty`.</span></span> <span data-ttu-id="4598a-128">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="4598a-128">Optional.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4598a-129">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4598a-129">JSON representation</span></span>

<span data-ttu-id="4598a-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4598a-130">Here is a JSON representation of the resource</span></span>
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


