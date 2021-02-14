---
author: JeremyKelley
ms.date: 09/10/2017
title: Deleted
localization_priority: Normal
description: Тип ресурса Deleted указывает, что элемент был удален.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 3743a343b9928eda4a888cff06a3ff1b7525f9c9
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239613"
---
# <a name="deleted-facet"></a><span data-ttu-id="c7240-103">Аспект Deleted</span><span class="sxs-lookup"><span data-stu-id="c7240-103">Deleted facet</span></span>

<span data-ttu-id="c7240-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7240-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c7240-p101">Тип ресурса **Deleted** указывает, что элемент был удален. В этой версии API наличие ненулевого значения ресурса указывает, что файл был удален. Нулевое (или отсутствующее) значение указывает, что файл не удален.</span><span class="sxs-lookup"><span data-stu-id="c7240-p101">The **Deleted** resource indicates that the item has been deleted. In this version of the API, the presence (non-null) of the resource value indicates that the file was deleted. A null (or missing) value indicates that the file is not deleted.</span></span>

<span data-ttu-id="c7240-108">Дополнительные сведения об отслеживании изменений и поиске удаленных элементов см. в статье о том, как [просматривать изменения в элементах](../api/driveitem-delta.md).</span><span class="sxs-lookup"><span data-stu-id="c7240-108">See [view changes for an item](../api/driveitem-delta.md) for more information on tracking changes and finding deleted items.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c7240-109">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c7240-109">JSON representation</span></span>

<span data-ttu-id="c7240-110">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c7240-110">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="c7240-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="c7240-111">Properties</span></span>

| <span data-ttu-id="c7240-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="c7240-112">Property</span></span> | <span data-ttu-id="c7240-113">Тип</span><span class="sxs-lookup"><span data-stu-id="c7240-113">Type</span></span>   | <span data-ttu-id="c7240-114">Описание</span><span class="sxs-lookup"><span data-stu-id="c7240-114">Description</span></span>                               |
|:---------|:-------|:------------------------------------------|
| <span data-ttu-id="c7240-115">state</span><span class="sxs-lookup"><span data-stu-id="c7240-115">state</span></span>    | <span data-ttu-id="c7240-116">String</span><span class="sxs-lookup"><span data-stu-id="c7240-116">String</span></span> | <span data-ttu-id="c7240-117">Представляет состояние удаленного элемента.</span><span class="sxs-lookup"><span data-stu-id="c7240-117">Represents the state of the deleted item.</span></span> |

## <a name="remarks"></a><span data-ttu-id="c7240-118">Заметки</span><span class="sxs-lookup"><span data-stu-id="c7240-118">Remarks</span></span> 

<span data-ttu-id="c7240-119">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="c7240-119">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The deleted facet providers properties about deleted items",
  "keywords": "deleted,delete,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Deleted"
} -->

