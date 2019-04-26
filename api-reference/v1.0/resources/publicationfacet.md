---
title: Тип ресурса publicationFacet
description: Ресурс **publicationFacet** содержит сведения о состоянии публикации ресурса driveItemVersion или driveItem.
localization_priority: Normal
ms.openlocfilehash: 3d722f56cf1d587483c672fb7a1b7c05abd3671b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579701"
---
# <a name="publicationfacet-resource-type"></a><span data-ttu-id="95e31-103">Тип ресурса publicationFacet</span><span class="sxs-lookup"><span data-stu-id="95e31-103">PublicationFacet resource type</span></span>

<span data-ttu-id="95e31-104">Ресурс **publicationFacet** содержит сведения о состоянии публикации ресурса [driveItemVersion](driveitemversion.md) или [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="95e31-104">The **publicationFacet** resource provides details on the published status of a [driveItemVersion](driveitemversion.md) or [driveItem](driveitem.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="95e31-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="95e31-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="95e31-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="95e31-106">Properties</span></span>

|   <span data-ttu-id="95e31-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="95e31-107">Property</span></span>    |  <span data-ttu-id="95e31-108">Тип</span><span class="sxs-lookup"><span data-stu-id="95e31-108">Type</span></span>  | <span data-ttu-id="95e31-109">Описание</span><span class="sxs-lookup"><span data-stu-id="95e31-109">Description</span></span> |
| :------------ | :----- | :---------- |
| <span data-ttu-id="95e31-110">**level**</span><span class="sxs-lookup"><span data-stu-id="95e31-110">**level**</span></span>     | <span data-ttu-id="95e31-111">String</span><span class="sxs-lookup"><span data-stu-id="95e31-111">String</span></span> | <span data-ttu-id="95e31-112">Состояние публикации для данного документа.</span><span class="sxs-lookup"><span data-stu-id="95e31-112">The state of publication for this document.</span></span> <span data-ttu-id="95e31-113">Возможные значения: `published` или `checkout`.</span><span class="sxs-lookup"><span data-stu-id="95e31-113">Either `published` or `checkout`.</span></span> <span data-ttu-id="95e31-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="95e31-114">Read-only.</span></span>  |
| <span data-ttu-id="95e31-115">**versionId**</span><span class="sxs-lookup"><span data-stu-id="95e31-115">**versionId**</span></span> | <span data-ttu-id="95e31-116">String</span><span class="sxs-lookup"><span data-stu-id="95e31-116">String</span></span> | <span data-ttu-id="95e31-117">Уникальный идентификатор для версии, отображаемый для текущего вызывающего объекта.</span><span class="sxs-lookup"><span data-stu-id="95e31-117">The unique identifier for the version that is visible to the current caller.</span></span> <span data-ttu-id="95e31-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="95e31-118">Read-only.</span></span>  |


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
