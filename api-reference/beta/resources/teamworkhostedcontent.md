---
title: тип ресурса teamworkHostedContent
description: Представляет богатый контент, который организован Microsoft Teams
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: da0b157bab78867bd3309b4529afe8ef734f0144
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882315"
---
# <a name="teamworkhostedcontent-resource-type"></a><span data-ttu-id="60ca4-103">тип ресурса teamworkHostedContent</span><span class="sxs-lookup"><span data-stu-id="60ca4-103">teamworkHostedContent resource type</span></span>

<span data-ttu-id="60ca4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60ca4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60ca4-105">Представляет богатый контент, например изображения и фрагменты кода в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="60ca4-105">Represents rich content like images and code snippets in Microsoft Teams.</span></span> <span data-ttu-id="60ca4-106">Для богатого [контента в сообщениях](chatMessage.md)каналов и чатов см. [в странице chatMessageHostedContent.](chatMessageHostedContent.md)</span><span class="sxs-lookup"><span data-stu-id="60ca4-106">For rich content in [channel and chat messages](chatMessage.md), see [chatMessageHostedContent](chatMessageHostedContent.md).</span></span>

## <a name="methods"></a><span data-ttu-id="60ca4-107">Методы</span><span class="sxs-lookup"><span data-stu-id="60ca4-107">Methods</span></span>

| <span data-ttu-id="60ca4-108">Метод</span><span class="sxs-lookup"><span data-stu-id="60ca4-108">Method</span></span>                                            | <span data-ttu-id="60ca4-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="60ca4-109">Return Type</span></span>                                       | <span data-ttu-id="60ca4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="60ca4-110">Description</span></span>                                                    | 
| :------------------------------------------------ | :------------------------------------------------ | :------------------------------------------------------------- |
| [<span data-ttu-id="60ca4-111">Получите иконки приложений</span><span class="sxs-lookup"><span data-stu-id="60ca4-111">Get app icon bytes</span></span>](../api/teamsappicon-get.md)     | [<span data-ttu-id="60ca4-112">teamworkHostedContent</span><span class="sxs-lookup"><span data-stu-id="60ca4-112">teamworkHostedContent</span></span>](teamworkhostedcontent.md)                   | <span data-ttu-id="60ca4-113">Получите bytes of the hosted content backing a Teams app icon.</span><span class="sxs-lookup"><span data-stu-id="60ca4-113">Get the bytes of the hosted content backing a Teams app icon.</span></span> |

## <a name="properties"></a><span data-ttu-id="60ca4-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="60ca4-114">Properties</span></span>
|<span data-ttu-id="60ca4-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="60ca4-115">Property</span></span>|<span data-ttu-id="60ca4-116">Тип</span><span class="sxs-lookup"><span data-stu-id="60ca4-116">Type</span></span>|<span data-ttu-id="60ca4-117">Описание</span><span class="sxs-lookup"><span data-stu-id="60ca4-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60ca4-118">contentBytes</span><span class="sxs-lookup"><span data-stu-id="60ca4-118">contentBytes</span></span>|<span data-ttu-id="60ca4-119">Двоичный</span><span class="sxs-lookup"><span data-stu-id="60ca4-119">Binary</span></span>|<span data-ttu-id="60ca4-120">Только напишите.</span><span class="sxs-lookup"><span data-stu-id="60ca4-120">Write only.</span></span> <span data-ttu-id="60ca4-121">Bytes for the hosted content (such as images).</span><span class="sxs-lookup"><span data-stu-id="60ca4-121">Bytes for the hosted content (such as images).</span></span>|
|<span data-ttu-id="60ca4-122">contentType</span><span class="sxs-lookup"><span data-stu-id="60ca4-122">contentType</span></span>|<span data-ttu-id="60ca4-123">String</span><span class="sxs-lookup"><span data-stu-id="60ca4-123">String</span></span>|<span data-ttu-id="60ca4-124">Только напишите.</span><span class="sxs-lookup"><span data-stu-id="60ca4-124">Write only.</span></span> <span data-ttu-id="60ca4-125">Тип контента, например изображение/png, изображение/jpg.</span><span class="sxs-lookup"><span data-stu-id="60ca4-125">Content type, such as image/png, image/jpg.</span></span>|
|<span data-ttu-id="60ca4-126">id</span><span class="sxs-lookup"><span data-stu-id="60ca4-126">id</span></span>|<span data-ttu-id="60ca4-127">Строка</span><span class="sxs-lookup"><span data-stu-id="60ca4-127">String</span></span>|<span data-ttu-id="60ca4-128">ID хост-контента.</span><span class="sxs-lookup"><span data-stu-id="60ca4-128">ID of the hosted content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="60ca4-129">Связи</span><span class="sxs-lookup"><span data-stu-id="60ca4-129">Relationships</span></span>
<span data-ttu-id="60ca4-130">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="60ca4-130">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="60ca4-131">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="60ca4-131">JSON representation</span></span>
<span data-ttu-id="60ca4-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="60ca4-132">The following is a JSON representation of the resource.</span></span>
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

