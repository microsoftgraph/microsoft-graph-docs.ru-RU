---
title: Тип ресурса workbookSessionInfo
description: Предоставляет сведения о сеансе книги.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: a2975fdf58d0f1d3a72f1f76853125d0a98bb485
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962452"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="ff72a-103">Тип ресурса workbookSessionInfo</span><span class="sxs-lookup"><span data-stu-id="ff72a-103">workbookSessionInfo resource type</span></span>

<span data-ttu-id="ff72a-104">Предоставляет сведения о сеансе книги.</span><span class="sxs-lookup"><span data-stu-id="ff72a-104">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="ff72a-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ff72a-105">JSON representation</span></span>

<span data-ttu-id="ff72a-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="ff72a-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="ff72a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ff72a-107">Properties</span></span>

| <span data-ttu-id="ff72a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ff72a-108">Property</span></span> | <span data-ttu-id="ff72a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ff72a-109">Type</span></span>  | <span data-ttu-id="ff72a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ff72a-110">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="ff72a-111">id</span><span class="sxs-lookup"><span data-stu-id="ff72a-111">id</span></span>  | <span data-ttu-id="ff72a-112">строка</span><span class="sxs-lookup"><span data-stu-id="ff72a-112">string</span></span> | <span data-ttu-id="ff72a-113">Идентификатор сеанса книги.</span><span class="sxs-lookup"><span data-stu-id="ff72a-113">Id of the workbook session.</span></span> |
| <span data-ttu-id="ff72a-114">persistChanges</span><span class="sxs-lookup"><span data-stu-id="ff72a-114">persistChanges</span></span> | <span data-ttu-id="ff72a-115">строка</span><span class="sxs-lookup"><span data-stu-id="ff72a-115">string</span></span> |  <span data-ttu-id="ff72a-116">Имеет значение `true` для сохраняемого сеанса.</span><span class="sxs-lookup"><span data-stu-id="ff72a-116">`true` for persistent session.</span></span> <span data-ttu-id="ff72a-117">Имеет значение `false` для несохраняемого сеанса (режим просмотра)</span><span class="sxs-lookup"><span data-stu-id="ff72a-117">`false` for non-persistent session (view mode)</span></span> |

