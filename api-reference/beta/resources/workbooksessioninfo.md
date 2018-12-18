---
title: Тип ресурса workbookSessionInfo
description: Предоставляет сведения о сеансе книги.
author: lumine2008
ms.openlocfilehash: 5a86fd4dfd653f16445eeccad8478db56db0ac5f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316844"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="1e34d-103">Тип ресурса workbookSessionInfo</span><span class="sxs-lookup"><span data-stu-id="1e34d-103">workbookSessionInfo resource type</span></span>

<span data-ttu-id="1e34d-104">Предоставляет сведения о сеансе книги.</span><span class="sxs-lookup"><span data-stu-id="1e34d-104">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="1e34d-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="1e34d-105">JSON representation</span></span>

<span data-ttu-id="1e34d-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="1e34d-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="1e34d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1e34d-107">Properties</span></span>

| <span data-ttu-id="1e34d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1e34d-108">Property</span></span> | <span data-ttu-id="1e34d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1e34d-109">Type</span></span>  | <span data-ttu-id="1e34d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1e34d-110">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="1e34d-111">id</span><span class="sxs-lookup"><span data-stu-id="1e34d-111">id</span></span>  | <span data-ttu-id="1e34d-112">строка</span><span class="sxs-lookup"><span data-stu-id="1e34d-112">string</span></span> | <span data-ttu-id="1e34d-113">Идентификатор сеанса книги.</span><span class="sxs-lookup"><span data-stu-id="1e34d-113">Id of the workbook session.</span></span> |
| <span data-ttu-id="1e34d-114">persistChanges</span><span class="sxs-lookup"><span data-stu-id="1e34d-114">persistChanges</span></span> | <span data-ttu-id="1e34d-115">строка</span><span class="sxs-lookup"><span data-stu-id="1e34d-115">string</span></span> |  <span data-ttu-id="1e34d-116">Имеет значение `true` для сохраняемого сеанса.</span><span class="sxs-lookup"><span data-stu-id="1e34d-116">`true` for persistent session.</span></span> <span data-ttu-id="1e34d-117">Имеет значение `false` для несохраняемого сеанса (режим просмотра)</span><span class="sxs-lookup"><span data-stu-id="1e34d-117">`false` for non-persistent session (view mode)</span></span> |

