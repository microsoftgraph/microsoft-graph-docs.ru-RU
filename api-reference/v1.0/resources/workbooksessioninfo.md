---
title: Тип ресурса workbookSessionInfo
description: Предоставляет сведения о сеансе книги.
author: lumine2008
ms.openlocfilehash: 1e097cad70a6058aab28ad85d7cf6b3c3b52ac75
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305987"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="6b837-103">Тип ресурса workbookSessionInfo</span><span class="sxs-lookup"><span data-stu-id="6b837-103">workbookSessionInfo resource type</span></span>

<span data-ttu-id="6b837-104">Предоставляет сведения о сеансе книги.</span><span class="sxs-lookup"><span data-stu-id="6b837-104">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="6b837-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="6b837-105">JSON representation</span></span>

<span data-ttu-id="6b837-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="6b837-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="6b837-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6b837-107">Properties</span></span>

| <span data-ttu-id="6b837-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6b837-108">Property</span></span> | <span data-ttu-id="6b837-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6b837-109">Type</span></span>  | <span data-ttu-id="6b837-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6b837-110">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="6b837-111">id</span><span class="sxs-lookup"><span data-stu-id="6b837-111">id</span></span>  | <span data-ttu-id="6b837-112">строка</span><span class="sxs-lookup"><span data-stu-id="6b837-112">string</span></span> | <span data-ttu-id="6b837-113">Идентификатор сеанса книги.</span><span class="sxs-lookup"><span data-stu-id="6b837-113">Id of the workbook session.</span></span> |
| <span data-ttu-id="6b837-114">persistChanges</span><span class="sxs-lookup"><span data-stu-id="6b837-114">persistChanges</span></span> | <span data-ttu-id="6b837-115">boolean</span><span class="sxs-lookup"><span data-stu-id="6b837-115">boolean</span></span> |  <span data-ttu-id="6b837-116">Имеет значение `true` для сохраняемого сеанса.</span><span class="sxs-lookup"><span data-stu-id="6b837-116">`true` for persistent session.</span></span> <span data-ttu-id="6b837-117">Имеет значение `false` для несохраняемого сеанса (режим просмотра)</span><span class="sxs-lookup"><span data-stu-id="6b837-117">`false` for non-persistent session (view mode)</span></span> |

