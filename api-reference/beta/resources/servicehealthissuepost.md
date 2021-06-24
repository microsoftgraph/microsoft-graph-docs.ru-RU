---
title: тип ресурса serviceHealthIssuePost
description: Представляет историческую должность в проблеме со здоровьем службы.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: 910236d2059f951169bea314a0b38ae2516b1918
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53107840"
---
# <a name="servicehealthissuepost-resource-type"></a><span data-ttu-id="36357-103">тип ресурса serviceHealthIssuePost</span><span class="sxs-lookup"><span data-stu-id="36357-103">serviceHealthIssuePost resource type</span></span>

<span data-ttu-id="36357-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36357-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36357-105">Представляет исторический пост в проблеме [со здоровьем службы.](../resources/servicehealthissue.md)</span><span class="sxs-lookup"><span data-stu-id="36357-105">Represents a historical post in a [service health issue](../resources/servicehealthissue.md).</span></span>

## <a name="properties"></a><span data-ttu-id="36357-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="36357-106">Properties</span></span>
|<span data-ttu-id="36357-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="36357-107">Property</span></span>|<span data-ttu-id="36357-108">Тип</span><span class="sxs-lookup"><span data-stu-id="36357-108">Type</span></span>|<span data-ttu-id="36357-109">Описание</span><span class="sxs-lookup"><span data-stu-id="36357-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36357-110">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="36357-110">createdDateTime</span></span>|<span data-ttu-id="36357-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36357-111">DateTimeOffset</span></span>|<span data-ttu-id="36357-112">Опубликовано время публикации.</span><span class="sxs-lookup"><span data-stu-id="36357-112">The published time of the post.</span></span>|
|<span data-ttu-id="36357-113">description</span><span class="sxs-lookup"><span data-stu-id="36357-113">description</span></span>|[<span data-ttu-id="36357-114">itemBody</span><span class="sxs-lookup"><span data-stu-id="36357-114">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="36357-115">Содержимое сообщения о проблеме службы.</span><span class="sxs-lookup"><span data-stu-id="36357-115">The content of the service issue post.</span></span>|
|<span data-ttu-id="36357-116">postType</span><span class="sxs-lookup"><span data-stu-id="36357-116">postType</span></span>|<span data-ttu-id="36357-117">postType</span><span class="sxs-lookup"><span data-stu-id="36357-117">postType</span></span>|<span data-ttu-id="36357-118">Тип столба исторической публикации службы.</span><span class="sxs-lookup"><span data-stu-id="36357-118">The post type of the service issue historical post.</span></span> <span data-ttu-id="36357-119">Возможные значения: `regular`, `quick`, `strategic`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="36357-119">Possible values are: `regular`, `quick`, `strategic`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="36357-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="36357-120">Relationships</span></span>
<span data-ttu-id="36357-121">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="36357-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="36357-122">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="36357-122">JSON representation</span></span>
<span data-ttu-id="36357-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="36357-123">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.serviceHealthIssuePost"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.serviceHealthIssuePost",
  "createdDateTime": "String (timestamp)",
  "postType": "String",
  "description": {
    "@odata.type": "microsoft.graph.itemBody"
  }
}
```

