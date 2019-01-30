---
title: Тип ресурса workbookSessionInfo
description: Предоставляет сведения о сеансе книги.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: a2975fdf58d0f1d3a72f1f76853125d0a98bb485
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642221"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="f073e-103">Тип ресурса workbookSessionInfo</span><span class="sxs-lookup"><span data-stu-id="f073e-103">workbookSessionInfo resource type</span></span>

<span data-ttu-id="f073e-104">Предоставляет сведения о сеансе книги.</span><span class="sxs-lookup"><span data-stu-id="f073e-104">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="f073e-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f073e-105">JSON representation</span></span>

<span data-ttu-id="f073e-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="f073e-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="f073e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f073e-107">Properties</span></span>

| <span data-ttu-id="f073e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f073e-108">Property</span></span> | <span data-ttu-id="f073e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f073e-109">Type</span></span>  | <span data-ttu-id="f073e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f073e-110">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="f073e-111">id</span><span class="sxs-lookup"><span data-stu-id="f073e-111">id</span></span>  | <span data-ttu-id="f073e-112">строка</span><span class="sxs-lookup"><span data-stu-id="f073e-112">string</span></span> | <span data-ttu-id="f073e-113">Идентификатор сеанса книги.</span><span class="sxs-lookup"><span data-stu-id="f073e-113">Id of the workbook session.</span></span> |
| <span data-ttu-id="f073e-114">persistChanges</span><span class="sxs-lookup"><span data-stu-id="f073e-114">persistChanges</span></span> | <span data-ttu-id="f073e-115">строка</span><span class="sxs-lookup"><span data-stu-id="f073e-115">string</span></span> |  <span data-ttu-id="f073e-116">Имеет значение `true` для сохраняемого сеанса.</span><span class="sxs-lookup"><span data-stu-id="f073e-116">`true` for persistent session.</span></span> <span data-ttu-id="f073e-117">Имеет значение `false` для несохраняемого сеанса (режим просмотра)</span><span class="sxs-lookup"><span data-stu-id="f073e-117">`false` for non-persistent session (view mode)</span></span> |

