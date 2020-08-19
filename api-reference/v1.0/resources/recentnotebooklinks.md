---
title: Тип ресурса recentNotebookLinks
description: Ссылки для открытия записной книжки OneNote. Этот тип ресурса существует как свойство ресурса recentNotebook.
localization_priority: Normal
author: jewan-microsoft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f438437d5287e666e99e24e9a4ca1e207aceb527
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806830"
---
# <a name="recentnotebooklinks-resource-type"></a><span data-ttu-id="a1d17-104">Тип ресурса recentNotebookLinks</span><span class="sxs-lookup"><span data-stu-id="a1d17-104">recentNotebookLinks resource type</span></span>

<span data-ttu-id="a1d17-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1d17-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a1d17-106">Ссылки для открытия записной книжки OneNote.</span><span class="sxs-lookup"><span data-stu-id="a1d17-106">Links for opening a OneNote notebook.</span></span> <span data-ttu-id="a1d17-107">Этот тип ресурса существует как свойство ресурса [recentNotebook](recentnotebook.md).</span><span class="sxs-lookup"><span data-stu-id="a1d17-107">This resource type exists as a property on a [recentNotebook](recentnotebook.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="a1d17-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a1d17-108">Properties</span></span>
| <span data-ttu-id="a1d17-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a1d17-109">Property</span></span>     | <span data-ttu-id="a1d17-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a1d17-110">Type</span></span>   |<span data-ttu-id="a1d17-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a1d17-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a1d17-112">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="a1d17-112">oneNoteClientUrl</span></span>|[<span data-ttu-id="a1d17-113">externalLink</span><span class="sxs-lookup"><span data-stu-id="a1d17-113">externalLink</span></span>](externallink.md)|<span data-ttu-id="a1d17-114">Открывает записную книжку в собственном клиенте OneNote, если он установлен.</span><span class="sxs-lookup"><span data-stu-id="a1d17-114">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="a1d17-115">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="a1d17-115">oneNoteWebUrl</span></span>|[<span data-ttu-id="a1d17-116">externalLink</span><span class="sxs-lookup"><span data-stu-id="a1d17-116">externalLink</span></span>](externallink.md)|<span data-ttu-id="a1d17-117">Открывает записную книжку в OneNote в Интернете.</span><span class="sxs-lookup"><span data-stu-id="a1d17-117">Opens the notebook in OneNote on the web.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a1d17-118">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a1d17-118">JSON representation</span></span>

<span data-ttu-id="a1d17-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a1d17-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recentNotebookLinks"
}-->

```json
{
  "oneNoteClientUrl": {"@odata.type": "microsoft.graph.externalLink"},
  "oneNoteWebUrl": {"@odata.type": "microsoft.graph.externalLink"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recentNotebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
