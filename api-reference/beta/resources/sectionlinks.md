---
title: Тип ресурса Сектионлинкс
description: Ссылки для открытия раздела OneNote.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 270cc08f797546f08dbb89c4137631dd30cc4ae0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008595"
---
# <a name="sectionlinks-resource-type"></a><span data-ttu-id="5597f-103">Тип ресурса Сектионлинкс</span><span class="sxs-lookup"><span data-stu-id="5597f-103">sectionLinks resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5597f-104">Ссылки для открытия раздела OneNote.</span><span class="sxs-lookup"><span data-stu-id="5597f-104">Links for opening a OneNote section.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5597f-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5597f-105">JSON representation</span></span>

<span data-ttu-id="5597f-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5597f-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="5597f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5597f-107">Properties</span></span>
| <span data-ttu-id="5597f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="5597f-108">Property</span></span>     | <span data-ttu-id="5597f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5597f-109">Type</span></span>   |<span data-ttu-id="5597f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5597f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5597f-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="5597f-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="5597f-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="5597f-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="5597f-113">Открывает раздел в собственном клиенте OneNote, если он установлен.</span><span class="sxs-lookup"><span data-stu-id="5597f-113">Opens the section in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="5597f-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="5597f-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="5597f-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="5597f-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="5597f-116">Открывает раздел в OneNote в Интернете.</span><span class="sxs-lookup"><span data-stu-id="5597f-116">Opens the section in OneNote on the web.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "sectionLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
