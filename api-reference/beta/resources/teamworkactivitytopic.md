---
title: Тип ресурса Теамворкактивититопик
description: Представляет раздел уведомления о канале активности.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a4425053cf41ebfbad139c6d0ea5fc246f0b1391
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377611"
---
# <a name="teamworkactivitytopic-resource-type"></a><span data-ttu-id="2a570-103">Тип ресурса Теамворкактивититопик</span><span class="sxs-lookup"><span data-stu-id="2a570-103">teamworkActivityTopic resource type</span></span>

<span data-ttu-id="2a570-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a570-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2a570-105">Представляет раздел уведомления о канале активности.</span><span class="sxs-lookup"><span data-stu-id="2a570-105">Represents the topic of an activity feed notification.</span></span>

## <a name="properties"></a><span data-ttu-id="2a570-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="2a570-106">Properties</span></span>
|<span data-ttu-id="2a570-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="2a570-107">Property</span></span>|<span data-ttu-id="2a570-108">Тип</span><span class="sxs-lookup"><span data-stu-id="2a570-108">Type</span></span>|<span data-ttu-id="2a570-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2a570-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a570-110">source</span><span class="sxs-lookup"><span data-stu-id="2a570-110">source</span></span>|<span data-ttu-id="2a570-111">теамворкактивититопиксаурце</span><span class="sxs-lookup"><span data-stu-id="2a570-111">teamworkActivityTopicSource</span></span>|<span data-ttu-id="2a570-112">Тип источника.</span><span class="sxs-lookup"><span data-stu-id="2a570-112">Type of source.</span></span> <span data-ttu-id="2a570-113">Возможные значения: `entityUrl`, `text`.</span><span class="sxs-lookup"><span data-stu-id="2a570-113">Possible values are: `entityUrl`, `text`.</span></span> <span data-ttu-id="2a570-114">Для поддерживаемых URL-адресов Microsoft Graph используйте `entityUrl` .</span><span class="sxs-lookup"><span data-stu-id="2a570-114">For supported Microsoft Graph URLs, use `entityUrl`.</span></span> <span data-ttu-id="2a570-115">Для настраиваемого текста используйте `text` .</span><span class="sxs-lookup"><span data-stu-id="2a570-115">For custom text, use `text`.</span></span>|
|<span data-ttu-id="2a570-116">value</span><span class="sxs-lookup"><span data-stu-id="2a570-116">value</span></span>|<span data-ttu-id="2a570-117">String</span><span class="sxs-lookup"><span data-stu-id="2a570-117">String</span></span>|<span data-ttu-id="2a570-118">Значение раздела.</span><span class="sxs-lookup"><span data-stu-id="2a570-118">The topic value.</span></span> <span data-ttu-id="2a570-119">Если свойство **Source** имеет значение `entityUrl` , это должен быть URL-адрес Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2a570-119">If the value of the **source** property is `entityUrl`, this must be a Microsoft Graph URL.</span></span> <span data-ttu-id="2a570-120">Если задано `text` значение вауле, это должно быть обычное текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="2a570-120">If the vaule is `text`, this must be a plain text value.</span></span>|
|<span data-ttu-id="2a570-121">webUrl</span><span class="sxs-lookup"><span data-stu-id="2a570-121">webUrl</span></span>|<span data-ttu-id="2a570-122">String</span><span class="sxs-lookup"><span data-stu-id="2a570-122">String</span></span>|<span data-ttu-id="2a570-123">Ссылка, которую пользователь щелкает при выборе уведомления.</span><span class="sxs-lookup"><span data-stu-id="2a570-123">The link the user clicks when they select the notification.</span></span> <span data-ttu-id="2a570-124">Необязательный параметр, если **источник** — это `entityUrl` обязательный **параметр** `text` .</span><span class="sxs-lookup"><span data-stu-id="2a570-124">Optional when **source** is `entityUrl`; required when **source** is `text`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2a570-125">Связи</span><span class="sxs-lookup"><span data-stu-id="2a570-125">Relationships</span></span>
<span data-ttu-id="2a570-126">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="2a570-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2a570-127">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2a570-127">JSON representation</span></span>
<span data-ttu-id="2a570-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2a570-128">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkActivityTopic"
}
-->
```json
{
  "@odata.type": "#microsoft.graph.teamworkActivityTopic",
  "source": "String",
  "value": "String",
  "webUrl": "String"
}
```

