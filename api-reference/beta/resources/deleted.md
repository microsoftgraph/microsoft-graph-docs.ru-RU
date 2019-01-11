---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Deleted
localization_priority: Normal
ms.openlocfilehash: 6316f31d41e9d8e7264a671ac0317ebf9b32173f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804769"
---
# <a name="deleted-facet"></a><span data-ttu-id="74a08-102">Аспект Deleted</span><span class="sxs-lookup"><span data-stu-id="74a08-102">Deleted facet</span></span>

> <span data-ttu-id="74a08-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="74a08-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="74a08-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="74a08-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="74a08-p102">Тип ресурса **Deleted** указывает, что элемент был удален. В этой версии API наличие ненулевого значения ресурса указывает, что файл был удален. Нулевое (или отсутствующее) значение указывает, что файл не удален.</span><span class="sxs-lookup"><span data-stu-id="74a08-p102">The **Deleted** resource indicates that the item has been deleted. In this version of the API, the presence (non-null) of the resource value indicates that the file was deleted. A null (or missing) value indicates that the file is not deleted.</span></span>

<span data-ttu-id="74a08-108">Дополнительные сведения об отслеживании изменений и поиске удаленных элементов см. в статье о том, как [просматривать изменения в элементах](../api/driveitem-delta.md).</span><span class="sxs-lookup"><span data-stu-id="74a08-108">See [view changes for an item](../api/driveitem-delta.md) for more information on tracking changes and finding deleted items.</span></span>

## <a name="json-representation"></a><span data-ttu-id="74a08-109">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="74a08-109">JSON representation</span></span>

<span data-ttu-id="74a08-110">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="74a08-110">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="74a08-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="74a08-111">Properties</span></span>

| <span data-ttu-id="74a08-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="74a08-112">Property</span></span> | <span data-ttu-id="74a08-113">Тип</span><span class="sxs-lookup"><span data-stu-id="74a08-113">Type</span></span>   | <span data-ttu-id="74a08-114">Описание</span><span class="sxs-lookup"><span data-stu-id="74a08-114">Description</span></span>                               |
|:---------|:-------|:------------------------------------------|
| <span data-ttu-id="74a08-115">state</span><span class="sxs-lookup"><span data-stu-id="74a08-115">state</span></span>    | <span data-ttu-id="74a08-116">String</span><span class="sxs-lookup"><span data-stu-id="74a08-116">String</span></span> | <span data-ttu-id="74a08-117">Представляет состояние удаленного элемента.</span><span class="sxs-lookup"><span data-stu-id="74a08-117">Represents the state of the deleted item.</span></span> |

## <a name="remarks"></a><span data-ttu-id="74a08-118">Заметки</span><span class="sxs-lookup"><span data-stu-id="74a08-118">Remarks</span></span> 

<span data-ttu-id="74a08-119">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="74a08-119">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The deleted facet providers properties about deleted items",
  "keywords": "deleted,delete,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Deleted"
} -->
