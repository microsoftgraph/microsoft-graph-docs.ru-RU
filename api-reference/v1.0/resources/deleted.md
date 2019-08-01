---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Deleted
localization_priority: Normal
description: Тип ресурса Deleted указывает, что элемент был удален.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d1f5c07c60c8de4890a2a4ac334df04a59b7339c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029521"
---
# <a name="deleted-facet"></a><span data-ttu-id="bedec-103">Аспект Deleted</span><span class="sxs-lookup"><span data-stu-id="bedec-103">Deleted facet</span></span>

<span data-ttu-id="bedec-p101">Тип ресурса **Deleted** указывает, что элемент был удален. В этой версии API наличие ненулевого значения ресурса указывает, что файл был удален. Нулевое (или отсутствующее) значение указывает, что файл не удален.</span><span class="sxs-lookup"><span data-stu-id="bedec-p101">The **Deleted** resource indicates that the item has been deleted. In this version of the API, the presence (non-null) of the resource value indicates that the file was deleted. A null (or missing) value indicates that the file is not deleted.</span></span>

<span data-ttu-id="bedec-107">Дополнительные сведения об отслеживании изменений и поиске удаленных элементов см. в статье о том, как [просматривать изменения в элементах](../api/driveitem-delta.md).</span><span class="sxs-lookup"><span data-stu-id="bedec-107">See [view changes for an item](../api/driveitem-delta.md) for more information on tracking changes and finding deleted items.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bedec-108">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bedec-108">JSON representation</span></span>

<span data-ttu-id="bedec-109">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bedec-109">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="bedec-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="bedec-110">Properties</span></span>

| <span data-ttu-id="bedec-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="bedec-111">Property</span></span> | <span data-ttu-id="bedec-112">Тип</span><span class="sxs-lookup"><span data-stu-id="bedec-112">Type</span></span>   | <span data-ttu-id="bedec-113">Описание</span><span class="sxs-lookup"><span data-stu-id="bedec-113">Description</span></span>                               |
|:---------|:-------|:------------------------------------------|
| <span data-ttu-id="bedec-114">state</span><span class="sxs-lookup"><span data-stu-id="bedec-114">state</span></span>    | <span data-ttu-id="bedec-115">String</span><span class="sxs-lookup"><span data-stu-id="bedec-115">String</span></span> | <span data-ttu-id="bedec-116">Представляет состояние удаленного элемента.</span><span class="sxs-lookup"><span data-stu-id="bedec-116">Represents the state of the deleted item.</span></span> |

## <a name="remarks"></a><span data-ttu-id="bedec-117">Заметки</span><span class="sxs-lookup"><span data-stu-id="bedec-117">Remarks</span></span> 

<span data-ttu-id="bedec-118">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="bedec-118">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The deleted facet providers properties about deleted items",
  "keywords": "deleted,delete,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Deleted"
} -->
