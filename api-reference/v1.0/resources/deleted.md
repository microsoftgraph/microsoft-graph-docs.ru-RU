---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Deleted
localization_priority: Normal
ms.openlocfilehash: a35bc781555486603c0319c819aa019704e362d9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886144"
---
# <a name="deleted-facet"></a><span data-ttu-id="4f9ca-102">Аспект Deleted</span><span class="sxs-lookup"><span data-stu-id="4f9ca-102">Deleted facet</span></span>

<span data-ttu-id="4f9ca-p101">Тип ресурса **Deleted** указывает, что элемент был удален. В этой версии API наличие ненулевого значения ресурса указывает, что файл был удален. Нулевое (или отсутствующее) значение указывает, что файл не удален.</span><span class="sxs-lookup"><span data-stu-id="4f9ca-p101">The **Deleted** resource indicates that the item has been deleted. In this version of the API, the presence (non-null) of the resource value indicates that the file was deleted. A null (or missing) value indicates that the file is not deleted.</span></span>

<span data-ttu-id="4f9ca-106">Дополнительные сведения об отслеживании изменений и поиске удаленных элементов см. в статье о том, как [просматривать изменения в элементах](../api/driveitem-delta.md).</span><span class="sxs-lookup"><span data-stu-id="4f9ca-106">See [view changes for an item](../api/driveitem-delta.md) for more information on tracking changes and finding deleted items.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4f9ca-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4f9ca-107">JSON representation</span></span>

<span data-ttu-id="4f9ca-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4f9ca-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="4f9ca-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="4f9ca-109">Properties</span></span>

| <span data-ttu-id="4f9ca-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="4f9ca-110">Property</span></span> | <span data-ttu-id="4f9ca-111">Тип</span><span class="sxs-lookup"><span data-stu-id="4f9ca-111">Type</span></span>   | <span data-ttu-id="4f9ca-112">Описание</span><span class="sxs-lookup"><span data-stu-id="4f9ca-112">Description</span></span>                               |
|:---------|:-------|:------------------------------------------|
| <span data-ttu-id="4f9ca-113">state</span><span class="sxs-lookup"><span data-stu-id="4f9ca-113">state</span></span>    | <span data-ttu-id="4f9ca-114">String</span><span class="sxs-lookup"><span data-stu-id="4f9ca-114">String</span></span> | <span data-ttu-id="4f9ca-115">Представляет состояние удаленного элемента.</span><span class="sxs-lookup"><span data-stu-id="4f9ca-115">Represents the state of the deleted item.</span></span> |

## <a name="remarks"></a><span data-ttu-id="4f9ca-116">Заметки</span><span class="sxs-lookup"><span data-stu-id="4f9ca-116">Remarks</span></span> 

<span data-ttu-id="4f9ca-117">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="4f9ca-117">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The deleted facet providers properties about deleted items",
  "keywords": "deleted,delete,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Deleted"
} -->
