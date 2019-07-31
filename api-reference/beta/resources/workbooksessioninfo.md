---
title: Тип ресурса workbookSessionInfo
description: Предоставляет сведения о сеансе книги.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 3b2d52b6389c6fc00eb0bf3b3b6d81774f6f882a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35963915"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="121c6-103">Тип ресурса workbookSessionInfo</span><span class="sxs-lookup"><span data-stu-id="121c6-103">workbookSessionInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="121c6-104">Предоставляет сведения о сеансе книги.</span><span class="sxs-lookup"><span data-stu-id="121c6-104">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="121c6-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="121c6-105">JSON representation</span></span>

<span data-ttu-id="121c6-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="121c6-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="121c6-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="121c6-107">Properties</span></span>

| <span data-ttu-id="121c6-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="121c6-108">Property</span></span> | <span data-ttu-id="121c6-109">Тип</span><span class="sxs-lookup"><span data-stu-id="121c6-109">Type</span></span>  | <span data-ttu-id="121c6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="121c6-110">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="121c6-111">id</span><span class="sxs-lookup"><span data-stu-id="121c6-111">id</span></span>  | <span data-ttu-id="121c6-112">string</span><span class="sxs-lookup"><span data-stu-id="121c6-112">string</span></span> | <span data-ttu-id="121c6-113">Идентификатор сеанса книги.</span><span class="sxs-lookup"><span data-stu-id="121c6-113">Id of the workbook session.</span></span> |
| <span data-ttu-id="121c6-114">persistChanges</span><span class="sxs-lookup"><span data-stu-id="121c6-114">persistChanges</span></span> | <span data-ttu-id="121c6-115">строка</span><span class="sxs-lookup"><span data-stu-id="121c6-115">string</span></span> |  <span data-ttu-id="121c6-116">Имеет значение `true` для сохраняемого сеанса.</span><span class="sxs-lookup"><span data-stu-id="121c6-116">`true` for persistent session.</span></span> <span data-ttu-id="121c6-117">Имеет значение `false` для несохраняемого сеанса (режим просмотра)</span><span class="sxs-lookup"><span data-stu-id="121c6-117">`false` for non-persistent session (view mode)</span></span> |

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
