---
author: daspek
ms.author: dspektor
ms.date: 09/13/2017
title: contentTypeOrder
localization_priority: Normal
ms.openlocfilehash: 32cca632933cf2b0fad1f8e9149973d95b4322d3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341234"
---
# <a name="contenttypeorder-resource-type"></a><span data-ttu-id="aea52-102">Тип ресурса contentTypeOrder</span><span class="sxs-lookup"><span data-stu-id="aea52-102">ContentTypeOrder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aea52-103">Ресурс **contentTypeOrder** указывает, в каком порядке тип контента будет отображаться в пользовательском интерфейсе выбора.</span><span class="sxs-lookup"><span data-stu-id="aea52-103">The **contentTypeOrder** resource specifies in which order the Content Type will appear in the selection UI.</span></span>

## <a name="json-representation"></a><span data-ttu-id="aea52-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="aea52-104">JSON representation</span></span>

<span data-ttu-id="aea52-105">Ниже показано представление ресурса **contentTypeOrder** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aea52-105">Here is a JSON representation of a **contentTypeOrder** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a><span data-ttu-id="aea52-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="aea52-106">Properties</span></span>

| <span data-ttu-id="aea52-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="aea52-107">Property name</span></span> | <span data-ttu-id="aea52-108">Тип</span><span class="sxs-lookup"><span data-stu-id="aea52-108">Type</span></span>    | <span data-ttu-id="aea52-109">Описание</span><span class="sxs-lookup"><span data-stu-id="aea52-109">Description</span></span>
|:--------------|:--------|:----------------------------------------------------
| <span data-ttu-id="aea52-110">**default**</span><span class="sxs-lookup"><span data-stu-id="aea52-110">**default**</span></span>   | <span data-ttu-id="aea52-111">boolean</span><span class="sxs-lookup"><span data-stu-id="aea52-111">boolean</span></span> | <span data-ttu-id="aea52-112">Указывает, используется ли этот тип контента по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="aea52-112">Whether this is the default Content Type</span></span>
| <span data-ttu-id="aea52-113">**position**</span><span class="sxs-lookup"><span data-stu-id="aea52-113">**position**</span></span>  | <span data-ttu-id="aea52-114">Int32</span><span class="sxs-lookup"><span data-stu-id="aea52-114">Int32</span></span>   | <span data-ttu-id="aea52-115">Указывает позицию, в которой тип контента отображается в пользовательском интерфейсе выбора.</span><span class="sxs-lookup"><span data-stu-id="aea52-115">Specifies the position in which the Content Type appears in the selection UI.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeOrder",
  "suppressions": []
}
-->
