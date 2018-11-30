---
title: Тип ресурса publicationFacet
description: Ресурс **publicationFacet** содержит сведения о состоянии публикации ресурса driveItemVersion или driveItem.
ms.openlocfilehash: 429ec649dc9f511a4012e6790842fdd774bead8b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024969"
---
# <a name="publicationfacet-resource-type"></a><span data-ttu-id="78079-103">Тип ресурса publicationFacet</span><span class="sxs-lookup"><span data-stu-id="78079-103">PublicationFacet resource type</span></span>

<span data-ttu-id="78079-104">Ресурс **publicationFacet** содержит сведения о состоянии публикации ресурса [driveItemVersion](driveitemversion.md) или [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="78079-104">The **publicationFacet** resource provides details on the published status of a [driveItemVersion](driveitemversion.md) or [driveItem](driveitem.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="78079-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="78079-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="78079-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="78079-106">Properties</span></span>

|   <span data-ttu-id="78079-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="78079-107">Property</span></span>    |  <span data-ttu-id="78079-108">Тип</span><span class="sxs-lookup"><span data-stu-id="78079-108">Type</span></span>  | <span data-ttu-id="78079-109">Описание</span><span class="sxs-lookup"><span data-stu-id="78079-109">Description</span></span> |
| :------------ | :----- | :---------- |
| <span data-ttu-id="78079-110">**level**</span><span class="sxs-lookup"><span data-stu-id="78079-110">**level**</span></span>     | <span data-ttu-id="78079-111">String</span><span class="sxs-lookup"><span data-stu-id="78079-111">String</span></span> | <span data-ttu-id="78079-112">Состояние публикации для данного документа.</span><span class="sxs-lookup"><span data-stu-id="78079-112">The state of publication for this document.</span></span> <span data-ttu-id="78079-113">Возможные значения: `published` или `checkout`.</span><span class="sxs-lookup"><span data-stu-id="78079-113">Either `published` or `checkout`.</span></span> <span data-ttu-id="78079-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="78079-114">Read-only.</span></span>  |
| <span data-ttu-id="78079-115">**versionId**</span><span class="sxs-lookup"><span data-stu-id="78079-115">**versionId**</span></span> | <span data-ttu-id="78079-116">String</span><span class="sxs-lookup"><span data-stu-id="78079-116">String</span></span> | <span data-ttu-id="78079-117">Уникальный идентификатор для версии, отображаемый для текущего вызывающего объекта.</span><span class="sxs-lookup"><span data-stu-id="78079-117">The unique identifier for the version that is visible to the current caller.</span></span> <span data-ttu-id="78079-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="78079-118">Read-only.</span></span>  |


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
