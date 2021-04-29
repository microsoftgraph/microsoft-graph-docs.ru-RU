---
title: тип ресурса topicModelingSettings
description: Параметры моделирования тем для дела об обнаружении электронных данных
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: bd433de0aa88298961366f50425706e1af4bffde
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080878"
---
# <a name="topicmodelingsettings-resource-type"></a><span data-ttu-id="fe68a-103">тип ресурса topicModelingSettings</span><span class="sxs-lookup"><span data-stu-id="fe68a-103">topicModelingSettings resource type</span></span>

<span data-ttu-id="fe68a-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="fe68a-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe68a-105">Параметры моделирования тем (Темы) для дела об обнаружении электронных данных.</span><span class="sxs-lookup"><span data-stu-id="fe68a-105">Topic modeling (Themes) settings for an eDiscovery case.</span></span> <span data-ttu-id="fe68a-106">Дополнительные данные см. в [обзоре Настройка параметров](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery)поиска и аналитики в Advanced eDiscovery.</span><span class="sxs-lookup"><span data-stu-id="fe68a-106">To learn more, see [Configure search and analytics settings in Advanced eDiscovery](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery).</span></span>

## <a name="properties"></a><span data-ttu-id="fe68a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="fe68a-107">Properties</span></span>

|<span data-ttu-id="fe68a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="fe68a-108">Property</span></span>|<span data-ttu-id="fe68a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="fe68a-109">Type</span></span>|<span data-ttu-id="fe68a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="fe68a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe68a-111">dynamicallyAdjustTopicCount</span><span class="sxs-lookup"><span data-stu-id="fe68a-111">dynamicallyAdjustTopicCount</span></span>|<span data-ttu-id="fe68a-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe68a-112">Boolean</span></span>|<span data-ttu-id="fe68a-113">Дополнительные дополнительные вопросы см. в [см. встраив максимальное количество тем динамически.](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#themes)</span><span class="sxs-lookup"><span data-stu-id="fe68a-113">To learn more, see [Adjust maximum number of themes dynamically](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#themes).</span></span>|
|<span data-ttu-id="fe68a-114">ignoreNumbers</span><span class="sxs-lookup"><span data-stu-id="fe68a-114">ignoreNumbers</span></span>|<span data-ttu-id="fe68a-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe68a-115">Boolean</span></span>|<span data-ttu-id="fe68a-116">Дополнительные данные см. в [дополнительных подробной информации о включаем числа в темы.](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#themes)</span><span class="sxs-lookup"><span data-stu-id="fe68a-116">To learn more, see [Include numbers in themes](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#themes).</span></span>|
|<span data-ttu-id="fe68a-117">isEnabled</span><span class="sxs-lookup"><span data-stu-id="fe68a-117">isEnabled</span></span>|<span data-ttu-id="fe68a-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe68a-118">Boolean</span></span>|<span data-ttu-id="fe68a-119">Указывает, включены ли темы для дела.</span><span class="sxs-lookup"><span data-stu-id="fe68a-119">Indicates whether themes is enabled for the case.</span></span>|
|<span data-ttu-id="fe68a-120">topicCount</span><span class="sxs-lookup"><span data-stu-id="fe68a-120">topicCount</span></span>|<span data-ttu-id="fe68a-121">Int32</span><span class="sxs-lookup"><span data-stu-id="fe68a-121">Int32</span></span>|<span data-ttu-id="fe68a-122">Дополнительные дополнительные вопросы см. в дополнительных подробной информации о [максимальном количестве тем.](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#themes)</span><span class="sxs-lookup"><span data-stu-id="fe68a-122">To learn more, see [Maximum number of themes](/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#themes).</span></span>|

## <a name="relationships"></a><span data-ttu-id="fe68a-123">Связи</span><span class="sxs-lookup"><span data-stu-id="fe68a-123">Relationships</span></span>

<span data-ttu-id="fe68a-124">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="fe68a-124">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fe68a-125">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="fe68a-125">JSON representation</span></span>

<span data-ttu-id="fe68a-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fe68a-126">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.ediscovery.topicModelingSettings"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.topicModelingSettings",
  "isEnabled": "Boolean",
  "ignoreNumbers": "Boolean",
  "topicCount": "Integer",
  "dynamicallyAdjustTopicCount": "Boolean"
}
```
