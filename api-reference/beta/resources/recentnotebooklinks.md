---
title: Тип ресурса recentNotebookLinks
description: Ссылки на открытие записной книжке OneNote. Этот тип ресурса существует как свойство ресурса recentNotebook.
localization_priority: Normal
ms.openlocfilehash: 5ccf861541526a1673d6174176cb8b2a62df6c23
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812875"
---
# <a name="recentnotebooklinks-resource-type"></a><span data-ttu-id="863cd-104">Тип ресурса recentNotebookLinks</span><span class="sxs-lookup"><span data-stu-id="863cd-104">recentNotebookLinks resource type</span></span>

> <span data-ttu-id="863cd-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="863cd-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="863cd-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="863cd-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="863cd-107">Ссылки на открытие записной книжке OneNote.</span><span class="sxs-lookup"><span data-stu-id="863cd-107">Links to open a OneNote notebook.</span></span> <span data-ttu-id="863cd-108">Этот тип ресурса существует как свойство ресурса [recentNotebook](recentnotebook.md).</span><span class="sxs-lookup"><span data-stu-id="863cd-108">This resource type exists as a property on a [recentNotebook](recentnotebook.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="863cd-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="863cd-109">Properties</span></span>
| <span data-ttu-id="863cd-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="863cd-110">Property</span></span>     | <span data-ttu-id="863cd-111">Тип</span><span class="sxs-lookup"><span data-stu-id="863cd-111">Type</span></span>   |<span data-ttu-id="863cd-112">Описание</span><span class="sxs-lookup"><span data-stu-id="863cd-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="863cd-113">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="863cd-113">oneNoteClientUrl</span></span>|[<span data-ttu-id="863cd-114">externalLink</span><span class="sxs-lookup"><span data-stu-id="863cd-114">externalLink</span></span>](externallink.md)|<span data-ttu-id="863cd-115">Открывает записную книжку в клиент OneNote, если она установлена.</span><span class="sxs-lookup"><span data-stu-id="863cd-115">Opens the notebook in the OneNote client, if it's installed.</span></span>|
|<span data-ttu-id="863cd-116">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="863cd-116">oneNoteWebUrl</span></span>|[<span data-ttu-id="863cd-117">externalLink</span><span class="sxs-lookup"><span data-stu-id="863cd-117">externalLink</span></span>](externallink.md)|<span data-ttu-id="863cd-118">Открывает записную книжку в OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="863cd-118">Opens the notebook in OneNote Online.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="863cd-119">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="863cd-119">JSON representation</span></span>

<span data-ttu-id="863cd-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="863cd-120">The following is a JSON representation of the resource.</span></span>

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
