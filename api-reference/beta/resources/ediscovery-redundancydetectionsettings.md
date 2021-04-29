---
title: тип ресурса redundancyDetectionSettings
description: Параметры избыточности для дела об обнаружении электронных данных
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: fd1ca1ea3faf03e2639896c79acd0629931c71c9
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080890"
---
# <a name="redundancydetectionsettings-resource-type"></a><span data-ttu-id="cc71f-103">тип ресурса redundancyDetectionSettings</span><span class="sxs-lookup"><span data-stu-id="cc71f-103">redundancyDetectionSettings resource type</span></span>

<span data-ttu-id="cc71f-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="cc71f-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc71f-105">Параметры избыточности (потоковой отправки электронной почты и обнаружения неподалеку от дубликата) для случая обнаружения электронных данных.</span><span class="sxs-lookup"><span data-stu-id="cc71f-105">Redundancy (email threading and near duplicate detection) settings for an eDiscovery case.</span></span>

## <a name="properties"></a><span data-ttu-id="cc71f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="cc71f-106">Properties</span></span>

|<span data-ttu-id="cc71f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="cc71f-107">Property</span></span>|<span data-ttu-id="cc71f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="cc71f-108">Type</span></span>|<span data-ttu-id="cc71f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="cc71f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc71f-110">isEnabled</span><span class="sxs-lookup"><span data-stu-id="cc71f-110">isEnabled</span></span>|<span data-ttu-id="cc71f-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc71f-111">Boolean</span></span>|<span data-ttu-id="cc71f-112">Указывает, включена ли потоковая отправка электронной почты и обнаружение дубликата.</span><span class="sxs-lookup"><span data-stu-id="cc71f-112">Indicates whether email threading and near duplicate detection are enabled.</span></span>|
|<span data-ttu-id="cc71f-113">maxWords</span><span class="sxs-lookup"><span data-stu-id="cc71f-113">maxWords</span></span>|<span data-ttu-id="cc71f-114">Int32</span><span class="sxs-lookup"><span data-stu-id="cc71f-114">Int32</span></span>|<span data-ttu-id="cc71f-115">Узнайте [больше о минимальном](https://docs.microsoft.com/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#near-duplicates-and-email-threading) или максимальном количестве слов.</span><span class="sxs-lookup"><span data-stu-id="cc71f-115">See [Minimum/maximum number of words](https://docs.microsoft.com/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#near-duplicates-and-email-threading) to learn more.</span></span>|
|<span data-ttu-id="cc71f-116">minWords</span><span class="sxs-lookup"><span data-stu-id="cc71f-116">minWords</span></span>|<span data-ttu-id="cc71f-117">Int32</span><span class="sxs-lookup"><span data-stu-id="cc71f-117">Int32</span></span>|<span data-ttu-id="cc71f-118">Узнайте [больше о минимальном](https://docs.microsoft.com/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#near-duplicates-and-email-threading) или максимальном количестве слов.</span><span class="sxs-lookup"><span data-stu-id="cc71f-118">See [Minimum/maximum number of words](https://docs.microsoft.com/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#near-duplicates-and-email-threading) to learn more.</span></span>|
|<span data-ttu-id="cc71f-119">similarityThreshold</span><span class="sxs-lookup"><span data-stu-id="cc71f-119">similarityThreshold</span></span>|<span data-ttu-id="cc71f-120">Int32</span><span class="sxs-lookup"><span data-stu-id="cc71f-120">Int32</span></span>|<span data-ttu-id="cc71f-121">Подробнее [см. в сообщении о пороге сходства](https://docs.microsoft.com/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#near-duplicates-and-email-threading) документов и электронной почты.</span><span class="sxs-lookup"><span data-stu-id="cc71f-121">See [Document and email similarity threshold](https://docs.microsoft.com/microsoft-365/compliance/configure-search-and-analytics-settings-in-advanced-ediscovery#near-duplicates-and-email-threading) to learn more.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cc71f-122">Связи</span><span class="sxs-lookup"><span data-stu-id="cc71f-122">Relationships</span></span>

<span data-ttu-id="cc71f-123">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="cc71f-123">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cc71f-124">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="cc71f-124">JSON representation</span></span>

<span data-ttu-id="cc71f-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cc71f-125">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.ediscovery.redundancyDetectionSettings"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.redundancyDetectionSettings",
  "isEnabled": "Boolean",
  "similarityThreshold": "Integer",
  "minWords": "Integer",
  "maxWords": "Integer"
}
```
