---
author: JeremyKelley
description: Ресурс publicationFacet содержит сведения о состоянии публикации ресурса driveItemVersion или driveItem.
ms.date: 09/10/2017
title: PublicationFacet
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 9c09f0863376e1569fb4af0acc0044fa1c7c8cfa
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008861"
---
# <a name="publicationfacet-resource-type"></a><span data-ttu-id="b918b-103">Тип ресурса publicationFacet</span><span class="sxs-lookup"><span data-stu-id="b918b-103">PublicationFacet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b918b-104">Ресурс **publicationFacet** содержит сведения о состоянии публикации ресурса [driveItemVersion](driveitemversion.md) или [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="b918b-104">The **publicationFacet** resource provides details on the published status of a [driveItemVersion](driveitemversion.md) or [driveItem](driveitem.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b918b-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b918b-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="b918b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b918b-106">Properties</span></span>

|   <span data-ttu-id="b918b-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b918b-107">Property</span></span>    |  <span data-ttu-id="b918b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b918b-108">Type</span></span>  | <span data-ttu-id="b918b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b918b-109">Description</span></span> |
| :------------ | :----- | :---------- |
| <span data-ttu-id="b918b-110">**level**</span><span class="sxs-lookup"><span data-stu-id="b918b-110">**level**</span></span>     | <span data-ttu-id="b918b-111">String</span><span class="sxs-lookup"><span data-stu-id="b918b-111">String</span></span> | <span data-ttu-id="b918b-112">Состояние публикации для данного документа.</span><span class="sxs-lookup"><span data-stu-id="b918b-112">The state of publication for this document.</span></span> <span data-ttu-id="b918b-113">Возможные значения: `published` или `checkout`.</span><span class="sxs-lookup"><span data-stu-id="b918b-113">Either `published` or `checkout`.</span></span> <span data-ttu-id="b918b-114">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b918b-114">Read-only.</span></span>  |
| <span data-ttu-id="b918b-115">**versionId**</span><span class="sxs-lookup"><span data-stu-id="b918b-115">**versionId**</span></span> | <span data-ttu-id="b918b-116">String</span><span class="sxs-lookup"><span data-stu-id="b918b-116">String</span></span> | <span data-ttu-id="b918b-117">Уникальный идентификатор для версии, отображаемый для текущего вызывающего объекта.</span><span class="sxs-lookup"><span data-stu-id="b918b-117">The unique identifier for the version that is visible to the current caller.</span></span> <span data-ttu-id="b918b-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b918b-118">Read-only.</span></span>  |


<!--
{
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo",
  "suppressions": []
}
-->
