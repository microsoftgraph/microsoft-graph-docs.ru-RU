---
title: Тип ресурса recentNotebookLinks
description: Ссылки для открытия записной книжки OneNote. Этот тип ресурса существует как свойство ресурса recentNotebook.
localization_priority: Normal
author: jewan-microsoft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f6961a267948c62ac1d24623c6d8bbeaf94f7569
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078999"
---
# <a name="recentnotebooklinks-resource-type"></a><span data-ttu-id="f8e4e-104">Тип ресурса recentNotebookLinks</span><span class="sxs-lookup"><span data-stu-id="f8e4e-104">recentNotebookLinks resource type</span></span>

<span data-ttu-id="f8e4e-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8e4e-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f8e4e-106">Ссылки для открытия записной книжки OneNote.</span><span class="sxs-lookup"><span data-stu-id="f8e4e-106">Links for opening a OneNote notebook.</span></span> <span data-ttu-id="f8e4e-107">Этот тип ресурса существует как свойство ресурса [recentNotebook](recentnotebook.md).</span><span class="sxs-lookup"><span data-stu-id="f8e4e-107">This resource type exists as a property on a [recentNotebook](recentnotebook.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="f8e4e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f8e4e-108">Properties</span></span>
| <span data-ttu-id="f8e4e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f8e4e-109">Property</span></span>     | <span data-ttu-id="f8e4e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f8e4e-110">Type</span></span>   |<span data-ttu-id="f8e4e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f8e4e-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f8e4e-112">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="f8e4e-112">oneNoteClientUrl</span></span>|[<span data-ttu-id="f8e4e-113">externalLink</span><span class="sxs-lookup"><span data-stu-id="f8e4e-113">externalLink</span></span>](externallink.md)|<span data-ttu-id="f8e4e-114">Открывает записную книжку в собственном клиенте OneNote, если он установлен.</span><span class="sxs-lookup"><span data-stu-id="f8e4e-114">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="f8e4e-115">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="f8e4e-115">oneNoteWebUrl</span></span>|[<span data-ttu-id="f8e4e-116">externalLink</span><span class="sxs-lookup"><span data-stu-id="f8e4e-116">externalLink</span></span>](externallink.md)|<span data-ttu-id="f8e4e-117">Открывает записную книжку в OneNote в Интернете.</span><span class="sxs-lookup"><span data-stu-id="f8e4e-117">Opens the notebook in OneNote on the web.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f8e4e-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f8e4e-118">JSON representation</span></span>

<span data-ttu-id="f8e4e-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f8e4e-119">The following is a JSON representation of the resource.</span></span>

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

