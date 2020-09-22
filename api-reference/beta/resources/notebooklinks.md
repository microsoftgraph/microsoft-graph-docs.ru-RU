---
title: Тип ресурса Нотебуклинкс
description: Ссылки для открытия записной книжки OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: b0050463ec3b88bd32e69efa6cfde5189fdce8d5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033673"
---
# <a name="notebooklinks-resource-type"></a><span data-ttu-id="7f499-103">Тип ресурса Нотебуклинкс</span><span class="sxs-lookup"><span data-stu-id="7f499-103">notebookLinks resource type</span></span>

<span data-ttu-id="7f499-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f499-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f499-105">Ссылки для открытия записной книжки OneNote.</span><span class="sxs-lookup"><span data-stu-id="7f499-105">Links for opening a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7f499-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7f499-106">JSON representation</span></span>

<span data-ttu-id="7f499-107">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7f499-107">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="7f499-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="7f499-108">Properties</span></span>
| <span data-ttu-id="7f499-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="7f499-109">Property</span></span>     | <span data-ttu-id="7f499-110">Тип</span><span class="sxs-lookup"><span data-stu-id="7f499-110">Type</span></span>   |<span data-ttu-id="7f499-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7f499-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7f499-112">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="7f499-112">oneNoteClientUrl</span></span>|[<span data-ttu-id="7f499-113">externalLink</span><span class="sxs-lookup"><span data-stu-id="7f499-113">externalLink</span></span>](externallink.md)|<span data-ttu-id="7f499-114">Открывает записную книжку в собственном клиенте OneNote, если он установлен.</span><span class="sxs-lookup"><span data-stu-id="7f499-114">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="7f499-115">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="7f499-115">oneNoteWebUrl</span></span>|[<span data-ttu-id="7f499-116">externalLink</span><span class="sxs-lookup"><span data-stu-id="7f499-116">externalLink</span></span>](externallink.md)|<span data-ttu-id="7f499-117">Открывает записную книжку в OneNote в Интернете.</span><span class="sxs-lookup"><span data-stu-id="7f499-117">Opens the notebook in OneNote on the web.</span></span>|

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


