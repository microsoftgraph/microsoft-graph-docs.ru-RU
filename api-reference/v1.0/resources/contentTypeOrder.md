---
author: daspek
ms.author: dspektor
ms.date: 09/13/2017
title: contentTypeOrder
localization_priority: Normal
ms.openlocfilehash: ccea5804c3f4eddb02b5d4163302362f29b5fbc8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561329"
---
# <a name="contenttypeorder-resource-type"></a><span data-ttu-id="7da14-102">Тип ресурса contentTypeOrder</span><span class="sxs-lookup"><span data-stu-id="7da14-102">ContentTypeOrder resource type</span></span>

<span data-ttu-id="7da14-103">Ресурс **contentTypeOrder** указывает, в каком порядке тип контента будет отображаться в пользовательском интерфейсе выбора.</span><span class="sxs-lookup"><span data-stu-id="7da14-103">The **contentTypeOrder** resource specifies in which order the Content Type will appear in the selection UI.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7da14-104">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7da14-104">JSON representation</span></span>

<span data-ttu-id="7da14-105">Ниже показано представление ресурса **contentTypeOrder** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7da14-105">Here is a JSON representation of a **contentTypeOrder** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.contentTypeOrder", "@type.aka": "oneDrive.contentTypeOrderFacet" } -->

```json
{
  "default": true,
  "position": 2
}
```

## <a name="properties"></a><span data-ttu-id="7da14-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="7da14-106">Properties</span></span>

| <span data-ttu-id="7da14-107">Имя свойства</span><span class="sxs-lookup"><span data-stu-id="7da14-107">Property name</span></span> | <span data-ttu-id="7da14-108">Тип</span><span class="sxs-lookup"><span data-stu-id="7da14-108">Type</span></span>    | <span data-ttu-id="7da14-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7da14-109">Description</span></span>
|:--------------|:--------|:----------------------------------------------------
| <span data-ttu-id="7da14-110">**default**</span><span class="sxs-lookup"><span data-stu-id="7da14-110">**default**</span></span>   | <span data-ttu-id="7da14-111">boolean</span><span class="sxs-lookup"><span data-stu-id="7da14-111">boolean</span></span> | <span data-ttu-id="7da14-112">Указывает, используется ли этот тип контента по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7da14-112">Whether this is the default Content Type</span></span>
| <span data-ttu-id="7da14-113">**position**</span><span class="sxs-lookup"><span data-stu-id="7da14-113">**position**</span></span>  | <span data-ttu-id="7da14-114">Int32</span><span class="sxs-lookup"><span data-stu-id="7da14-114">Int32</span></span>   | <span data-ttu-id="7da14-115">Указывает позицию, в которой тип контента отображается в пользовательском интерфейсе выбора.</span><span class="sxs-lookup"><span data-stu-id="7da14-115">Specifies the position in which the Content Type appears in the selection UI.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentTypeOrder"
} -->
