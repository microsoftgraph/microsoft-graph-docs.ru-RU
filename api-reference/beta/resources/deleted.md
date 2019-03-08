---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Deleted
localization_priority: Normal
ms.openlocfilehash: 06fe9835ef4b31d7a48bad955b17872142a94b2d
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480784"
---
# <a name="deleted-facet"></a><span data-ttu-id="95a95-102">Аспект Deleted</span><span class="sxs-lookup"><span data-stu-id="95a95-102">Deleted facet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95a95-p101">Тип ресурса **Deleted** указывает, что элемент был удален. В этой версии API наличие ненулевого значения ресурса указывает, что файл был удален. Нулевое (или отсутствующее) значение указывает, что файл не удален.</span><span class="sxs-lookup"><span data-stu-id="95a95-p101">The **Deleted** resource indicates that the item has been deleted. In this version of the API, the presence (non-null) of the resource value indicates that the file was deleted. A null (or missing) value indicates that the file is not deleted.</span></span>

<span data-ttu-id="95a95-106">Дополнительные сведения об отслеживании изменений и поиске удаленных элементов см. в статье о том, как [просматривать изменения в элементах](../api/driveitem-delta.md).</span><span class="sxs-lookup"><span data-stu-id="95a95-106">See [view changes for an item](../api/driveitem-delta.md) for more information on tracking changes and finding deleted items.</span></span>

## <a name="json-representation"></a><span data-ttu-id="95a95-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="95a95-107">JSON representation</span></span>

<span data-ttu-id="95a95-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="95a95-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  "state"
  ],
  "@odata.type": "microsoft.graph.deleted"
}-->
```json
{
  "state": "string"
}
```
## <a name="properties"></a><span data-ttu-id="95a95-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="95a95-109">Properties</span></span>

| <span data-ttu-id="95a95-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="95a95-110">Property</span></span> | <span data-ttu-id="95a95-111">Тип</span><span class="sxs-lookup"><span data-stu-id="95a95-111">Type</span></span>   | <span data-ttu-id="95a95-112">Описание</span><span class="sxs-lookup"><span data-stu-id="95a95-112">Description</span></span>                               |
|:---------|:-------|:------------------------------------------|
| <span data-ttu-id="95a95-113">state</span><span class="sxs-lookup"><span data-stu-id="95a95-113">state</span></span>    | <span data-ttu-id="95a95-114">String</span><span class="sxs-lookup"><span data-stu-id="95a95-114">String</span></span> | <span data-ttu-id="95a95-115">Представляет состояние удаленного элемента.</span><span class="sxs-lookup"><span data-stu-id="95a95-115">Represents the state of the deleted item.</span></span> |

## <a name="remarks"></a><span data-ttu-id="95a95-116">Заметки</span><span class="sxs-lookup"><span data-stu-id="95a95-116">Remarks</span></span> 

<span data-ttu-id="95a95-117">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="95a95-117">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The deleted facet providers properties about deleted items",
  "keywords": "deleted,delete,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Deleted",
  "suppressions": [
    "Error: /api-reference/beta/resources/deleted.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
