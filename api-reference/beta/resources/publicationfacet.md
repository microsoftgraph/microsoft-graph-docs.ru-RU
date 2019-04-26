---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: PublicationFacet
localization_priority: Normal
ms.openlocfilehash: a95ec524b8e33ce65d9ecb7030a90a49305cdf6c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344093"
---
# <a name="publicationfacet-resource-type"></a><span data-ttu-id="09c15-102">Тип ресурса publicationFacet</span><span class="sxs-lookup"><span data-stu-id="09c15-102">PublicationFacet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09c15-103">Ресурс **publicationFacet** содержит сведения о состоянии публикации ресурса [driveItemVersion](driveitemversion.md) или [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="09c15-103">The **publicationFacet** resource provides details on the published status of a [driveItemVersion](driveitemversion.md) or [driveItem](driveitem.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="09c15-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="09c15-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="09c15-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="09c15-105">Properties</span></span>

|   <span data-ttu-id="09c15-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="09c15-106">Property</span></span>    |  <span data-ttu-id="09c15-107">Тип</span><span class="sxs-lookup"><span data-stu-id="09c15-107">Type</span></span>  | <span data-ttu-id="09c15-108">Описание</span><span class="sxs-lookup"><span data-stu-id="09c15-108">Description</span></span> |
| :------------ | :----- | :---------- |
| <span data-ttu-id="09c15-109">**level**</span><span class="sxs-lookup"><span data-stu-id="09c15-109">**level**</span></span>     | <span data-ttu-id="09c15-110">String</span><span class="sxs-lookup"><span data-stu-id="09c15-110">String</span></span> | <span data-ttu-id="09c15-111">Состояние публикации для данного документа.</span><span class="sxs-lookup"><span data-stu-id="09c15-111">The state of publication for this document.</span></span> <span data-ttu-id="09c15-112">Возможные значения: `published` или `checkout`.</span><span class="sxs-lookup"><span data-stu-id="09c15-112">Either `published` or `checkout`.</span></span> <span data-ttu-id="09c15-113">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="09c15-113">Read-only.</span></span>  |
| <span data-ttu-id="09c15-114">**versionId**</span><span class="sxs-lookup"><span data-stu-id="09c15-114">**versionId**</span></span> | <span data-ttu-id="09c15-115">String</span><span class="sxs-lookup"><span data-stu-id="09c15-115">String</span></span> | <span data-ttu-id="09c15-116">Уникальный идентификатор для версии, отображаемый для текущего вызывающего объекта.</span><span class="sxs-lookup"><span data-stu-id="09c15-116">The unique identifier for the version that is visible to the current caller.</span></span> <span data-ttu-id="09c15-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="09c15-117">Read-only.</span></span>  |


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
