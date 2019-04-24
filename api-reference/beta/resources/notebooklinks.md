---
title: Тип ресурса Нотебуклинкс
description: Ссылки для открытия записной книжки OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: f6995c112410d22cfe5849f54d0077bf8b79f6b3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463287"
---
# <a name="notebooklinks-resource-type"></a><span data-ttu-id="10368-103">Тип ресурса Нотебуклинкс</span><span class="sxs-lookup"><span data-stu-id="10368-103">notebookLinks resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10368-104">Ссылки для открытия записной книжки OneNote.</span><span class="sxs-lookup"><span data-stu-id="10368-104">Links for opening a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="10368-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="10368-105">JSON representation</span></span>

<span data-ttu-id="10368-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="10368-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="10368-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="10368-107">Properties</span></span>
| <span data-ttu-id="10368-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="10368-108">Property</span></span>     | <span data-ttu-id="10368-109">Тип</span><span class="sxs-lookup"><span data-stu-id="10368-109">Type</span></span>   |<span data-ttu-id="10368-110">Описание</span><span class="sxs-lookup"><span data-stu-id="10368-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="10368-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="10368-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="10368-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="10368-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="10368-113">Открывает записную книжку в собственном клиенте OneNote, если он установлен.</span><span class="sxs-lookup"><span data-stu-id="10368-113">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="10368-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="10368-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="10368-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="10368-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="10368-116">Открывает записную книжку в OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="10368-116">Opens the notebook in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "notebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/notebooklinks.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
