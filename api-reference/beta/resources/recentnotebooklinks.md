---
title: Тип ресурса recentNotebookLinks
description: Ссылки для открытия записной книжки OneNote. Этот тип ресурса существует как свойство ресурса recentNotebook.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: f98feb5e9fbe5cede591f4edf0349b3bf4267de9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521259"
---
# <a name="recentnotebooklinks-resource-type"></a><span data-ttu-id="67325-104">Тип ресурса recentNotebookLinks</span><span class="sxs-lookup"><span data-stu-id="67325-104">recentNotebookLinks resource type</span></span>

<span data-ttu-id="67325-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67325-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67325-106">Ссылки для открытия записной книжки OneNote.</span><span class="sxs-lookup"><span data-stu-id="67325-106">Links to open a OneNote notebook.</span></span> <span data-ttu-id="67325-107">Этот тип ресурса существует как свойство ресурса [recentNotebook](recentnotebook.md).</span><span class="sxs-lookup"><span data-stu-id="67325-107">This resource type exists as a property on a [recentNotebook](recentnotebook.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="67325-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="67325-108">Properties</span></span>
| <span data-ttu-id="67325-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="67325-109">Property</span></span>     | <span data-ttu-id="67325-110">Тип</span><span class="sxs-lookup"><span data-stu-id="67325-110">Type</span></span>   |<span data-ttu-id="67325-111">Описание</span><span class="sxs-lookup"><span data-stu-id="67325-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="67325-112">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="67325-112">oneNoteClientUrl</span></span>|[<span data-ttu-id="67325-113">externalLink</span><span class="sxs-lookup"><span data-stu-id="67325-113">externalLink</span></span>](externallink.md)|<span data-ttu-id="67325-114">Открывает записную книжку в клиенте OneNote, если она установлена.</span><span class="sxs-lookup"><span data-stu-id="67325-114">Opens the notebook in the OneNote client, if it's installed.</span></span>|
|<span data-ttu-id="67325-115">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="67325-115">oneNoteWebUrl</span></span>|[<span data-ttu-id="67325-116">externalLink</span><span class="sxs-lookup"><span data-stu-id="67325-116">externalLink</span></span>](externallink.md)|<span data-ttu-id="67325-117">Открывает записную книжку в OneNote в Интернете.</span><span class="sxs-lookup"><span data-stu-id="67325-117">Opens the notebook in OneNote on the web.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="67325-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="67325-118">JSON representation</span></span>

<span data-ttu-id="67325-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="67325-119">The following is a JSON representation of the resource.</span></span>

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
