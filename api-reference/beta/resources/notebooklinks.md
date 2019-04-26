---
title: Тип ресурса Нотебуклинкс
description: Ссылки для открытия записной книжки OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: b9ea408c869c5ad8fb546b6ea9548f3fc7c33b63
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342154"
---
# <a name="notebooklinks-resource-type"></a><span data-ttu-id="02f46-103">Тип ресурса Нотебуклинкс</span><span class="sxs-lookup"><span data-stu-id="02f46-103">notebookLinks resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02f46-104">Ссылки для открытия записной книжки OneNote.</span><span class="sxs-lookup"><span data-stu-id="02f46-104">Links for opening a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="02f46-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="02f46-105">JSON representation</span></span>

<span data-ttu-id="02f46-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="02f46-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="02f46-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="02f46-107">Properties</span></span>
| <span data-ttu-id="02f46-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="02f46-108">Property</span></span>     | <span data-ttu-id="02f46-109">Тип</span><span class="sxs-lookup"><span data-stu-id="02f46-109">Type</span></span>   |<span data-ttu-id="02f46-110">Описание</span><span class="sxs-lookup"><span data-stu-id="02f46-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="02f46-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="02f46-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="02f46-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="02f46-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="02f46-113">Открывает записную книжку в собственном клиенте OneNote, если он установлен.</span><span class="sxs-lookup"><span data-stu-id="02f46-113">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="02f46-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="02f46-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="02f46-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="02f46-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="02f46-116">Открывает записную книжку в OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="02f46-116">Opens the notebook in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "notebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
