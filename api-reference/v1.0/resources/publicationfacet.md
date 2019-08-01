---
title: Тип ресурса publicationFacet
description: Ресурс **publicationFacet** содержит сведения о состоянии публикации ресурса driveItemVersion или driveItem.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 5189b578d0a996ceb27014d2c5400e508e1e8a56
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034953"
---
# <a name="publicationfacet-resource-type"></a><span data-ttu-id="a175c-103">Тип ресурса publicationFacet</span><span class="sxs-lookup"><span data-stu-id="a175c-103">PublicationFacet resource type</span></span>

<span data-ttu-id="a175c-104">Ресурс **publicationFacet** содержит сведения о состоянии публикации ресурса [driveItemVersion](driveitemversion.md) или [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="a175c-104">The **publicationFacet** resource provides details on the published status of a [driveItemVersion](driveitemversion.md) or [driveItem](driveitem.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a175c-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a175c-105">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.publicationFacet"
}-->

```json
{
  "level": "published | checkout",
  "versionId": "string"
}
```

## <a name="properties"></a><span data-ttu-id="a175c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a175c-106">Properties</span></span>

|   <span data-ttu-id="a175c-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a175c-107">Property</span></span>    |  <span data-ttu-id="a175c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a175c-108">Type</span></span>  | <span data-ttu-id="a175c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a175c-109">Description</span></span> |
| :------------ | :----- | :---------- |
| <span data-ttu-id="a175c-110">**level**</span><span class="sxs-lookup"><span data-stu-id="a175c-110">**level**</span></span>     | <span data-ttu-id="a175c-111">String</span><span class="sxs-lookup"><span data-stu-id="a175c-111">String</span></span> | <span data-ttu-id="a175c-112">Состояние публикации для данного документа.</span><span class="sxs-lookup"><span data-stu-id="a175c-112">The state of publication for this document.</span></span> <span data-ttu-id="a175c-113">Возможные значения: `published` или `checkout`.</span><span class="sxs-lookup"><span data-stu-id="a175c-113">Either `published` or `checkout`.</span></span> <span data-ttu-id="a175c-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a175c-114">Read-only.</span></span>  |
| <span data-ttu-id="a175c-115">**versionId**</span><span class="sxs-lookup"><span data-stu-id="a175c-115">**versionId**</span></span> | <span data-ttu-id="a175c-116">String</span><span class="sxs-lookup"><span data-stu-id="a175c-116">String</span></span> | <span data-ttu-id="a175c-117">Уникальный идентификатор для версии, отображаемый для текущего вызывающего объекта.</span><span class="sxs-lookup"><span data-stu-id="a175c-117">The unique identifier for the version that is visible to the current caller.</span></span> <span data-ttu-id="a175c-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a175c-118">Read-only.</span></span>  |


<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "suppressions": [
    " Warning: /api-reference/v1.0/resources/publicationfacet.md:
      Found potential enums in resource example that weren't defined in a table:(published,checkout) are in resource, but () are in table"
  ],
  "tocPath": "Facets/Photo"
} -->
