---
title: Тип ресурса workbookSessionInfo
description: Предоставляет сведения о сеансе книги.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: f2e6b925e7cc1790b1c6d4f08bab02fa92f19936
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033336"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="7c149-103">Тип ресурса workbookSessionInfo</span><span class="sxs-lookup"><span data-stu-id="7c149-103">workbookSessionInfo resource type</span></span>

<span data-ttu-id="7c149-104">Предоставляет сведения о сеансе книги.</span><span class="sxs-lookup"><span data-stu-id="7c149-104">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="7c149-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7c149-105">JSON representation</span></span>

<span data-ttu-id="7c149-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="7c149-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="7c149-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7c149-107">Properties</span></span>

| <span data-ttu-id="7c149-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="7c149-108">Property</span></span> | <span data-ttu-id="7c149-109">Тип</span><span class="sxs-lookup"><span data-stu-id="7c149-109">Type</span></span>  | <span data-ttu-id="7c149-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7c149-110">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="7c149-111">id</span><span class="sxs-lookup"><span data-stu-id="7c149-111">id</span></span>  | <span data-ttu-id="7c149-112">string</span><span class="sxs-lookup"><span data-stu-id="7c149-112">string</span></span> | <span data-ttu-id="7c149-113">Идентификатор сеанса книги.</span><span class="sxs-lookup"><span data-stu-id="7c149-113">Id of the workbook session.</span></span> |
| <span data-ttu-id="7c149-114">persistChanges</span><span class="sxs-lookup"><span data-stu-id="7c149-114">persistChanges</span></span> | <span data-ttu-id="7c149-115">boolean</span><span class="sxs-lookup"><span data-stu-id="7c149-115">boolean</span></span> |  <span data-ttu-id="7c149-116">Имеет значение `true` для сохраняемого сеанса.</span><span class="sxs-lookup"><span data-stu-id="7c149-116">`true` for persistent session.</span></span> <span data-ttu-id="7c149-117">Имеет значение `false` для несохраняемого сеанса (режим просмотра)</span><span class="sxs-lookup"><span data-stu-id="7c149-117">`false` for non-persistent session (view mode)</span></span> |

