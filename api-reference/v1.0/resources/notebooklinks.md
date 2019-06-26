---
title: Тип ресурса Нотебуклинкс
description: Ссылки для открытия записной книжки OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 376000d84ccec8cdc0c1ae601e65f3217275b1e4
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2019
ms.locfileid: "35236624"
---
# <a name="notebooklinks-resource-type"></a><span data-ttu-id="9b96a-103">Тип ресурса Нотебуклинкс</span><span class="sxs-lookup"><span data-stu-id="9b96a-103">notebookLinks resource type</span></span>

<span data-ttu-id="9b96a-104">Ссылки для открытия записной книжки OneNote.</span><span class="sxs-lookup"><span data-stu-id="9b96a-104">Links for opening a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9b96a-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9b96a-105">JSON representation</span></span>

<span data-ttu-id="9b96a-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9b96a-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="9b96a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="9b96a-107">Properties</span></span>
| <span data-ttu-id="9b96a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="9b96a-108">Property</span></span>     | <span data-ttu-id="9b96a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="9b96a-109">Type</span></span>   |<span data-ttu-id="9b96a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9b96a-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9b96a-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="9b96a-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="9b96a-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="9b96a-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="9b96a-113">Открывает записную книжку в собственном клиенте OneNote, если он установлен.</span><span class="sxs-lookup"><span data-stu-id="9b96a-113">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="9b96a-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="9b96a-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="9b96a-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="9b96a-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="9b96a-116">Открывает записную книжку в OneNote в Интернете.</span><span class="sxs-lookup"><span data-stu-id="9b96a-116">Opens the notebook in OneNote on the web.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
