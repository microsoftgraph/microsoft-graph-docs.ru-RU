---
author: JeremyKelley
description: Тип ресурса Deleted указывает, что элемент был удален.
ms.date: 09/10/2017
title: Deleted
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: b3c1a7a4c9a7c290ba71a21ba288e6195334377b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507270"
---
# <a name="deleted-facet"></a><span data-ttu-id="55983-103">Аспект Deleted</span><span class="sxs-lookup"><span data-stu-id="55983-103">Deleted facet</span></span>

<span data-ttu-id="55983-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="55983-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55983-p101">Тип ресурса **Deleted** указывает, что элемент был удален. В этой версии API наличие ненулевого значения ресурса указывает, что файл был удален. Нулевое (или отсутствующее) значение указывает, что файл не удален.</span><span class="sxs-lookup"><span data-stu-id="55983-p101">The **Deleted** resource indicates that the item has been deleted. In this version of the API, the presence (non-null) of the resource value indicates that the file was deleted. A null (or missing) value indicates that the file is not deleted.</span></span>

<span data-ttu-id="55983-108">Дополнительные сведения об отслеживании изменений и поиске удаленных элементов см. в статье о том, как [просматривать изменения в элементах](../api/driveitem-delta.md).</span><span class="sxs-lookup"><span data-stu-id="55983-108">See [view changes for an item](../api/driveitem-delta.md) for more information on tracking changes and finding deleted items.</span></span>

## <a name="json-representation"></a><span data-ttu-id="55983-109">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="55983-109">JSON representation</span></span>

<span data-ttu-id="55983-110">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="55983-110">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="55983-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="55983-111">Properties</span></span>

| <span data-ttu-id="55983-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="55983-112">Property</span></span> | <span data-ttu-id="55983-113">Тип</span><span class="sxs-lookup"><span data-stu-id="55983-113">Type</span></span>   | <span data-ttu-id="55983-114">Описание</span><span class="sxs-lookup"><span data-stu-id="55983-114">Description</span></span>                               |
|:---------|:-------|:------------------------------------------|
| <span data-ttu-id="55983-115">state</span><span class="sxs-lookup"><span data-stu-id="55983-115">state</span></span>    | <span data-ttu-id="55983-116">String</span><span class="sxs-lookup"><span data-stu-id="55983-116">String</span></span> | <span data-ttu-id="55983-117">Представляет состояние удаленного элемента.</span><span class="sxs-lookup"><span data-stu-id="55983-117">Represents the state of the deleted item.</span></span> |

## <a name="remarks"></a><span data-ttu-id="55983-118">Заметки</span><span class="sxs-lookup"><span data-stu-id="55983-118">Remarks</span></span> 

<span data-ttu-id="55983-119">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="55983-119">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


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
