---
title: Тип ресурса Сектионлинкс
description: Ссылки для открытия раздела OneNote.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 0e84f6d071423159918479bdb1836855fed113a6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520873"
---
# <a name="sectionlinks-resource-type"></a><span data-ttu-id="03dfc-103">Тип ресурса Сектионлинкс</span><span class="sxs-lookup"><span data-stu-id="03dfc-103">sectionLinks resource type</span></span>

<span data-ttu-id="03dfc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03dfc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03dfc-105">Ссылки для открытия раздела OneNote.</span><span class="sxs-lookup"><span data-stu-id="03dfc-105">Links for opening a OneNote section.</span></span>

## <a name="json-representation"></a><span data-ttu-id="03dfc-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="03dfc-106">JSON representation</span></span>

<span data-ttu-id="03dfc-107">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="03dfc-107">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="03dfc-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="03dfc-108">Properties</span></span>
| <span data-ttu-id="03dfc-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="03dfc-109">Property</span></span>     | <span data-ttu-id="03dfc-110">Тип</span><span class="sxs-lookup"><span data-stu-id="03dfc-110">Type</span></span>   |<span data-ttu-id="03dfc-111">Описание</span><span class="sxs-lookup"><span data-stu-id="03dfc-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="03dfc-112">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="03dfc-112">oneNoteClientUrl</span></span>|[<span data-ttu-id="03dfc-113">externalLink</span><span class="sxs-lookup"><span data-stu-id="03dfc-113">externalLink</span></span>](externallink.md)|<span data-ttu-id="03dfc-114">Открывает раздел в собственном клиенте OneNote, если он установлен.</span><span class="sxs-lookup"><span data-stu-id="03dfc-114">Opens the section in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="03dfc-115">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="03dfc-115">oneNoteWebUrl</span></span>|[<span data-ttu-id="03dfc-116">externalLink</span><span class="sxs-lookup"><span data-stu-id="03dfc-116">externalLink</span></span>](externallink.md)|<span data-ttu-id="03dfc-117">Открывает раздел в OneNote в Интернете.</span><span class="sxs-lookup"><span data-stu-id="03dfc-117">Opens the section in OneNote on the web.</span></span>|

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
