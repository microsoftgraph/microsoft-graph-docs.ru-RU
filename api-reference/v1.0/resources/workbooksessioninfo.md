---
title: Тип ресурса workbookSessionInfo
description: Предоставляет сведения о сеансе книги.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 502781c4049c9451f5ed67ff97222abf4df462d7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960275"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="ed96e-103">Тип ресурса workbookSessionInfo</span><span class="sxs-lookup"><span data-stu-id="ed96e-103">workbookSessionInfo resource type</span></span>

<span data-ttu-id="ed96e-104">Предоставляет сведения о сеансе книги.</span><span class="sxs-lookup"><span data-stu-id="ed96e-104">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="ed96e-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ed96e-105">JSON representation</span></span>

<span data-ttu-id="ed96e-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="ed96e-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="ed96e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ed96e-107">Properties</span></span>

| <span data-ttu-id="ed96e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ed96e-108">Property</span></span> | <span data-ttu-id="ed96e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ed96e-109">Type</span></span>  | <span data-ttu-id="ed96e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ed96e-110">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="ed96e-111">id</span><span class="sxs-lookup"><span data-stu-id="ed96e-111">id</span></span>  | <span data-ttu-id="ed96e-112">строка</span><span class="sxs-lookup"><span data-stu-id="ed96e-112">string</span></span> | <span data-ttu-id="ed96e-113">Идентификатор сеанса книги.</span><span class="sxs-lookup"><span data-stu-id="ed96e-113">Id of the workbook session.</span></span> |
| <span data-ttu-id="ed96e-114">persistChanges</span><span class="sxs-lookup"><span data-stu-id="ed96e-114">persistChanges</span></span> | <span data-ttu-id="ed96e-115">boolean</span><span class="sxs-lookup"><span data-stu-id="ed96e-115">boolean</span></span> |  <span data-ttu-id="ed96e-116">Имеет значение `true` для сохраняемого сеанса.</span><span class="sxs-lookup"><span data-stu-id="ed96e-116">`true` for persistent session.</span></span> <span data-ttu-id="ed96e-117">Имеет значение `false` для несохраняемого сеанса (режим просмотра)</span><span class="sxs-lookup"><span data-stu-id="ed96e-117">`false` for non-persistent session (view mode)</span></span> |

