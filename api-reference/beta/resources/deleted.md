---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Deleted
ms.openlocfilehash: 5a0dd4132f39574f0af04282bd3f39bfd303eef1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076462"
---
# <a name="deleted-facet"></a><span data-ttu-id="47e10-102">Аспект Deleted</span><span class="sxs-lookup"><span data-stu-id="47e10-102">Deleted facet</span></span>

> <span data-ttu-id="47e10-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="47e10-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="47e10-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47e10-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="47e10-p102">Тип ресурса **Deleted** указывает, что элемент был удален. В этой версии API наличие ненулевого значения ресурса указывает, что файл был удален. Нулевое (или отсутствующее) значение указывает, что файл не удален.</span><span class="sxs-lookup"><span data-stu-id="47e10-p102">The **Deleted** resource indicates that the item has been deleted. In this version of the API, the presence (non-null) of the resource value indicates that the file was deleted. A null (or missing) value indicates that the file is not deleted.</span></span>

<span data-ttu-id="47e10-108">Дополнительные сведения об отслеживании изменений и поиске удаленных элементов см. в статье о том, как [просматривать изменения в элементах](../api/driveitem-delta.md).</span><span class="sxs-lookup"><span data-stu-id="47e10-108">See [view changes for an item](../api/driveitem-delta.md) for more information on tracking changes and finding deleted items.</span></span>

## <a name="json-representation"></a><span data-ttu-id="47e10-109">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="47e10-109">JSON representation</span></span>

<span data-ttu-id="47e10-110">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="47e10-110">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="47e10-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="47e10-111">Properties</span></span>

| <span data-ttu-id="47e10-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="47e10-112">Property</span></span> | <span data-ttu-id="47e10-113">Тип</span><span class="sxs-lookup"><span data-stu-id="47e10-113">Type</span></span>   | <span data-ttu-id="47e10-114">Описание</span><span class="sxs-lookup"><span data-stu-id="47e10-114">Description</span></span>                               |
|:---------|:-------|:------------------------------------------|
| <span data-ttu-id="47e10-115">state</span><span class="sxs-lookup"><span data-stu-id="47e10-115">state</span></span>    | <span data-ttu-id="47e10-116">String</span><span class="sxs-lookup"><span data-stu-id="47e10-116">String</span></span> | <span data-ttu-id="47e10-117">Представляет состояние удаленного элемента.</span><span class="sxs-lookup"><span data-stu-id="47e10-117">Represents the state of the deleted item.</span></span> |

## <a name="remarks"></a><span data-ttu-id="47e10-118">Заметки</span><span class="sxs-lookup"><span data-stu-id="47e10-118">Remarks</span></span> 

<span data-ttu-id="47e10-119">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="47e10-119">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The deleted facet providers properties about deleted items",
  "keywords": "deleted,delete,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Deleted"
} -->
