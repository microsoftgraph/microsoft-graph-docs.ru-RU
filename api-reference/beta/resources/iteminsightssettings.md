---
title: тип ресурса itemInsightsSettings
description: Представляет параметры конфиденциальности для itemInsights.
localization_priority: Normal
author: simonhult
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 80ca42440bcf365e051d9fb25fbc088af8a7f4bb
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53108826"
---
# <a name="iteminsightssettings-resource-type"></a><span data-ttu-id="3ca42-103">тип ресурса itemInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="3ca42-103">itemInsightsSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ca42-104">Представляет параметры конфиденциальности [для itemInsights и](iteminsights.md) параметр конфиденциальности для анализа [часов собраний.](https://support.microsoft.com/en-us/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1)</span><span class="sxs-lookup"><span data-stu-id="3ca42-104">Represents privacy settings for [itemInsights](iteminsights.md) and privacy setting for [meeting hours insights](https://support.microsoft.com/en-us/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1) .</span></span> <span data-ttu-id="3ca42-105">Используйте этот API, чтобы отключить/включить вычисление и обзор информации о элементах и сведения о часах собраний.</span><span class="sxs-lookup"><span data-stu-id="3ca42-105">Use this API to disable/enable calculation and visibility of item insights and meeting hours insights.</span></span> 

- <span data-ttu-id="3ca42-106">Сведения о элементах. Вычисляется связь между пользователями и элементами, такими как документы или сайты в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="3ca42-106">Item insights: Calculates relationship between users and items such as documents or sites in Microsoft 365.</span></span>  
- <span data-ttu-id="3ca42-107">Сведения о часах собраний: вычисляет часы собраний календаря на основе действий в Word, Excel, PowerPoint, электронной почте и Outlook в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="3ca42-107">Meeting hours insights: Calculates a person's calendar meeting hours based on activities in Word, Excel, PowerPoint, email, and Outlook calendar in Microsoft 365.</span></span>

<span data-ttu-id="3ca42-108">Используйте [ресурс userInsightsSettings,](userinsightssettings.md) чтобы отключить и включить вычисления и видимость озарения элементов и сведения о часах собраний пользователя.</span><span class="sxs-lookup"><span data-stu-id="3ca42-108">Use the [userInsightsSettings](userinsightssettings.md) resource to disable/enable calculation and visibility of item insights and meeting hours insights of a user.</span></span>

## <a name="methods"></a><span data-ttu-id="3ca42-109">Методы</span><span class="sxs-lookup"><span data-stu-id="3ca42-109">Methods</span></span>

| <span data-ttu-id="3ca42-110">Метод</span><span class="sxs-lookup"><span data-stu-id="3ca42-110">Method</span></span>       | <span data-ttu-id="3ca42-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3ca42-111">Return Type</span></span> | <span data-ttu-id="3ca42-112">Описание</span><span class="sxs-lookup"><span data-stu-id="3ca42-112">Description</span></span> |
|:-------------------------------------------------------------|:----------------------------------------------|:-----------------------------------------------------------------|
| <span data-ttu-id="3ca42-113">[получение](../api/iteminsightssettings-get.md);</span><span class="sxs-lookup"><span data-stu-id="3ca42-113">[Get](../api/iteminsightssettings-get.md)</span></span>| [<span data-ttu-id="3ca42-114">itemInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="3ca42-114">itemInsightsSettings</span></span>](iteminsightssettings.md) | <span data-ttu-id="3ca42-115">Ознакомьтесь с свойствами **объекта itemInsightsSettings.**</span><span class="sxs-lookup"><span data-stu-id="3ca42-115">Read the properties of an **itemInsightsSettings** object.</span></span> |
| [<span data-ttu-id="3ca42-116">Обновление</span><span class="sxs-lookup"><span data-stu-id="3ca42-116">Update</span></span>](../api/iteminsightssettings-update.md)| [<span data-ttu-id="3ca42-117">itemInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="3ca42-117">itemInsightsSettings</span></span>](iteminsightssettings.md) | <span data-ttu-id="3ca42-118">Обновление **объекта itemInsightsSettings.**</span><span class="sxs-lookup"><span data-stu-id="3ca42-118">Update an **itemInsightsSettings** object.</span></span>|


## <a name="properties"></a><span data-ttu-id="3ca42-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="3ca42-119">Properties</span></span>
| <span data-ttu-id="3ca42-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="3ca42-120">Property</span></span>   | <span data-ttu-id="3ca42-121">Тип</span><span class="sxs-lookup"><span data-stu-id="3ca42-121">Type</span></span>|<span data-ttu-id="3ca42-122">Описание</span><span class="sxs-lookup"><span data-stu-id="3ca42-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3ca42-123">isEnabledInOrganization</span><span class="sxs-lookup"><span data-stu-id="3ca42-123">isEnabledInOrganization</span></span>|<span data-ttu-id="3ca42-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="3ca42-124">Boolean</span></span>| <span data-ttu-id="3ca42-125">`true` если включена информация о элементах организации; `false` если сведения о элементах организации отключены для всех пользователей без исключений.</span><span class="sxs-lookup"><span data-stu-id="3ca42-125">`true` if organization item insights are enabled; `false` if organization item insights are disabled for all users without exceptions.</span></span> <span data-ttu-id="3ca42-126">Значение по умолчанию: `true`.</span><span class="sxs-lookup"><span data-stu-id="3ca42-126">Default is `true`.</span></span> <span data-ttu-id="3ca42-127">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="3ca42-127">Optional.</span></span>|
|<span data-ttu-id="3ca42-128">disabledForGroup</span><span class="sxs-lookup"><span data-stu-id="3ca42-128">disabledForGroup</span></span>|<span data-ttu-id="3ca42-129">Строка</span><span class="sxs-lookup"><span data-stu-id="3ca42-129">String</span></span>| <span data-ttu-id="3ca42-130">ID группы Azure AD, из которой отключены сведения о элементах участников.</span><span class="sxs-lookup"><span data-stu-id="3ca42-130">The ID of an Azure AD group, of which the members' item insights are disabled.</span></span> <span data-ttu-id="3ca42-131">Значение по умолчанию: `empty`.</span><span class="sxs-lookup"><span data-stu-id="3ca42-131">Default is `empty`.</span></span> <span data-ttu-id="3ca42-132">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="3ca42-132">Optional.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3ca42-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3ca42-133">JSON representation</span></span>

<span data-ttu-id="3ca42-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3ca42-134">Here is a JSON representation of the resource</span></span>
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


