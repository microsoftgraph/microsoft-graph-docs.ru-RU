---
author: JeremyKelley
ms.date: 09/10/2017
title: Folder
localization_priority: Normal
description: 'Ресурс Folder — это единая структура, объединяющая данные элемента, связанные с папками. '
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 27ea5bc0d90d89c13fe751e78e9aef423dd099ff
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50240040"
---
# <a name="folder-resource-type"></a><span data-ttu-id="9d248-103">Тип ресурса Folder</span><span class="sxs-lookup"><span data-stu-id="9d248-103">Folder resource type</span></span>

<span data-ttu-id="9d248-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d248-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9d248-p101">Ресурс **Folder** — это единая структура, объединяющая данные элемента, связанные с папками. Ресурсы [**DriveItem**](driveitem.md) с ненулевым аспектом **folder** являются контейнерами для других ресурсов DriveItem.</span><span class="sxs-lookup"><span data-stu-id="9d248-p101">The **Folder** resource groups folder-related data on an item into a single structure. [**DriveItems**](driveitem.md) with a non-null **folder** facet are containers for other DriveItems.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9d248-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9d248-107">JSON representation</span></span>

<span data-ttu-id="9d248-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9d248-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.folder"
}-->

```json
{
  "childCount": 1024,
  "view": { "@odata.type": "microsoft.graph.folderView" }
}
```

## <a name="properties"></a><span data-ttu-id="9d248-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="9d248-109">Properties</span></span>

| <span data-ttu-id="9d248-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="9d248-110">Property</span></span>       | <span data-ttu-id="9d248-111">Тип</span><span class="sxs-lookup"><span data-stu-id="9d248-111">Type</span></span>           | <span data-ttu-id="9d248-112">Описание</span><span class="sxs-lookup"><span data-stu-id="9d248-112">Description</span></span>
|:---------------|:---------------|:-------------------------------------------
| <span data-ttu-id="9d248-113">**childCount**</span><span class="sxs-lookup"><span data-stu-id="9d248-113">**childCount**</span></span> | <span data-ttu-id="9d248-114">Int32</span><span class="sxs-lookup"><span data-stu-id="9d248-114">Int32</span></span>          | <span data-ttu-id="9d248-115">Количество дочерних элементов, содержащихся непосредственно в этом контейнере.</span><span class="sxs-lookup"><span data-stu-id="9d248-115">Number of children contained immediately within this container.</span></span>
| <span data-ttu-id="9d248-116">**view**</span><span class="sxs-lookup"><span data-stu-id="9d248-116">**view**</span></span>       | <span data-ttu-id="9d248-117">[folderView][]</span><span class="sxs-lookup"><span data-stu-id="9d248-117">[folderView][]</span></span> | <span data-ttu-id="9d248-118">Коллекция свойств, определяющих рекомендуемое представление для папки.</span><span class="sxs-lookup"><span data-stu-id="9d248-118">A collection of properties defining the recommended view for the folder.</span></span>

## <a name="remarks"></a><span data-ttu-id="9d248-119">Замечания</span><span class="sxs-lookup"><span data-stu-id="9d248-119">Remarks</span></span> 

<span data-ttu-id="9d248-120">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem][].</span><span class="sxs-lookup"><span data-stu-id="9d248-120">For more information about the facets on a DriveItem, see [DriveItem][].</span></span>

[folderView]: folderview.md
[DriveItem]: driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "The Folder facet describes properties of a folder",
  "keywords": "folder,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Folder"
} -->

