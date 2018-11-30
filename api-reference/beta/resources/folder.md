---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Folder
ms.openlocfilehash: 834b2cd7c81a947ca1e6d4619f39a8533677e6c3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080873"
---
# <a name="folder-resource-type"></a><span data-ttu-id="9d9cd-102">Тип ресурса Folder</span><span class="sxs-lookup"><span data-stu-id="9d9cd-102">Folder resource type</span></span>

> <span data-ttu-id="9d9cd-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9d9cd-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9d9cd-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d9cd-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9d9cd-p102">Ресурс **Folder** — это единая структура, объединяющая данные элемента, связанные с папками. Ресурсы [**DriveItem**](driveitem.md) с ненулевым аспектом **folder** являются контейнерами для других ресурсов DriveItem.</span><span class="sxs-lookup"><span data-stu-id="9d9cd-p102">The **Folder** resource groups folder-related data on an item into a single structure. [**DriveItems**](driveitem.md) with a non-null **folder** facet are containers for other DriveItems.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9d9cd-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9d9cd-107">JSON representation</span></span>

<span data-ttu-id="9d9cd-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9d9cd-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="9d9cd-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="9d9cd-109">Properties</span></span>

| <span data-ttu-id="9d9cd-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="9d9cd-110">Property</span></span>       | <span data-ttu-id="9d9cd-111">Тип</span><span class="sxs-lookup"><span data-stu-id="9d9cd-111">Type</span></span>           | <span data-ttu-id="9d9cd-112">Описание</span><span class="sxs-lookup"><span data-stu-id="9d9cd-112">Description</span></span>
|:---------------|:---------------|:-------------------------------------------
| <span data-ttu-id="9d9cd-113">**childCount**</span><span class="sxs-lookup"><span data-stu-id="9d9cd-113">**childCount**</span></span> | <span data-ttu-id="9d9cd-114">Int64</span><span class="sxs-lookup"><span data-stu-id="9d9cd-114">Int64</span></span>          | <span data-ttu-id="9d9cd-115">Количество дочерних элементов, содержащихся непосредственно в этом контейнере.</span><span class="sxs-lookup"><span data-stu-id="9d9cd-115">Number of children contained immediately within this container.</span></span>
| <span data-ttu-id="9d9cd-116">**view**</span><span class="sxs-lookup"><span data-stu-id="9d9cd-116">**view**</span></span>       | <span data-ttu-id="9d9cd-117">[folderView][]</span><span class="sxs-lookup"><span data-stu-id="9d9cd-117">[folderView][]</span></span> | <span data-ttu-id="9d9cd-118">Коллекция свойств, определяющих рекомендуемое представление для папки.</span><span class="sxs-lookup"><span data-stu-id="9d9cd-118">A collection of properties defining the recommended view for the folder.</span></span>


## <a name="remarks"></a><span data-ttu-id="9d9cd-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="9d9cd-119">Remarks</span></span> 

<span data-ttu-id="9d9cd-120">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem][].</span><span class="sxs-lookup"><span data-stu-id="9d9cd-120">For more information about the facets on a DriveItem, see [DriveItem][].</span></span>

[folderView]: folderview.md
[DriveItem]: driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "folder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
