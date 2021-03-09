---
title: тип ресурса teamworkHostedContent
description: Представляет богатый контент, который организован Microsoft Teams
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 93b3b4fc817c1fe3aa3973a112b9cf887c825b6e
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50578862"
---
# <a name="teamworkhostedcontent-resource-type"></a><span data-ttu-id="24e2e-103">тип ресурса teamworkHostedContent</span><span class="sxs-lookup"><span data-stu-id="24e2e-103">teamworkHostedContent resource type</span></span>

<span data-ttu-id="24e2e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24e2e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24e2e-105">Представляет богатый контент, например изображения и фрагменты кода в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="24e2e-105">Represents rich content like images and code snippets in Microsoft Teams.</span></span> <span data-ttu-id="24e2e-106">Для богатого [контента в сообщениях](chatMessage.md)каналов и чатов см. [в странице chatMessageHostedContent.](chatMessageHostedContent.md)</span><span class="sxs-lookup"><span data-stu-id="24e2e-106">For rich content in [channel and chat messages](chatMessage.md), see [chatMessageHostedContent](chatMessageHostedContent.md).</span></span>

## <a name="properties"></a><span data-ttu-id="24e2e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="24e2e-107">Properties</span></span>
|<span data-ttu-id="24e2e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="24e2e-108">Property</span></span>|<span data-ttu-id="24e2e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="24e2e-109">Type</span></span>|<span data-ttu-id="24e2e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="24e2e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24e2e-111">contentBytes</span><span class="sxs-lookup"><span data-stu-id="24e2e-111">contentBytes</span></span>|<span data-ttu-id="24e2e-112">Двоичный</span><span class="sxs-lookup"><span data-stu-id="24e2e-112">Binary</span></span>|<span data-ttu-id="24e2e-113">Только напишите.</span><span class="sxs-lookup"><span data-stu-id="24e2e-113">Write only.</span></span> <span data-ttu-id="24e2e-114">Bytes for the hosted content (such as images).</span><span class="sxs-lookup"><span data-stu-id="24e2e-114">Bytes for the hosted content (such as images).</span></span>|
|<span data-ttu-id="24e2e-115">contentType</span><span class="sxs-lookup"><span data-stu-id="24e2e-115">contentType</span></span>|<span data-ttu-id="24e2e-116">String</span><span class="sxs-lookup"><span data-stu-id="24e2e-116">String</span></span>|<span data-ttu-id="24e2e-117">Только напишите.</span><span class="sxs-lookup"><span data-stu-id="24e2e-117">Write only.</span></span> <span data-ttu-id="24e2e-118">Тип контента, например изображение/png, изображение/jpg.</span><span class="sxs-lookup"><span data-stu-id="24e2e-118">Content type, such as image/png, image/jpg.</span></span>|
|<span data-ttu-id="24e2e-119">id</span><span class="sxs-lookup"><span data-stu-id="24e2e-119">id</span></span>|<span data-ttu-id="24e2e-120">String</span><span class="sxs-lookup"><span data-stu-id="24e2e-120">String</span></span>|<span data-ttu-id="24e2e-121">ID хост-контента.</span><span class="sxs-lookup"><span data-stu-id="24e2e-121">ID of the hosted content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="24e2e-122">Связи</span><span class="sxs-lookup"><span data-stu-id="24e2e-122">Relationships</span></span>
<span data-ttu-id="24e2e-123">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="24e2e-123">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="24e2e-124">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="24e2e-124">JSON representation</span></span>
<span data-ttu-id="24e2e-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="24e2e-125">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamworkHostedContent",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkHostedContent",
  "id": "String (identifier)",
  "contentBytes": "Binary",
  "contentType": "String"
}
```

