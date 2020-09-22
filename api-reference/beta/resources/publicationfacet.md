---
author: JeremyKelley
description: Ресурс publicationFacet содержит сведения о состоянии публикации ресурса driveItemVersion или driveItem.
ms.date: 09/10/2017
title: PublicationFacet
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 3df98fd151e8ca528a0a946a273ff6e64eb54a8e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993093"
---
# <a name="publicationfacet-resource-type"></a><span data-ttu-id="e222e-103">Тип ресурса publicationFacet</span><span class="sxs-lookup"><span data-stu-id="e222e-103">PublicationFacet resource type</span></span>

<span data-ttu-id="e222e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e222e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e222e-105">Ресурс **publicationFacet** содержит сведения о состоянии публикации ресурса [driveItemVersion](driveitemversion.md) или [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="e222e-105">The **publicationFacet** resource provides details on the published status of a [driveItemVersion](driveitemversion.md) or [driveItem](driveitem.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e222e-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e222e-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="e222e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e222e-107">Properties</span></span>

|   <span data-ttu-id="e222e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e222e-108">Property</span></span>    |  <span data-ttu-id="e222e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e222e-109">Type</span></span>  | <span data-ttu-id="e222e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e222e-110">Description</span></span> |
| :------------ | :----- | :---------- |
| <span data-ttu-id="e222e-111">**level**</span><span class="sxs-lookup"><span data-stu-id="e222e-111">**level**</span></span>     | <span data-ttu-id="e222e-112">String</span><span class="sxs-lookup"><span data-stu-id="e222e-112">String</span></span> | <span data-ttu-id="e222e-113">Состояние публикации для данного документа.</span><span class="sxs-lookup"><span data-stu-id="e222e-113">The state of publication for this document.</span></span> <span data-ttu-id="e222e-114">Возможные значения: `published` или `checkout`.</span><span class="sxs-lookup"><span data-stu-id="e222e-114">Either `published` or `checkout`.</span></span> <span data-ttu-id="e222e-115">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e222e-115">Read-only.</span></span>  |
| <span data-ttu-id="e222e-116">**versionId**</span><span class="sxs-lookup"><span data-stu-id="e222e-116">**versionId**</span></span> | <span data-ttu-id="e222e-117">String</span><span class="sxs-lookup"><span data-stu-id="e222e-117">String</span></span> | <span data-ttu-id="e222e-118">Уникальный идентификатор для версии, отображаемый для текущего вызывающего объекта.</span><span class="sxs-lookup"><span data-stu-id="e222e-118">The unique identifier for the version that is visible to the current caller.</span></span> <span data-ttu-id="e222e-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e222e-119">Read-only.</span></span>  |


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


