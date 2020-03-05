---
title: Тип ресурса publicationFacet
description: Ресурс **publicationFacet** содержит сведения о состоянии публикации ресурса driveItemVersion или driveItem.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: defd2c9b06a0d866ce43bbd4a9e8b36bdad770fb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447040"
---
# <a name="publicationfacet-resource-type"></a><span data-ttu-id="3b3a0-103">Тип ресурса publicationFacet</span><span class="sxs-lookup"><span data-stu-id="3b3a0-103">PublicationFacet resource type</span></span>

<span data-ttu-id="3b3a0-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3b3a0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3b3a0-105">Ресурс **publicationFacet** содержит сведения о состоянии публикации ресурса [driveItemVersion](driveitemversion.md) или [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="3b3a0-105">The **publicationFacet** resource provides details on the published status of a [driveItemVersion](driveitemversion.md) or [driveItem](driveitem.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3b3a0-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3b3a0-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="3b3a0-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="3b3a0-107">Properties</span></span>

|   <span data-ttu-id="3b3a0-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="3b3a0-108">Property</span></span>    |  <span data-ttu-id="3b3a0-109">Тип</span><span class="sxs-lookup"><span data-stu-id="3b3a0-109">Type</span></span>  | <span data-ttu-id="3b3a0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3b3a0-110">Description</span></span> |
| :------------ | :----- | :---------- |
| <span data-ttu-id="3b3a0-111">**level**</span><span class="sxs-lookup"><span data-stu-id="3b3a0-111">**level**</span></span>     | <span data-ttu-id="3b3a0-112">String</span><span class="sxs-lookup"><span data-stu-id="3b3a0-112">String</span></span> | <span data-ttu-id="3b3a0-113">Состояние публикации для данного документа.</span><span class="sxs-lookup"><span data-stu-id="3b3a0-113">The state of publication for this document.</span></span> <span data-ttu-id="3b3a0-114">Возможные значения: `published` или `checkout`.</span><span class="sxs-lookup"><span data-stu-id="3b3a0-114">Either `published` or `checkout`.</span></span> <span data-ttu-id="3b3a0-115">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3b3a0-115">Read-only.</span></span>  |
| <span data-ttu-id="3b3a0-116">**versionId**</span><span class="sxs-lookup"><span data-stu-id="3b3a0-116">**versionId**</span></span> | <span data-ttu-id="3b3a0-117">String</span><span class="sxs-lookup"><span data-stu-id="3b3a0-117">String</span></span> | <span data-ttu-id="3b3a0-118">Уникальный идентификатор для версии, отображаемый для текущего вызывающего объекта.</span><span class="sxs-lookup"><span data-stu-id="3b3a0-118">The unique identifier for the version that is visible to the current caller.</span></span> <span data-ttu-id="3b3a0-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3b3a0-119">Read-only.</span></span>  |


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
