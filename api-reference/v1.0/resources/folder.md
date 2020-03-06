---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Folder
localization_priority: Normal
description: 'Ресурс Folder — это единая структура, объединяющая данные элемента, связанные с папками. '
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 1ee34252671477a1efb83daf056330b499d94966
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531396"
---
# <a name="folder-resource-type"></a><span data-ttu-id="56d63-103">Тип ресурса Folder</span><span class="sxs-lookup"><span data-stu-id="56d63-103">Folder resource type</span></span>

<span data-ttu-id="56d63-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56d63-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="56d63-p101">Ресурс **Folder** — это единая структура, объединяющая данные элемента, связанные с папками. Ресурсы [**DriveItem**](driveitem.md) с ненулевым аспектом **folder** являются контейнерами для других ресурсов DriveItem.</span><span class="sxs-lookup"><span data-stu-id="56d63-p101">The **Folder** resource groups folder-related data on an item into a single structure. [**DriveItems**](driveitem.md) with a non-null **folder** facet are containers for other DriveItems.</span></span>

## <a name="json-representation"></a><span data-ttu-id="56d63-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="56d63-107">JSON representation</span></span>

<span data-ttu-id="56d63-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="56d63-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="56d63-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="56d63-109">Properties</span></span>

| <span data-ttu-id="56d63-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="56d63-110">Property</span></span>       | <span data-ttu-id="56d63-111">Тип</span><span class="sxs-lookup"><span data-stu-id="56d63-111">Type</span></span>           | <span data-ttu-id="56d63-112">Описание</span><span class="sxs-lookup"><span data-stu-id="56d63-112">Description</span></span>
|:---------------|:---------------|:-------------------------------------------
| <span data-ttu-id="56d63-113">**childCount**</span><span class="sxs-lookup"><span data-stu-id="56d63-113">**childCount**</span></span> | <span data-ttu-id="56d63-114">Int32</span><span class="sxs-lookup"><span data-stu-id="56d63-114">Int32</span></span>          | <span data-ttu-id="56d63-115">Количество дочерних элементов, содержащихся непосредственно в этом контейнере.</span><span class="sxs-lookup"><span data-stu-id="56d63-115">Number of children contained immediately within this container.</span></span>
| <span data-ttu-id="56d63-116">**view**</span><span class="sxs-lookup"><span data-stu-id="56d63-116">**view**</span></span>       | <span data-ttu-id="56d63-117">[folderView][]</span><span class="sxs-lookup"><span data-stu-id="56d63-117">[folderView][]</span></span> | <span data-ttu-id="56d63-118">Коллекция свойств, определяющих рекомендуемое представление для папки.</span><span class="sxs-lookup"><span data-stu-id="56d63-118">A collection of properties defining the recommended view for the folder.</span></span>

## <a name="remarks"></a><span data-ttu-id="56d63-119">Замечания</span><span class="sxs-lookup"><span data-stu-id="56d63-119">Remarks</span></span> 

<span data-ttu-id="56d63-120">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem][].</span><span class="sxs-lookup"><span data-stu-id="56d63-120">For more information about the facets on a DriveItem, see [DriveItem][].</span></span>

[folderView]: folderview.md
[DriveItem]: driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "The Folder facet describes properties of a folder",
  "keywords": "folder,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Folder"
} -->
