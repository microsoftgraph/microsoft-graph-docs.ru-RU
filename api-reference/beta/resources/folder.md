---
author: JeremyKelley
description: 'Ресурс Folder — это единая структура, объединяющая данные элемента, связанные с папками. '
ms.date: 09/10/2017
title: Folder
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: b7950008a3bcd310e90f604becb865d130781b34
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42497897"
---
# <a name="folder-resource-type"></a><span data-ttu-id="eeb9f-103">Тип ресурса Folder</span><span class="sxs-lookup"><span data-stu-id="eeb9f-103">Folder resource type</span></span>

<span data-ttu-id="eeb9f-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="eeb9f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eeb9f-p101">Ресурс **Folder** — это единая структура, объединяющая данные элемента, связанные с папками. Ресурсы [**DriveItem**](driveitem.md) с ненулевым аспектом **folder** являются контейнерами для других ресурсов DriveItem.</span><span class="sxs-lookup"><span data-stu-id="eeb9f-p101">The **Folder** resource groups folder-related data on an item into a single structure. [**DriveItems**](driveitem.md) with a non-null **folder** facet are containers for other DriveItems.</span></span>

## <a name="json-representation"></a><span data-ttu-id="eeb9f-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eeb9f-107">JSON representation</span></span>

<span data-ttu-id="eeb9f-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eeb9f-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="eeb9f-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="eeb9f-109">Properties</span></span>

| <span data-ttu-id="eeb9f-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="eeb9f-110">Property</span></span>       | <span data-ttu-id="eeb9f-111">Тип</span><span class="sxs-lookup"><span data-stu-id="eeb9f-111">Type</span></span>           | <span data-ttu-id="eeb9f-112">Описание</span><span class="sxs-lookup"><span data-stu-id="eeb9f-112">Description</span></span>
|:---------------|:---------------|:-------------------------------------------
| <span data-ttu-id="eeb9f-113">**childCount**</span><span class="sxs-lookup"><span data-stu-id="eeb9f-113">**childCount**</span></span> | <span data-ttu-id="eeb9f-114">Int64</span><span class="sxs-lookup"><span data-stu-id="eeb9f-114">Int64</span></span>          | <span data-ttu-id="eeb9f-115">Количество дочерних элементов, содержащихся непосредственно в этом контейнере.</span><span class="sxs-lookup"><span data-stu-id="eeb9f-115">Number of children contained immediately within this container.</span></span>
| <span data-ttu-id="eeb9f-116">**view**</span><span class="sxs-lookup"><span data-stu-id="eeb9f-116">**view**</span></span>       | <span data-ttu-id="eeb9f-117">[folderView][]</span><span class="sxs-lookup"><span data-stu-id="eeb9f-117">[folderView][]</span></span> | <span data-ttu-id="eeb9f-118">Коллекция свойств, определяющих рекомендуемое представление для папки.</span><span class="sxs-lookup"><span data-stu-id="eeb9f-118">A collection of properties defining the recommended view for the folder.</span></span>


## <a name="remarks"></a><span data-ttu-id="eeb9f-119">Замечания</span><span class="sxs-lookup"><span data-stu-id="eeb9f-119">Remarks</span></span> 

<span data-ttu-id="eeb9f-120">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem][].</span><span class="sxs-lookup"><span data-stu-id="eeb9f-120">For more information about the facets on a DriveItem, see [DriveItem][].</span></span>

[folderView]: folderview.md
[DriveItem]: driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "folder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
