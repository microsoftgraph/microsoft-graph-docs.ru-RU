---
title: Тип ресурса workbookSessionInfo
description: Предоставляет сведения о сеансе книги.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 900ebdcefbdfa83e7b72b1c926a441f1c497626a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826931"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="a1d3b-103">Тип ресурса workbookSessionInfo</span><span class="sxs-lookup"><span data-stu-id="a1d3b-103">workbookSessionInfo resource type</span></span>

<span data-ttu-id="a1d3b-104">Предоставляет сведения о сеансе книги.</span><span class="sxs-lookup"><span data-stu-id="a1d3b-104">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="a1d3b-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a1d3b-105">JSON representation</span></span>

<span data-ttu-id="a1d3b-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="a1d3b-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.workbookSessionInfo"
}-->

```json
{
  "id": "string",
  "persistChanges": true
}
```

## <a name="properties"></a><span data-ttu-id="a1d3b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a1d3b-107">Properties</span></span>

| <span data-ttu-id="a1d3b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a1d3b-108">Property</span></span> | <span data-ttu-id="a1d3b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a1d3b-109">Type</span></span>  | <span data-ttu-id="a1d3b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a1d3b-110">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="a1d3b-111">id</span><span class="sxs-lookup"><span data-stu-id="a1d3b-111">id</span></span>  | <span data-ttu-id="a1d3b-112">строка</span><span class="sxs-lookup"><span data-stu-id="a1d3b-112">string</span></span> | <span data-ttu-id="a1d3b-113">Идентификатор сеанса книги.</span><span class="sxs-lookup"><span data-stu-id="a1d3b-113">Id of the workbook session.</span></span> |
| <span data-ttu-id="a1d3b-114">persistChanges</span><span class="sxs-lookup"><span data-stu-id="a1d3b-114">persistChanges</span></span> | <span data-ttu-id="a1d3b-115">boolean</span><span class="sxs-lookup"><span data-stu-id="a1d3b-115">boolean</span></span> |  <span data-ttu-id="a1d3b-116">Имеет значение `true` для сохраняемого сеанса.</span><span class="sxs-lookup"><span data-stu-id="a1d3b-116">`true` for persistent session.</span></span> <span data-ttu-id="a1d3b-117">Имеет значение `false` для несохраняемого сеанса (режим просмотра)</span><span class="sxs-lookup"><span data-stu-id="a1d3b-117">`false` for non-persistent session (view mode)</span></span> |

