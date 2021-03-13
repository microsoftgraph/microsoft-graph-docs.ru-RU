---
title: тип ресурса updateWindow
description: тип ресурса updateWindow.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 7d8f12c7cfcb4c83075087d7b894dc95fe92a695
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761228"
---
# <a name="updatewindow-resource-type"></a><span data-ttu-id="7b9e4-103">тип ресурса updateWindow</span><span class="sxs-lookup"><span data-stu-id="7b9e4-103">updateWindow resource type</span></span>

<span data-ttu-id="7b9e4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7b9e4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b9e4-105">Представляет окно времени, в [течение которого агенты](onpremisesagent.md) могут получать обновления.</span><span class="sxs-lookup"><span data-stu-id="7b9e4-105">Represents time window during which [agents](onpremisesagent.md) can receive updates.</span></span>

## <a name="properties"></a><span data-ttu-id="7b9e4-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="7b9e4-106">Properties</span></span>

| <span data-ttu-id="7b9e4-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="7b9e4-107">Property</span></span>     | <span data-ttu-id="7b9e4-108">Тип</span><span class="sxs-lookup"><span data-stu-id="7b9e4-108">Type</span></span>        | <span data-ttu-id="7b9e4-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7b9e4-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7b9e4-110">updateWindowEndTime</span><span class="sxs-lookup"><span data-stu-id="7b9e4-110">updateWindowEndTime</span></span>|<span data-ttu-id="7b9e4-111">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="7b9e4-111">TimeOfDay</span></span>|<span data-ttu-id="7b9e4-112">Конец окне времени, в течение которого агенты могут получать обновления</span><span class="sxs-lookup"><span data-stu-id="7b9e4-112">End of a time window during which agents can receive updates</span></span>|
|<span data-ttu-id="7b9e4-113">updateWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="7b9e4-113">updateWindowStartTime</span></span>|<span data-ttu-id="7b9e4-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="7b9e4-114">TimeOfDay</span></span>|<span data-ttu-id="7b9e4-115">Начало окна времени, в течение которого агенты могут получать обновления</span><span class="sxs-lookup"><span data-stu-id="7b9e4-115">Start of a time window during which agents can receive updates</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7b9e4-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7b9e4-116">JSON representation</span></span>

<span data-ttu-id="7b9e4-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7b9e4-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.updateWindow",
  "baseType": null
}-->

```json
{
  "updateWindowEndTime": "String (timestamp)",
  "updateWindowStartTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "updateWindow resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


