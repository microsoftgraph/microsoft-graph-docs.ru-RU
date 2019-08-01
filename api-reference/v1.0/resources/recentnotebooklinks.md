---
title: Тип ресурса recentNotebookLinks
description: Ссылки для открытия записной книжки OneNote. Этот тип ресурса существует как свойство ресурса recentNotebook.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f112d8ff87329ca23a3a44fb33dafe4582072519
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034834"
---
# <a name="recentnotebooklinks-resource-type"></a><span data-ttu-id="5f046-104">Тип ресурса recentNotebookLinks</span><span class="sxs-lookup"><span data-stu-id="5f046-104">recentNotebookLinks resource type</span></span>

<span data-ttu-id="5f046-105">Ссылки для открытия записной книжки OneNote.</span><span class="sxs-lookup"><span data-stu-id="5f046-105">Links for opening a OneNote notebook.</span></span> <span data-ttu-id="5f046-106">Этот тип ресурса существует как свойство ресурса [recentNotebook](recentnotebook.md).</span><span class="sxs-lookup"><span data-stu-id="5f046-106">This resource type exists as a property on a [recentNotebook](recentnotebook.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="5f046-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5f046-107">Properties</span></span>
| <span data-ttu-id="5f046-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="5f046-108">Property</span></span>     | <span data-ttu-id="5f046-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5f046-109">Type</span></span>   |<span data-ttu-id="5f046-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5f046-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5f046-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="5f046-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="5f046-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="5f046-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="5f046-113">Открывает записную книжку в собственном клиенте OneNote, если он установлен.</span><span class="sxs-lookup"><span data-stu-id="5f046-113">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="5f046-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="5f046-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="5f046-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="5f046-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="5f046-116">Открывает записную книжку в OneNote в Интернете.</span><span class="sxs-lookup"><span data-stu-id="5f046-116">Opens the notebook in OneNote on the web.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5f046-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5f046-117">JSON representation</span></span>

<span data-ttu-id="5f046-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5f046-118">The following is a JSON representation of the resource.</span></span>

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
