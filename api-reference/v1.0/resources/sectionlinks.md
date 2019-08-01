---
title: Тип ресурса Сектионлинкс
description: Ссылки для открытия раздела OneNote.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 76a79c6f2fa148e492d5ded3295364efcb0d1a32
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034540"
---
# <a name="sectionlinks-resource-type"></a><span data-ttu-id="05ea0-103">Тип ресурса Сектионлинкс</span><span class="sxs-lookup"><span data-stu-id="05ea0-103">sectionLinks resource type</span></span>

<span data-ttu-id="05ea0-104">Ссылки для открытия раздела OneNote.</span><span class="sxs-lookup"><span data-stu-id="05ea0-104">Links for opening a OneNote section.</span></span>

## <a name="json-representation"></a><span data-ttu-id="05ea0-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="05ea0-105">JSON representation</span></span>

<span data-ttu-id="05ea0-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="05ea0-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.sectionLinks"
}-->

```json
{
  "oneNoteClientUrl": {"@odata.type": "microsoft.graph.externalLink"},
  "oneNoteWebUrl": {"@odata.type": "microsoft.graph.externalLink"}
}

```
## <a name="properties"></a><span data-ttu-id="05ea0-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="05ea0-107">Properties</span></span>
| <span data-ttu-id="05ea0-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="05ea0-108">Property</span></span>     | <span data-ttu-id="05ea0-109">Тип</span><span class="sxs-lookup"><span data-stu-id="05ea0-109">Type</span></span>   |<span data-ttu-id="05ea0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="05ea0-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="05ea0-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="05ea0-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="05ea0-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="05ea0-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="05ea0-113">Открывает раздел в собственном клиенте OneNote, если он установлен.</span><span class="sxs-lookup"><span data-stu-id="05ea0-113">Opens the section in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="05ea0-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="05ea0-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="05ea0-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="05ea0-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="05ea0-116">Открывает раздел в OneNote в Интернете.</span><span class="sxs-lookup"><span data-stu-id="05ea0-116">Opens the section in OneNote on the web.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sectionLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
