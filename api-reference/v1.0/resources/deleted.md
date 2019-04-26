---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Deleted
localization_priority: Normal
ms.openlocfilehash: d52ca0a9815e46ebc11a653be381ac65f3cd209e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32574626"
---
# <a name="deleted-facet"></a><span data-ttu-id="a5d38-102">Аспект Deleted</span><span class="sxs-lookup"><span data-stu-id="a5d38-102">Deleted facet</span></span>

<span data-ttu-id="a5d38-p101">Тип ресурса **Deleted** указывает, что элемент был удален. В этой версии API наличие ненулевого значения ресурса указывает, что файл был удален. Нулевое (или отсутствующее) значение указывает, что файл не удален.</span><span class="sxs-lookup"><span data-stu-id="a5d38-p101">The **Deleted** resource indicates that the item has been deleted. In this version of the API, the presence (non-null) of the resource value indicates that the file was deleted. A null (or missing) value indicates that the file is not deleted.</span></span>

<span data-ttu-id="a5d38-106">Дополнительные сведения об отслеживании изменений и поиске удаленных элементов см. в статье о том, как [просматривать изменения в элементах](../api/driveitem-delta.md).</span><span class="sxs-lookup"><span data-stu-id="a5d38-106">See [view changes for an item](../api/driveitem-delta.md) for more information on tracking changes and finding deleted items.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a5d38-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a5d38-107">JSON representation</span></span>

<span data-ttu-id="a5d38-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a5d38-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="a5d38-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="a5d38-109">Properties</span></span>

| <span data-ttu-id="a5d38-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="a5d38-110">Property</span></span> | <span data-ttu-id="a5d38-111">Тип</span><span class="sxs-lookup"><span data-stu-id="a5d38-111">Type</span></span>   | <span data-ttu-id="a5d38-112">Описание</span><span class="sxs-lookup"><span data-stu-id="a5d38-112">Description</span></span>                               |
|:---------|:-------|:------------------------------------------|
| <span data-ttu-id="a5d38-113">state</span><span class="sxs-lookup"><span data-stu-id="a5d38-113">state</span></span>    | <span data-ttu-id="a5d38-114">String</span><span class="sxs-lookup"><span data-stu-id="a5d38-114">String</span></span> | <span data-ttu-id="a5d38-115">Представляет состояние удаленного элемента.</span><span class="sxs-lookup"><span data-stu-id="a5d38-115">Represents the state of the deleted item.</span></span> |

## <a name="remarks"></a><span data-ttu-id="a5d38-116">Заметки</span><span class="sxs-lookup"><span data-stu-id="a5d38-116">Remarks</span></span> 

<span data-ttu-id="a5d38-117">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="a5d38-117">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The deleted facet providers properties about deleted items",
  "keywords": "deleted,delete,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Deleted"
} -->
