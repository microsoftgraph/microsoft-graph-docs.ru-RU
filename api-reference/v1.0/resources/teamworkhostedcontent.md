---
title: тип ресурса teamworkHostedContent
description: Представляет богатый контент, на который ведется Microsoft Teams.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 0a4a4d0a553f77766dd4ddb1f68e27b440fdbf2f
ms.sourcegitcommit: cde4a3386b08a67cb476df6d46b51885c643d94f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/10/2021
ms.locfileid: "50634329"
---
# <a name="teamworkhostedcontent-resource-type"></a><span data-ttu-id="b027d-103">тип ресурса teamworkHostedContent</span><span class="sxs-lookup"><span data-stu-id="b027d-103">teamworkHostedContent resource type</span></span>

<span data-ttu-id="b027d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b027d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b027d-105">Представляет богатый контент, например изображения и фрагменты кода в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="b027d-105">Represents rich content like images and code snippets in Microsoft Teams.</span></span> <span data-ttu-id="b027d-106">Для богатого [контента в сообщениях](chatMessage.md)каналов и чатов см. [в странице chatMessageHostedContent.](chatMessageHostedContent.md)</span><span class="sxs-lookup"><span data-stu-id="b027d-106">For rich content in [channel and chat messages](chatMessage.md), see [chatMessageHostedContent](chatMessageHostedContent.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b027d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b027d-107">Properties</span></span>
|<span data-ttu-id="b027d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b027d-108">Property</span></span>|<span data-ttu-id="b027d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b027d-109">Type</span></span>|<span data-ttu-id="b027d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b027d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b027d-111">contentBytes</span><span class="sxs-lookup"><span data-stu-id="b027d-111">contentBytes</span></span>|<span data-ttu-id="b027d-112">Двоичный</span><span class="sxs-lookup"><span data-stu-id="b027d-112">Binary</span></span>|<span data-ttu-id="b027d-113">Только напишите.</span><span class="sxs-lookup"><span data-stu-id="b027d-113">Write only.</span></span> <span data-ttu-id="b027d-114">Bytes for the hosted content (such as images).</span><span class="sxs-lookup"><span data-stu-id="b027d-114">Bytes for the hosted content (such as images).</span></span>|
|<span data-ttu-id="b027d-115">contentType</span><span class="sxs-lookup"><span data-stu-id="b027d-115">contentType</span></span>|<span data-ttu-id="b027d-116">String</span><span class="sxs-lookup"><span data-stu-id="b027d-116">String</span></span>|<span data-ttu-id="b027d-117">Только напишите.</span><span class="sxs-lookup"><span data-stu-id="b027d-117">Write only.</span></span> <span data-ttu-id="b027d-118">Тип контента.</span><span class="sxs-lookup"><span data-stu-id="b027d-118">Content type.</span></span> <span data-ttu-id="b027d-119">sicj as image/png, image/jpg.</span><span class="sxs-lookup"><span data-stu-id="b027d-119">sicj as image/png, image/jpg.</span></span>|
|<span data-ttu-id="b027d-120">id</span><span class="sxs-lookup"><span data-stu-id="b027d-120">id</span></span>|<span data-ttu-id="b027d-121">String</span><span class="sxs-lookup"><span data-stu-id="b027d-121">String</span></span>|<span data-ttu-id="b027d-122">ID хост-контента.</span><span class="sxs-lookup"><span data-stu-id="b027d-122">ID of the hosted content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b027d-123">Связи</span><span class="sxs-lookup"><span data-stu-id="b027d-123">Relationships</span></span>
<span data-ttu-id="b027d-124">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b027d-124">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b027d-125">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b027d-125">JSON representation</span></span>
<span data-ttu-id="b027d-126">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b027d-126">The following is a JSON representation of the resource.</span></span>
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
