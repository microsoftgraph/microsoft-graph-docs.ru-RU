---
author: JeremyKelley
description: Тип ресурса Deleted указывает, что элемент был удален.
ms.date: 09/10/2017
title: Deleted
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 2771f1c46fca5c352499dbfb3b41f718834da8b5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973130"
---
# <a name="deleted-facet"></a><span data-ttu-id="9df80-103">Аспект Deleted</span><span class="sxs-lookup"><span data-stu-id="9df80-103">Deleted facet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9df80-p101">Тип ресурса **Deleted** указывает, что элемент был удален. В этой версии API наличие ненулевого значения ресурса указывает, что файл был удален. Нулевое (или отсутствующее) значение указывает, что файл не удален.</span><span class="sxs-lookup"><span data-stu-id="9df80-p101">The **Deleted** resource indicates that the item has been deleted. In this version of the API, the presence (non-null) of the resource value indicates that the file was deleted. A null (or missing) value indicates that the file is not deleted.</span></span>

<span data-ttu-id="9df80-107">Дополнительные сведения об отслеживании изменений и поиске удаленных элементов см. в статье о том, как [просматривать изменения в элементах](../api/driveitem-delta.md).</span><span class="sxs-lookup"><span data-stu-id="9df80-107">See [view changes for an item](../api/driveitem-delta.md) for more information on tracking changes and finding deleted items.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9df80-108">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9df80-108">JSON representation</span></span>

<span data-ttu-id="9df80-109">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9df80-109">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="9df80-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="9df80-110">Properties</span></span>

| <span data-ttu-id="9df80-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="9df80-111">Property</span></span> | <span data-ttu-id="9df80-112">Тип</span><span class="sxs-lookup"><span data-stu-id="9df80-112">Type</span></span>   | <span data-ttu-id="9df80-113">Описание</span><span class="sxs-lookup"><span data-stu-id="9df80-113">Description</span></span>                               |
|:---------|:-------|:------------------------------------------|
| <span data-ttu-id="9df80-114">state</span><span class="sxs-lookup"><span data-stu-id="9df80-114">state</span></span>    | <span data-ttu-id="9df80-115">String</span><span class="sxs-lookup"><span data-stu-id="9df80-115">String</span></span> | <span data-ttu-id="9df80-116">Представляет состояние удаленного элемента.</span><span class="sxs-lookup"><span data-stu-id="9df80-116">Represents the state of the deleted item.</span></span> |

## <a name="remarks"></a><span data-ttu-id="9df80-117">Заметки</span><span class="sxs-lookup"><span data-stu-id="9df80-117">Remarks</span></span> 

<span data-ttu-id="9df80-118">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="9df80-118">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The deleted facet providers properties about deleted items",
  "keywords": "deleted,delete,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Deleted",
  "suppressions": []
}
-->
