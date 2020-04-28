---
title: Тип ресурса Пажелинкс
description: Ссылки для открытия страницы OneNote.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 27f4c45a9ea2747d5ca5748184b84e4fabb54f55
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522055"
---
# <a name="pagelinks-resource-type"></a><span data-ttu-id="372bf-103">Тип ресурса Пажелинкс</span><span class="sxs-lookup"><span data-stu-id="372bf-103">pageLinks resource type</span></span>

<span data-ttu-id="372bf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="372bf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="372bf-105">Ссылки для открытия страницы OneNote.</span><span class="sxs-lookup"><span data-stu-id="372bf-105">Links for opening a OneNote page.</span></span>

## <a name="json-representation"></a><span data-ttu-id="372bf-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="372bf-106">JSON representation</span></span>

<span data-ttu-id="372bf-107">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="372bf-107">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="372bf-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="372bf-108">Properties</span></span>
| <span data-ttu-id="372bf-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="372bf-109">Property</span></span>     | <span data-ttu-id="372bf-110">Тип</span><span class="sxs-lookup"><span data-stu-id="372bf-110">Type</span></span>   |<span data-ttu-id="372bf-111">Описание</span><span class="sxs-lookup"><span data-stu-id="372bf-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="372bf-112">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="372bf-112">oneNoteClientUrl</span></span>|[<span data-ttu-id="372bf-113">externalLink</span><span class="sxs-lookup"><span data-stu-id="372bf-113">externalLink</span></span>](externallink.md)|<span data-ttu-id="372bf-114">Открывает страницу в собственном клиенте OneNote, если она установлена.</span><span class="sxs-lookup"><span data-stu-id="372bf-114">Opens the page in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="372bf-115">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="372bf-115">oneNoteWebUrl</span></span>|[<span data-ttu-id="372bf-116">externalLink</span><span class="sxs-lookup"><span data-stu-id="372bf-116">externalLink</span></span>](externallink.md)|<span data-ttu-id="372bf-117">Открывает страницу в OneNote в Интернете.</span><span class="sxs-lookup"><span data-stu-id="372bf-117">Opens the page in OneNote on the web.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "pageLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
