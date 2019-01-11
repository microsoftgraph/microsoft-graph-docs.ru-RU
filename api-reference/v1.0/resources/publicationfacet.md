---
title: Тип ресурса publicationFacet
description: Ресурс **publicationFacet** содержит сведения о состоянии публикации ресурса driveItemVersion или driveItem.
localization_priority: Normal
ms.openlocfilehash: 3d722f56cf1d587483c672fb7a1b7c05abd3671b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810531"
---
# <a name="publicationfacet-resource-type"></a><span data-ttu-id="6e00c-103">Тип ресурса publicationFacet</span><span class="sxs-lookup"><span data-stu-id="6e00c-103">PublicationFacet resource type</span></span>

<span data-ttu-id="6e00c-104">Ресурс **publicationFacet** содержит сведения о состоянии публикации ресурса [driveItemVersion](driveitemversion.md) или [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="6e00c-104">The **publicationFacet** resource provides details on the published status of a [driveItemVersion](driveitemversion.md) or [driveItem](driveitem.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6e00c-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="6e00c-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="6e00c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="6e00c-106">Properties</span></span>

|   <span data-ttu-id="6e00c-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="6e00c-107">Property</span></span>    |  <span data-ttu-id="6e00c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="6e00c-108">Type</span></span>  | <span data-ttu-id="6e00c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6e00c-109">Description</span></span> |
| :------------ | :----- | :---------- |
| <span data-ttu-id="6e00c-110">**level**</span><span class="sxs-lookup"><span data-stu-id="6e00c-110">**level**</span></span>     | <span data-ttu-id="6e00c-111">String</span><span class="sxs-lookup"><span data-stu-id="6e00c-111">String</span></span> | <span data-ttu-id="6e00c-112">Состояние публикации для данного документа.</span><span class="sxs-lookup"><span data-stu-id="6e00c-112">The state of publication for this document.</span></span> <span data-ttu-id="6e00c-113">Возможные значения: `published` или `checkout`.</span><span class="sxs-lookup"><span data-stu-id="6e00c-113">Either `published` or `checkout`.</span></span> <span data-ttu-id="6e00c-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6e00c-114">Read-only.</span></span>  |
| <span data-ttu-id="6e00c-115">**versionId**</span><span class="sxs-lookup"><span data-stu-id="6e00c-115">**versionId**</span></span> | <span data-ttu-id="6e00c-116">String</span><span class="sxs-lookup"><span data-stu-id="6e00c-116">String</span></span> | <span data-ttu-id="6e00c-117">Уникальный идентификатор для версии, отображаемый для текущего вызывающего объекта.</span><span class="sxs-lookup"><span data-stu-id="6e00c-117">The unique identifier for the version that is visible to the current caller.</span></span> <span data-ttu-id="6e00c-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6e00c-118">Read-only.</span></span>  |


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
