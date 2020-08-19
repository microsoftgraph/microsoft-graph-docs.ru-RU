---
title: Тип ресурса Пажелинкс
description: Ссылки для открытия страницы OneNote.
localization_priority: Normal
author: jewan-microsoft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e12dda3b2f2370cf7491809ca0554f341f17fa4d
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811877"
---
# <a name="pagelinks-resource-type"></a><span data-ttu-id="f9877-103">Тип ресурса Пажелинкс</span><span class="sxs-lookup"><span data-stu-id="f9877-103">pageLinks resource type</span></span>

<span data-ttu-id="f9877-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9877-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f9877-105">Ссылки для открытия страницы OneNote.</span><span class="sxs-lookup"><span data-stu-id="f9877-105">Links for opening a OneNote page.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f9877-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f9877-106">JSON representation</span></span>

<span data-ttu-id="f9877-107">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f9877-107">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="f9877-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f9877-108">Properties</span></span>
| <span data-ttu-id="f9877-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f9877-109">Property</span></span>     | <span data-ttu-id="f9877-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f9877-110">Type</span></span>   |<span data-ttu-id="f9877-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f9877-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f9877-112">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="f9877-112">oneNoteClientUrl</span></span>|[<span data-ttu-id="f9877-113">externalLink</span><span class="sxs-lookup"><span data-stu-id="f9877-113">externalLink</span></span>](externallink.md)|<span data-ttu-id="f9877-114">Открывает страницу в собственном клиенте OneNote, если она установлена.</span><span class="sxs-lookup"><span data-stu-id="f9877-114">Opens the page in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="f9877-115">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="f9877-115">oneNoteWebUrl</span></span>|[<span data-ttu-id="f9877-116">externalLink</span><span class="sxs-lookup"><span data-stu-id="f9877-116">externalLink</span></span>](externallink.md)|<span data-ttu-id="f9877-117">Открывает страницу в OneNote в Интернете.</span><span class="sxs-lookup"><span data-stu-id="f9877-117">Opens the page in OneNote on the web.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "pageLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
