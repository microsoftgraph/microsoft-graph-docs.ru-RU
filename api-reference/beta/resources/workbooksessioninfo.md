---
title: Тип ресурса workbookSessionInfo
description: Предоставляет сведения о сеансе книги.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 3035574b92dfa703b926a81163efbb7f6eff764b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345789"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="22e32-103">Тип ресурса workbookSessionInfo</span><span class="sxs-lookup"><span data-stu-id="22e32-103">workbookSessionInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22e32-104">Предоставляет сведения о сеансе книги.</span><span class="sxs-lookup"><span data-stu-id="22e32-104">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="22e32-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="22e32-105">JSON representation</span></span>

<span data-ttu-id="22e32-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="22e32-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="22e32-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="22e32-107">Properties</span></span>

| <span data-ttu-id="22e32-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="22e32-108">Property</span></span> | <span data-ttu-id="22e32-109">Тип</span><span class="sxs-lookup"><span data-stu-id="22e32-109">Type</span></span>  | <span data-ttu-id="22e32-110">Описание</span><span class="sxs-lookup"><span data-stu-id="22e32-110">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="22e32-111">id</span><span class="sxs-lookup"><span data-stu-id="22e32-111">id</span></span>  | <span data-ttu-id="22e32-112">строка</span><span class="sxs-lookup"><span data-stu-id="22e32-112">string</span></span> | <span data-ttu-id="22e32-113">Идентификатор сеанса книги.</span><span class="sxs-lookup"><span data-stu-id="22e32-113">Id of the workbook session.</span></span> |
| <span data-ttu-id="22e32-114">persistChanges</span><span class="sxs-lookup"><span data-stu-id="22e32-114">persistChanges</span></span> | <span data-ttu-id="22e32-115">строка</span><span class="sxs-lookup"><span data-stu-id="22e32-115">string</span></span> |  <span data-ttu-id="22e32-116">Имеет значение `true` для сохраняемого сеанса.</span><span class="sxs-lookup"><span data-stu-id="22e32-116">`true` for persistent session.</span></span> <span data-ttu-id="22e32-117">Имеет значение `false` для несохраняемого сеанса (режим просмотра)</span><span class="sxs-lookup"><span data-stu-id="22e32-117">`false` for non-persistent session (view mode)</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "workbookSessionInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
