---
author: daspek
ms.author: dspektor
ms.date: 09/13/2017
title: contentTypeOrder
ms.openlocfilehash: fe7309373ded16fe2660e0c5a69773c18ffb581a
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="contenttypeorder-resource-type"></a><span data-ttu-id="5add0-102">Тип ресурса contentTypeOrder</span><span class="sxs-lookup"><span data-stu-id="5add0-102">ContentTypeOrder resource type</span></span>

<span data-ttu-id="5add0-103">Ресурс **contentTypeOrder** указывает, в каком порядке тип контента будет отображаться в средстве выбора.</span><span class="sxs-lookup"><span data-stu-id="5add0-103">The **contentTypeOrder** resource specifies in which order the Content Type will appear in the selection UI.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5add0-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="5add0-104">JSON representation</span></span>

<span data-ttu-id="5add0-105">Ниже показано представление ресурса **contentTypeOrder** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5add0-105">Here is a JSON representation of a **baseItem** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a><span data-ttu-id="5add0-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="5add0-106">Properties</span></span>

| <span data-ttu-id="5add0-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="5add0-107">Property name</span></span> | <span data-ttu-id="5add0-108">Тип</span><span class="sxs-lookup"><span data-stu-id="5add0-108">Type</span></span>    | <span data-ttu-id="5add0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5add0-109">Description</span></span>
|:--------------|:--------|:----------------------------------------------------
| <span data-ttu-id="5add0-110">**default**</span><span class="sxs-lookup"><span data-stu-id="5add0-110">**Default**</span></span>   | <span data-ttu-id="5add0-111">логический</span><span class="sxs-lookup"><span data-stu-id="5add0-111">boolean</span></span> | <span data-ttu-id="5add0-112">Указывает, используется ли этот тип контента по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5add0-112">Whether this is the default Content Type</span></span>
| <span data-ttu-id="5add0-113">**position**</span><span class="sxs-lookup"><span data-stu-id="5add0-113">**position**</span></span>  | <span data-ttu-id="5add0-114">Int32</span><span class="sxs-lookup"><span data-stu-id="5add0-114">Int32</span></span>   | <span data-ttu-id="5add0-115">Указывает позицию, в которой тип контента отображается в средстве выбора.</span><span class="sxs-lookup"><span data-stu-id="5add0-115">Specifies the position in which the Content Type appears in the selection UI.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeOrder"
} -->
