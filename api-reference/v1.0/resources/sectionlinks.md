---
title: Тип ресурса Сектионлинкс
description: Ссылки для открытия раздела OneNote.
localization_priority: Normal
author: jewan-microsoft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 2c0bf1090f3d60388819b871b88ef8d34aa77d82
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812185"
---
# <a name="sectionlinks-resource-type"></a><span data-ttu-id="db07f-103">Тип ресурса Сектионлинкс</span><span class="sxs-lookup"><span data-stu-id="db07f-103">sectionLinks resource type</span></span>

<span data-ttu-id="db07f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db07f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="db07f-105">Ссылки для открытия раздела OneNote.</span><span class="sxs-lookup"><span data-stu-id="db07f-105">Links for opening a OneNote section.</span></span>

## <a name="json-representation"></a><span data-ttu-id="db07f-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="db07f-106">JSON representation</span></span>

<span data-ttu-id="db07f-107">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="db07f-107">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="db07f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="db07f-108">Properties</span></span>
| <span data-ttu-id="db07f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="db07f-109">Property</span></span>     | <span data-ttu-id="db07f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="db07f-110">Type</span></span>   |<span data-ttu-id="db07f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="db07f-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="db07f-112">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="db07f-112">oneNoteClientUrl</span></span>|[<span data-ttu-id="db07f-113">externalLink</span><span class="sxs-lookup"><span data-stu-id="db07f-113">externalLink</span></span>](externallink.md)|<span data-ttu-id="db07f-114">Открывает раздел в собственном клиенте OneNote, если он установлен.</span><span class="sxs-lookup"><span data-stu-id="db07f-114">Opens the section in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="db07f-115">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="db07f-115">oneNoteWebUrl</span></span>|[<span data-ttu-id="db07f-116">externalLink</span><span class="sxs-lookup"><span data-stu-id="db07f-116">externalLink</span></span>](externallink.md)|<span data-ttu-id="db07f-117">Открывает раздел в OneNote в Интернете.</span><span class="sxs-lookup"><span data-stu-id="db07f-117">Opens the section in OneNote on the web.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sectionLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
