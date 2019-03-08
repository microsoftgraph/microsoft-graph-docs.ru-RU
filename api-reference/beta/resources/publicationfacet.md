---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: PublicationFacet
localization_priority: Normal
ms.openlocfilehash: 66e12c3240d1cade57d377e43403b33102fe166e
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482065"
---
# <a name="publicationfacet-resource-type"></a><span data-ttu-id="a473f-102">Тип ресурса publicationFacet</span><span class="sxs-lookup"><span data-stu-id="a473f-102">PublicationFacet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a473f-103">Ресурс **publicationFacet** содержит сведения о состоянии публикации ресурса [driveItemVersion](driveitemversion.md) или [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="a473f-103">The **publicationFacet** resource provides details on the published status of a [driveItemVersion](driveitemversion.md) or [driveItem](driveitem.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a473f-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a473f-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="a473f-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="a473f-105">Properties</span></span>

|   <span data-ttu-id="a473f-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="a473f-106">Property</span></span>    |  <span data-ttu-id="a473f-107">Тип</span><span class="sxs-lookup"><span data-stu-id="a473f-107">Type</span></span>  | <span data-ttu-id="a473f-108">Описание</span><span class="sxs-lookup"><span data-stu-id="a473f-108">Description</span></span> |
| :------------ | :----- | :---------- |
| <span data-ttu-id="a473f-109">**level**</span><span class="sxs-lookup"><span data-stu-id="a473f-109">**level**</span></span>     | <span data-ttu-id="a473f-110">String</span><span class="sxs-lookup"><span data-stu-id="a473f-110">String</span></span> | <span data-ttu-id="a473f-111">Состояние публикации для данного документа.</span><span class="sxs-lookup"><span data-stu-id="a473f-111">The state of publication for this document.</span></span> <span data-ttu-id="a473f-112">Возможные значения: `published` или `checkout`.</span><span class="sxs-lookup"><span data-stu-id="a473f-112">Either `published` or `checkout`.</span></span> <span data-ttu-id="a473f-113">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a473f-113">Read-only.</span></span>  |
| <span data-ttu-id="a473f-114">**versionId**</span><span class="sxs-lookup"><span data-stu-id="a473f-114">**versionId**</span></span> | <span data-ttu-id="a473f-115">String</span><span class="sxs-lookup"><span data-stu-id="a473f-115">String</span></span> | <span data-ttu-id="a473f-116">Уникальный идентификатор для версии, отображаемый для текущего вызывающего объекта.</span><span class="sxs-lookup"><span data-stu-id="a473f-116">The unique identifier for the version that is visible to the current caller.</span></span> <span data-ttu-id="a473f-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a473f-117">Read-only.</span></span>  |


<!--
{
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo",
  "suppressions": [
    "Error: /api-reference/beta/resources/publicationfacet.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
