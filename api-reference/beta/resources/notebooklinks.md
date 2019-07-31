---
title: Тип ресурса Нотебуклинкс
description: Ссылки для открытия записной книжки OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 866176f1c831c70b7a057d1a53ad6b5fa7e5cda4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966659"
---
# <a name="notebooklinks-resource-type"></a><span data-ttu-id="ad02f-103">Тип ресурса Нотебуклинкс</span><span class="sxs-lookup"><span data-stu-id="ad02f-103">notebookLinks resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad02f-104">Ссылки для открытия записной книжки OneNote.</span><span class="sxs-lookup"><span data-stu-id="ad02f-104">Links for opening a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ad02f-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ad02f-105">JSON representation</span></span>

<span data-ttu-id="ad02f-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ad02f-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="ad02f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ad02f-107">Properties</span></span>
| <span data-ttu-id="ad02f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ad02f-108">Property</span></span>     | <span data-ttu-id="ad02f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ad02f-109">Type</span></span>   |<span data-ttu-id="ad02f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ad02f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ad02f-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="ad02f-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="ad02f-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="ad02f-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="ad02f-113">Открывает записную книжку в собственном клиенте OneNote, если он установлен.</span><span class="sxs-lookup"><span data-stu-id="ad02f-113">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="ad02f-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="ad02f-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="ad02f-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="ad02f-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="ad02f-116">Открывает записную книжку в OneNote в Интернете.</span><span class="sxs-lookup"><span data-stu-id="ad02f-116">Opens the notebook in OneNote on the web.</span></span>|

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
