---
author: daspek
ms.author: dspektor
ms.date: 09/13/2017
title: contentTypeOrder
ms.openlocfilehash: 8cb47837d8df1c38ed25fc87d3b4d7da450fed1a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024610"
---
# <a name="contenttypeorder-resource-type"></a><span data-ttu-id="90708-102">Тип ресурса contentTypeOrder</span><span class="sxs-lookup"><span data-stu-id="90708-102">ContentTypeOrder resource type</span></span>

<span data-ttu-id="90708-103">Ресурс **contentTypeOrder** указывает, в каком порядке тип контента будет отображаться в пользовательском интерфейсе выбора.</span><span class="sxs-lookup"><span data-stu-id="90708-103">The **contentTypeOrder** resource specifies in which order the Content Type will appear in the selection UI.</span></span>

## <a name="json-representation"></a><span data-ttu-id="90708-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="90708-104">JSON representation</span></span>

<span data-ttu-id="90708-105">Ниже показано представление ресурса **contentTypeOrder** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="90708-105">Here is a JSON representation of a **contentTypeOrder** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a><span data-ttu-id="90708-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="90708-106">Properties</span></span>

| <span data-ttu-id="90708-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="90708-107">Property name</span></span> | <span data-ttu-id="90708-108">Тип</span><span class="sxs-lookup"><span data-stu-id="90708-108">Type</span></span>    | <span data-ttu-id="90708-109">Описание</span><span class="sxs-lookup"><span data-stu-id="90708-109">Description</span></span>
|:--------------|:--------|:----------------------------------------------------
| <span data-ttu-id="90708-110">**default**</span><span class="sxs-lookup"><span data-stu-id="90708-110">**default**</span></span>   | <span data-ttu-id="90708-111">boolean</span><span class="sxs-lookup"><span data-stu-id="90708-111">boolean</span></span> | <span data-ttu-id="90708-112">Указывает, используется ли этот тип контента по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="90708-112">Whether this is the default Content Type</span></span>
| <span data-ttu-id="90708-113">**position**</span><span class="sxs-lookup"><span data-stu-id="90708-113">**position**</span></span>  | <span data-ttu-id="90708-114">Int32</span><span class="sxs-lookup"><span data-stu-id="90708-114">Int32</span></span>   | <span data-ttu-id="90708-115">Указывает позицию, в которой тип контента отображается в пользовательском интерфейсе выбора.</span><span class="sxs-lookup"><span data-stu-id="90708-115">Specifies the position in which the Content Type appears in the selection UI.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeOrder"
} -->
