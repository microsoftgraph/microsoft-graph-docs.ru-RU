---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: PublicationFacet
ms.openlocfilehash: 60dff1e0dd97073ccb7eccd7be0f51b6b77fc273
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078905"
---
# <a name="publicationfacet-resource-type"></a><span data-ttu-id="4865b-102">Тип ресурса publicationFacet</span><span class="sxs-lookup"><span data-stu-id="4865b-102">PublicationFacet resource type</span></span>

> <span data-ttu-id="4865b-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4865b-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4865b-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4865b-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4865b-105">Ресурс **publicationFacet** содержит сведения о состоянии публикации ресурса [driveItemVersion](driveitemversion.md) или [driveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="4865b-105">The **publicationFacet** resource provides details on the published status of a [driveItemVersion](driveitemversion.md) or [driveItem](driveitem.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4865b-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="4865b-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="4865b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4865b-107">Properties</span></span>

|   <span data-ttu-id="4865b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4865b-108">Property</span></span>    |  <span data-ttu-id="4865b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4865b-109">Type</span></span>  | <span data-ttu-id="4865b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4865b-110">Description</span></span> |
| :------------ | :----- | :---------- |
| <span data-ttu-id="4865b-111">**level**</span><span class="sxs-lookup"><span data-stu-id="4865b-111">**level**</span></span>     | <span data-ttu-id="4865b-112">String</span><span class="sxs-lookup"><span data-stu-id="4865b-112">String</span></span> | <span data-ttu-id="4865b-113">Состояние публикации для данного документа.</span><span class="sxs-lookup"><span data-stu-id="4865b-113">The state of publication for this document.</span></span> <span data-ttu-id="4865b-114">Возможные значения: `published` или `checkout`.</span><span class="sxs-lookup"><span data-stu-id="4865b-114">Either `published` or `checkout`.</span></span> <span data-ttu-id="4865b-115">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4865b-115">Read-only.</span></span>  |
| <span data-ttu-id="4865b-116">**versionId**</span><span class="sxs-lookup"><span data-stu-id="4865b-116">**versionId**</span></span> | <span data-ttu-id="4865b-117">String</span><span class="sxs-lookup"><span data-stu-id="4865b-117">String</span></span> | <span data-ttu-id="4865b-118">Уникальный идентификатор для версии, отображаемый для текущего вызывающего объекта.</span><span class="sxs-lookup"><span data-stu-id="4865b-118">The unique identifier for the version that is visible to the current caller.</span></span> <span data-ttu-id="4865b-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4865b-119">Read-only.</span></span>  |


<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo"
} -->
