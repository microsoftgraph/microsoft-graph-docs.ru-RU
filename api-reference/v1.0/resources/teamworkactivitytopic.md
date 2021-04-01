---
title: тип ресурса teamworkActivityTopic
description: Представляет тему уведомления о канале действий.
author: eddie-lee-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: abf2372aca7d58061f609c97521795f328af89f6
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51474018"
---
# <a name="teamworkactivitytopic-resource-type"></a><span data-ttu-id="7935d-103">тип ресурса teamworkActivityTopic</span><span class="sxs-lookup"><span data-stu-id="7935d-103">teamworkActivityTopic resource type</span></span>

<span data-ttu-id="7935d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7935d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7935d-105">Представляет тему уведомления о канале действий.</span><span class="sxs-lookup"><span data-stu-id="7935d-105">Represents the topic of an activity feed notification.</span></span>

## <a name="properties"></a><span data-ttu-id="7935d-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="7935d-106">Properties</span></span>
|<span data-ttu-id="7935d-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="7935d-107">Property</span></span>|<span data-ttu-id="7935d-108">Тип</span><span class="sxs-lookup"><span data-stu-id="7935d-108">Type</span></span>|<span data-ttu-id="7935d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7935d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7935d-110">source</span><span class="sxs-lookup"><span data-stu-id="7935d-110">source</span></span>|<span data-ttu-id="7935d-111">teamworkActivityTopicSource</span><span class="sxs-lookup"><span data-stu-id="7935d-111">teamworkActivityTopicSource</span></span>|<span data-ttu-id="7935d-112">Тип источника.</span><span class="sxs-lookup"><span data-stu-id="7935d-112">Type of source.</span></span> <span data-ttu-id="7935d-113">Возможные значения: `entityUrl`, `text`.</span><span class="sxs-lookup"><span data-stu-id="7935d-113">Possible values are: `entityUrl`, `text`.</span></span> <span data-ttu-id="7935d-114">Для поддерживаемых URL-адресов Microsoft Graph используйте `entityUrl` .</span><span class="sxs-lookup"><span data-stu-id="7935d-114">For supported Microsoft Graph URLs, use `entityUrl`.</span></span> <span data-ttu-id="7935d-115">Для пользовательского текста используйте `text` .</span><span class="sxs-lookup"><span data-stu-id="7935d-115">For custom text, use `text`.</span></span>|
|<span data-ttu-id="7935d-116">value</span><span class="sxs-lookup"><span data-stu-id="7935d-116">value</span></span>|<span data-ttu-id="7935d-117">String</span><span class="sxs-lookup"><span data-stu-id="7935d-117">String</span></span>|<span data-ttu-id="7935d-118">Значение темы.</span><span class="sxs-lookup"><span data-stu-id="7935d-118">The topic value.</span></span> <span data-ttu-id="7935d-119">Если значение свойства **источника** , это должен `entityUrl` быть URL-адрес Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="7935d-119">If the value of the **source** property is `entityUrl`, this must be a Microsoft Graph URL.</span></span> <span data-ttu-id="7935d-120">Если вейл `text` есть, это должно быть простое текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="7935d-120">If the vaule is `text`, this must be a plain text value.</span></span>|
|<span data-ttu-id="7935d-121">webUrl</span><span class="sxs-lookup"><span data-stu-id="7935d-121">webUrl</span></span>|<span data-ttu-id="7935d-122">String</span><span class="sxs-lookup"><span data-stu-id="7935d-122">String</span></span>|<span data-ttu-id="7935d-123">При выборе уведомления пользователь щелкает ссылку.</span><span class="sxs-lookup"><span data-stu-id="7935d-123">The link the user clicks when they select the notification.</span></span> <span data-ttu-id="7935d-124">**Необязательный,** когда `entityUrl` источник; требуется, **когда источник** `text` .</span><span class="sxs-lookup"><span data-stu-id="7935d-124">Optional when **source** is `entityUrl`; required when **source** is `text`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7935d-125">Связи</span><span class="sxs-lookup"><span data-stu-id="7935d-125">Relationships</span></span>
<span data-ttu-id="7935d-126">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7935d-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7935d-127">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7935d-127">JSON representation</span></span>
<span data-ttu-id="7935d-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7935d-128">The following is a JSON representation of the resource.</span></span>
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

