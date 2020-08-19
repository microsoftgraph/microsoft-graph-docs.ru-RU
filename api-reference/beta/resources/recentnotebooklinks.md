---
title: Тип ресурса recentNotebookLinks
description: Ссылки для открытия записной книжки OneNote. Этот тип ресурса существует как свойство ресурса recentNotebook.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: jewan-microsoft
ms.openlocfilehash: 4114704a13b4116534d96743ceacfba51df67847
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812458"
---
# <a name="recentnotebooklinks-resource-type"></a><span data-ttu-id="bf418-104">Тип ресурса recentNotebookLinks</span><span class="sxs-lookup"><span data-stu-id="bf418-104">recentNotebookLinks resource type</span></span>

<span data-ttu-id="bf418-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf418-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf418-106">Ссылки для открытия записной книжки OneNote.</span><span class="sxs-lookup"><span data-stu-id="bf418-106">Links to open a OneNote notebook.</span></span> <span data-ttu-id="bf418-107">Этот тип ресурса существует как свойство ресурса [recentNotebook](recentnotebook.md).</span><span class="sxs-lookup"><span data-stu-id="bf418-107">This resource type exists as a property on a [recentNotebook](recentnotebook.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="bf418-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="bf418-108">Properties</span></span>
| <span data-ttu-id="bf418-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="bf418-109">Property</span></span>     | <span data-ttu-id="bf418-110">Тип</span><span class="sxs-lookup"><span data-stu-id="bf418-110">Type</span></span>   |<span data-ttu-id="bf418-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bf418-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bf418-112">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="bf418-112">oneNoteClientUrl</span></span>|[<span data-ttu-id="bf418-113">externalLink</span><span class="sxs-lookup"><span data-stu-id="bf418-113">externalLink</span></span>](externallink.md)|<span data-ttu-id="bf418-114">Открывает записную книжку в клиенте OneNote, если она установлена.</span><span class="sxs-lookup"><span data-stu-id="bf418-114">Opens the notebook in the OneNote client, if it's installed.</span></span>|
|<span data-ttu-id="bf418-115">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="bf418-115">oneNoteWebUrl</span></span>|[<span data-ttu-id="bf418-116">externalLink</span><span class="sxs-lookup"><span data-stu-id="bf418-116">externalLink</span></span>](externallink.md)|<span data-ttu-id="bf418-117">Открывает записную книжку в OneNote в Интернете.</span><span class="sxs-lookup"><span data-stu-id="bf418-117">Opens the notebook in OneNote on the web.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bf418-118">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="bf418-118">JSON representation</span></span>

<span data-ttu-id="bf418-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bf418-119">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "recentNotebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
