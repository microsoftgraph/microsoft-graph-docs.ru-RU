---
title: Тип ресурса Сектионлинкс
description: Ссылки для открытия раздела OneNote.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c4fecff18c2271da383a03002e38eed4bf42aa93
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533780"
---
# <a name="sectionlinks-resource-type"></a><span data-ttu-id="ea12a-103">Тип ресурса Сектионлинкс</span><span class="sxs-lookup"><span data-stu-id="ea12a-103">sectionLinks resource type</span></span>

<span data-ttu-id="ea12a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea12a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ea12a-105">Ссылки для открытия раздела OneNote.</span><span class="sxs-lookup"><span data-stu-id="ea12a-105">Links for opening a OneNote section.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ea12a-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ea12a-106">JSON representation</span></span>

<span data-ttu-id="ea12a-107">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ea12a-107">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="ea12a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ea12a-108">Properties</span></span>
| <span data-ttu-id="ea12a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ea12a-109">Property</span></span>     | <span data-ttu-id="ea12a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ea12a-110">Type</span></span>   |<span data-ttu-id="ea12a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ea12a-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ea12a-112">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="ea12a-112">oneNoteClientUrl</span></span>|[<span data-ttu-id="ea12a-113">externalLink</span><span class="sxs-lookup"><span data-stu-id="ea12a-113">externalLink</span></span>](externallink.md)|<span data-ttu-id="ea12a-114">Открывает раздел в собственном клиенте OneNote, если он установлен.</span><span class="sxs-lookup"><span data-stu-id="ea12a-114">Opens the section in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="ea12a-115">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="ea12a-115">oneNoteWebUrl</span></span>|[<span data-ttu-id="ea12a-116">externalLink</span><span class="sxs-lookup"><span data-stu-id="ea12a-116">externalLink</span></span>](externallink.md)|<span data-ttu-id="ea12a-117">Открывает раздел в OneNote в Интернете.</span><span class="sxs-lookup"><span data-stu-id="ea12a-117">Opens the section in OneNote on the web.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sectionLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
