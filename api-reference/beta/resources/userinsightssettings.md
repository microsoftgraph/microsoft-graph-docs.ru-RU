---
title: тип ресурса userInsightsSettings
description: Представляет параметры конфиденциальности пользователей для анализа элементов и данных о часах собраний.
localization_priority: Normal
author: simonhult
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 5ecc9277d0bd98df99387a5dd222998074c6eb1b
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53109217"
---
# <a name="userinsightssettings-resource-type"></a><span data-ttu-id="e6956-103">тип ресурса userInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="e6956-103">userInsightsSettings resource type</span></span>

<span data-ttu-id="e6956-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6956-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6956-105">Представляет параметры конфиденциальности пользователей [для itemInsights](iteminsights.md) и [собраний.](https://support.microsoft.com/en-us/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1)</span><span class="sxs-lookup"><span data-stu-id="e6956-105">Represents user privacy settings for [itemInsights](iteminsights.md) and [meeting hours insights](https://support.microsoft.com/en-us/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1) .</span></span> <span data-ttu-id="e6956-106">Используйте этот ресурс, чтобы отключить/включить вычисления и видимость данных о элементах и сведения о часах собраний пользователя.</span><span class="sxs-lookup"><span data-stu-id="e6956-106">Use this resource to disable/enable calculation and visibility of item insights and meeting hours insights of a user.</span></span> 

- <span data-ttu-id="e6956-107">Сведения о элементах. Вычисляется связь между пользователями и элементами, такими как документы или сайты в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="e6956-107">Item insights: Calculates relationship between users and items such as documents or sites in Microsoft 365.</span></span>  
- <span data-ttu-id="e6956-108">Сведения о часах собраний: вычисляет часы собраний календаря на основе действий в Word, Excel, PowerPoint, электронной почте и Outlook в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="e6956-108">Meeting hours insights: Calculates a person's calendar meeting hours based on activities in Word, Excel, PowerPoint, email, and Outlook calendar in Microsoft 365.</span></span>

<span data-ttu-id="e6956-109">Используйте [ресурс itemInsightsSettings,](iteminsightssettings.md) чтобы отключить/включить вычисления и видимость анализа элементов и сведения о часах собраний на уровне организации.</span><span class="sxs-lookup"><span data-stu-id="e6956-109">Use the [itemInsightsSettings](iteminsightssettings.md) resource to disable/enable calculation and visibility of item insights and meeting hours insights at an organization level.</span></span>

## <a name="methods"></a><span data-ttu-id="e6956-110">Методы</span><span class="sxs-lookup"><span data-stu-id="e6956-110">Methods</span></span>

| <span data-ttu-id="e6956-111">Метод</span><span class="sxs-lookup"><span data-stu-id="e6956-111">Method</span></span>                                                 | <span data-ttu-id="e6956-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e6956-112">Return Type</span></span>                                                   | <span data-ttu-id="e6956-113">Описание</span><span class="sxs-lookup"><span data-stu-id="e6956-113">Description</span></span>                                                                                        |
|:-------------------------------------------------------|:--------------------------------------------------------------|:---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="e6956-114">[получение](../api/userinsightssettings-get.md);</span><span class="sxs-lookup"><span data-stu-id="e6956-114">[Get](../api/userinsightssettings-get.md)</span></span>       | [<span data-ttu-id="e6956-115">userInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="e6956-115">userInsightsSettings</span></span>](userinsightssettings.md) | <span data-ttu-id="e6956-116">Ознакомьтесь с свойствами **объекта userinsightsettings.**</span><span class="sxs-lookup"><span data-stu-id="e6956-116">Read the properties of a **userinsightssettings** object.</span></span>  |
| [<span data-ttu-id="e6956-117">Обновление</span><span class="sxs-lookup"><span data-stu-id="e6956-117">Update</span></span>](../api/userinsightssettings-update.md) | [<span data-ttu-id="e6956-118">userInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="e6956-118">userInsightsSettings</span></span>](userinsightssettings.md) | <span data-ttu-id="e6956-119">Обновление свойств объекта **userinsightsettings.**</span><span class="sxs-lookup"><span data-stu-id="e6956-119">Update the properties of a **userinsightssettings** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e6956-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="e6956-120">Properties</span></span>
| <span data-ttu-id="e6956-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="e6956-121">Property</span></span>                   | <span data-ttu-id="e6956-122">Тип</span><span class="sxs-lookup"><span data-stu-id="e6956-122">Type</span></span>                                                  | <span data-ttu-id="e6956-123">Описание</span><span class="sxs-lookup"><span data-stu-id="e6956-123">Description</span></span>                                                                                                                                                         |
|----------------------------|-------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="e6956-124">isEnabled</span><span class="sxs-lookup"><span data-stu-id="e6956-124">isEnabled</span></span>     | <span data-ttu-id="e6956-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6956-125">Boolean</span></span>  |  <span data-ttu-id="e6956-126">`true` если включены **сведения о элементах itemInsights и** часах собраний; `false` если сведения о **элементах itemInsights и** время собраний отключены.</span><span class="sxs-lookup"><span data-stu-id="e6956-126">`true` if user's **itemInsights** and meeting hours insights are enabled; `false` if user's **itemInsights** and meeting hours insights are disabled.</span></span> <span data-ttu-id="e6956-127">Значение по умолчанию: `true`.</span><span class="sxs-lookup"><span data-stu-id="e6956-127">Default is `true`.</span></span> <span data-ttu-id="e6956-128">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="e6956-128">Optional.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e6956-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e6956-129">JSON representation</span></span>

<span data-ttu-id="e6956-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e6956-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.userInsightsSettings"
}-->

```json
{
  "isEnabled": "Boolean"
}
```


