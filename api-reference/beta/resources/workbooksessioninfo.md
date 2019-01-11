---
title: Тип ресурса workbookSessionInfo
description: Предоставляет сведения о сеансе книги.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 25812d48626c7dc5e468915f7308941a4f74b38e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860965"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="25498-103">Тип ресурса workbookSessionInfo</span><span class="sxs-lookup"><span data-stu-id="25498-103">workbookSessionInfo resource type</span></span>

<span data-ttu-id="25498-104">Предоставляет сведения о сеансе книги.</span><span class="sxs-lookup"><span data-stu-id="25498-104">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="25498-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="25498-105">JSON representation</span></span>

<span data-ttu-id="25498-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="25498-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="25498-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="25498-107">Properties</span></span>

| <span data-ttu-id="25498-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="25498-108">Property</span></span> | <span data-ttu-id="25498-109">Тип</span><span class="sxs-lookup"><span data-stu-id="25498-109">Type</span></span>  | <span data-ttu-id="25498-110">Описание</span><span class="sxs-lookup"><span data-stu-id="25498-110">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="25498-111">id</span><span class="sxs-lookup"><span data-stu-id="25498-111">id</span></span>  | <span data-ttu-id="25498-112">строка</span><span class="sxs-lookup"><span data-stu-id="25498-112">string</span></span> | <span data-ttu-id="25498-113">Идентификатор сеанса книги.</span><span class="sxs-lookup"><span data-stu-id="25498-113">Id of the workbook session.</span></span> |
| <span data-ttu-id="25498-114">persistChanges</span><span class="sxs-lookup"><span data-stu-id="25498-114">persistChanges</span></span> | <span data-ttu-id="25498-115">строка</span><span class="sxs-lookup"><span data-stu-id="25498-115">string</span></span> |  <span data-ttu-id="25498-116">Имеет значение `true` для сохраняемого сеанса.</span><span class="sxs-lookup"><span data-stu-id="25498-116">`true` for persistent session.</span></span> <span data-ttu-id="25498-117">Имеет значение `false` для несохраняемого сеанса (режим просмотра)</span><span class="sxs-lookup"><span data-stu-id="25498-117">`false` for non-persistent session (view mode)</span></span> |

