---
title: Тип ресурса Пажелинкс
description: Ссылки для открытия страницы OneNote.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 5224702d22d111b54d29db15da3c20923ccf7317
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035646"
---
# <a name="pagelinks-resource-type"></a><span data-ttu-id="35c6f-103">Тип ресурса Пажелинкс</span><span class="sxs-lookup"><span data-stu-id="35c6f-103">pageLinks resource type</span></span>

<span data-ttu-id="35c6f-104">Ссылки для открытия страницы OneNote.</span><span class="sxs-lookup"><span data-stu-id="35c6f-104">Links for opening a OneNote page.</span></span>

## <a name="json-representation"></a><span data-ttu-id="35c6f-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="35c6f-105">JSON representation</span></span>

<span data-ttu-id="35c6f-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="35c6f-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.pageLinks"
}-->

```json
{
  "oneNoteClientUrl": {"@odata.type": "microsoft.graph.externalLink"},
  "oneNoteWebUrl": {"@odata.type": "microsoft.graph.externalLink"}
}

```
## <a name="properties"></a><span data-ttu-id="35c6f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="35c6f-107">Properties</span></span>
| <span data-ttu-id="35c6f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="35c6f-108">Property</span></span>     | <span data-ttu-id="35c6f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="35c6f-109">Type</span></span>   |<span data-ttu-id="35c6f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="35c6f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="35c6f-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="35c6f-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="35c6f-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="35c6f-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="35c6f-113">Открывает страницу в собственном клиенте OneNote, если она установлена.</span><span class="sxs-lookup"><span data-stu-id="35c6f-113">Opens the page in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="35c6f-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="35c6f-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="35c6f-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="35c6f-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="35c6f-116">Открывает страницу в OneNote в Интернете.</span><span class="sxs-lookup"><span data-stu-id="35c6f-116">Opens the page in OneNote on the web.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "pageLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
