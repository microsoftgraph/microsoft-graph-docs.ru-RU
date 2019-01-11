---
title: Тип ресурса notebookLinks
description: Ссылки для открытия записной книжки OneNote.
author: Jewan-microsoft
localization_priority: Normal
ms.openlocfilehash: 9c3012abd5b7ca7b9e7b4a1ce2b36159bcd4d966
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884380"
---
# <a name="notebooklinks-resource-type"></a><span data-ttu-id="47d9c-103">Тип ресурса notebookLinks</span><span class="sxs-lookup"><span data-stu-id="47d9c-103">notebookLinks resource type</span></span>

> <span data-ttu-id="47d9c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="47d9c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="47d9c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47d9c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="47d9c-106">Ссылки для открытия записной книжки OneNote.</span><span class="sxs-lookup"><span data-stu-id="47d9c-106">Links for opening a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="47d9c-107">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="47d9c-107">JSON representation</span></span>

<span data-ttu-id="47d9c-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="47d9c-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.notebookLinks"
}-->

```json
{
  "oneNoteClientUrl": {"@odata.type": "microsoft.graph.externalLink"},
  "oneNoteWebUrl": {"@odata.type": "microsoft.graph.externalLink"}
}

```
## <a name="properties"></a><span data-ttu-id="47d9c-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="47d9c-109">Properties</span></span>
| <span data-ttu-id="47d9c-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="47d9c-110">Property</span></span>     | <span data-ttu-id="47d9c-111">Тип</span><span class="sxs-lookup"><span data-stu-id="47d9c-111">Type</span></span>   |<span data-ttu-id="47d9c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="47d9c-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="47d9c-113">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="47d9c-113">oneNoteClientUrl</span></span>|[<span data-ttu-id="47d9c-114">externalLink</span><span class="sxs-lookup"><span data-stu-id="47d9c-114">externalLink</span></span>](externallink.md)|<span data-ttu-id="47d9c-115">Открывает записную книжку в собственном клиенте OneNote, если он установлен.</span><span class="sxs-lookup"><span data-stu-id="47d9c-115">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="47d9c-116">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="47d9c-116">oneNoteWebUrl</span></span>|[<span data-ttu-id="47d9c-117">externalLink</span><span class="sxs-lookup"><span data-stu-id="47d9c-117">externalLink</span></span>](externallink.md)|<span data-ttu-id="47d9c-118">Открывает записную книжку в OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="47d9c-118">Opens the notebook in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
