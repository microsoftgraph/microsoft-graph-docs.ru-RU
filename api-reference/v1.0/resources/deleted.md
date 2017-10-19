---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Deleted
ms.openlocfilehash: 1d45219b2ef26bdc96c46e386d66d91874f9bc0b
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="deleted-facet"></a><span data-ttu-id="35888-102">Аспект Deleted</span><span class="sxs-lookup"><span data-stu-id="35888-102">Deleted facet</span></span>

<span data-ttu-id="35888-103">Ресурс **Deleted** указывает, что элемент был удален.</span><span class="sxs-lookup"><span data-stu-id="35888-103">The **Deleted** resource indicates that the item has been deleted.</span></span>
<span data-ttu-id="35888-104">В этой версии API наличие ненулевого значения ресурса указывает, что файл был удален.</span><span class="sxs-lookup"><span data-stu-id="35888-104">The Deleted resource indicates that the item has been deleted. In this version of the API, the presence (non-null) of the resource value indicates that the file was deleted. A null (or missing) value indicates that the file is not deleted.</span></span>
<span data-ttu-id="35888-105">Нулевое (или отсутствующее) значение указывает, что файл не удален.</span><span class="sxs-lookup"><span data-stu-id="35888-105">A null (or missing) value indicates the driveItem is not the root..</span></span>

<span data-ttu-id="35888-106">Дополнительные сведения об отслеживании изменений и поиске удаленных элементов см. в статье о том, как [просматривать изменения для элемента](../api/driveitem_delta.md).</span><span class="sxs-lookup"><span data-stu-id="35888-106">See [view changes for an item](../api/driveitem_delta.md) for more information on tracking changes and finding deleted items.</span></span>

## <a name="json-representation"></a><span data-ttu-id="35888-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="35888-107">JSON representation</span></span>

<span data-ttu-id="35888-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="35888-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="35888-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="35888-109">Properties</span></span>

| <span data-ttu-id="35888-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="35888-110">Property</span></span> | <span data-ttu-id="35888-111">Тип</span><span class="sxs-lookup"><span data-stu-id="35888-111">Type</span></span>   | <span data-ttu-id="35888-112">Описание</span><span class="sxs-lookup"><span data-stu-id="35888-112">Description</span></span>                               |
|:---------|:-------|:------------------------------------------|
| <span data-ttu-id="35888-113">state</span><span class="sxs-lookup"><span data-stu-id="35888-113">state</span></span>    | <span data-ttu-id="35888-114">String</span><span class="sxs-lookup"><span data-stu-id="35888-114">String</span></span> | <span data-ttu-id="35888-115">Представляет состояние удаленного элемента.</span><span class="sxs-lookup"><span data-stu-id="35888-115">Represents the state of the deleted item.</span></span> |

## <a name="remarks"></a><span data-ttu-id="35888-116">Заметки</span><span class="sxs-lookup"><span data-stu-id="35888-116">Remarks</span></span> 

<span data-ttu-id="35888-117">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="35888-117">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The deleted facet providers properties about deleted items",
  "keywords": "deleted,delete,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Deleted"
} -->
