---
title: Тип ресурса Итеминсигхтссеттингс
description: Представляет параметры конфиденциальности для Итеминсигхтс.
localization_priority: Normal
author: simonhult
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: c84b2397c938997a3285d16612d090ae22444580
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522771"
---
# <a name="iteminsightssettings-resource-type"></a><span data-ttu-id="55b4d-103">Тип ресурса Итеминсигхтссеттингс</span><span class="sxs-lookup"><span data-stu-id="55b4d-103">itemInsightsSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55b4d-104">Представляет параметры конфиденциальности для [итеминсигхтс](iteminsights.md) и параметров конфиденциальности для отслеживания времени проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="55b4d-104">Represents privacy settings for [itemInsights](iteminsights.md) and privacy setting for meeting hours insights.</span></span> <span data-ttu-id="55b4d-105">Используйте этот API, чтобы отключить или включить вычисление и видимость данных об объеме и времени собраний.</span><span class="sxs-lookup"><span data-stu-id="55b4d-105">Use this API to disable/enable calculation and visibility of item insights and meeting hours insights.</span></span> 

- <span data-ttu-id="55b4d-106">Application Insights: вычисляет отношения между пользователями и элементами, такими как документы или сайты в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="55b4d-106">Item insights: Calculates relationship between users and items such as documents or sites in Microsoft 365.</span></span>  
- <span data-ttu-id="55b4d-107">Сведения о часах собраний: вычисляет время собрания в календаре пользователя на основе действий в Word, Excel, PowerPoint, электронной почте и календаре Outlook в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="55b4d-107">Meeting hours insights: Calculates a person's calendar meeting hours based on activities in Word, Excel, PowerPoint, email, and Outlook calendar in Microsoft 365.</span></span>

> [!NOTE]
> <span data-ttu-id="55b4d-108">Сведения о времени проведения собраний выходят на клиентов, начиная с ноября 2020.</span><span class="sxs-lookup"><span data-stu-id="55b4d-108">Meeting hours insights are rolling out to customers starting November 2020.</span></span> 

## <a name="methods"></a><span data-ttu-id="55b4d-109">Методы</span><span class="sxs-lookup"><span data-stu-id="55b4d-109">Methods</span></span>

| <span data-ttu-id="55b4d-110">Метод</span><span class="sxs-lookup"><span data-stu-id="55b4d-110">Method</span></span>       | <span data-ttu-id="55b4d-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="55b4d-111">Return Type</span></span> | <span data-ttu-id="55b4d-112">Описание</span><span class="sxs-lookup"><span data-stu-id="55b4d-112">Description</span></span> |
|:-------------------------------------------------------------|:----------------------------------------------|:-----------------------------------------------------------------|
| <span data-ttu-id="55b4d-113">[получение](../api/iteminsightssettings-get.md);</span><span class="sxs-lookup"><span data-stu-id="55b4d-113">[Get](../api/iteminsightssettings-get.md)</span></span>| [<span data-ttu-id="55b4d-114">итеминсигхтссеттингс</span><span class="sxs-lookup"><span data-stu-id="55b4d-114">itemInsightsSettings</span></span>](iteminsightssettings.md) | <span data-ttu-id="55b4d-115">Чтение свойств объекта **итеминсигхтссеттингс** .</span><span class="sxs-lookup"><span data-stu-id="55b4d-115">Read the properties of an **itemInsightsSettings** object.</span></span> |
| <span data-ttu-id="55b4d-116">[обновление](../api/iteminsightssettings-update.md).</span><span class="sxs-lookup"><span data-stu-id="55b4d-116">[Update](../api/iteminsightssettings-update.md)</span></span>| [<span data-ttu-id="55b4d-117">итеминсигхтссеттингс</span><span class="sxs-lookup"><span data-stu-id="55b4d-117">itemInsightsSettings</span></span>](iteminsightssettings.md) | <span data-ttu-id="55b4d-118">Обновление объекта **итеминсигхтссеттингс** .</span><span class="sxs-lookup"><span data-stu-id="55b4d-118">Update an **itemInsightsSettings** object.</span></span>|


## <a name="properties"></a><span data-ttu-id="55b4d-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="55b4d-119">Properties</span></span>
| <span data-ttu-id="55b4d-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="55b4d-120">Property</span></span>   | <span data-ttu-id="55b4d-121">Тип</span><span class="sxs-lookup"><span data-stu-id="55b4d-121">Type</span></span>|<span data-ttu-id="55b4d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="55b4d-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="55b4d-123">isEnabledInOrganization</span><span class="sxs-lookup"><span data-stu-id="55b4d-123">isEnabledInOrganization</span></span>|<span data-ttu-id="55b4d-124">Логический</span><span class="sxs-lookup"><span data-stu-id="55b4d-124">Boolean</span></span>| <span data-ttu-id="55b4d-125">`true` , если аналитика элемента организации включена; `false` Если аналитика элемента Организации отключена для всех пользователей без исключений.</span><span class="sxs-lookup"><span data-stu-id="55b4d-125">`true` if organization item insights are enabled; `false` if organization item insights are disabled for all users without exceptions.</span></span> <span data-ttu-id="55b4d-126">Значение по умолчанию: `true`.</span><span class="sxs-lookup"><span data-stu-id="55b4d-126">Default is `true`.</span></span> <span data-ttu-id="55b4d-127">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="55b4d-127">Optional.</span></span>|
|<span data-ttu-id="55b4d-128">disabledForGroup</span><span class="sxs-lookup"><span data-stu-id="55b4d-128">disabledForGroup</span></span>|<span data-ttu-id="55b4d-129">String</span><span class="sxs-lookup"><span data-stu-id="55b4d-129">String</span></span>| <span data-ttu-id="55b4d-130">Идентификатор группы Azure AD, для которой отключается аналитика элемента "участники".</span><span class="sxs-lookup"><span data-stu-id="55b4d-130">The ID of an Azure AD group, of which the members' item insights are disabled.</span></span> <span data-ttu-id="55b4d-131">Значение по умолчанию: `empty`.</span><span class="sxs-lookup"><span data-stu-id="55b4d-131">Default is `empty`.</span></span> <span data-ttu-id="55b4d-132">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="55b4d-132">Optional.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="55b4d-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="55b4d-133">JSON representation</span></span>

<span data-ttu-id="55b4d-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="55b4d-134">Here is a JSON representation of the resource</span></span>
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


