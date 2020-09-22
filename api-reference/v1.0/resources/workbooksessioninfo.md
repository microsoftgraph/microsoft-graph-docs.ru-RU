---
title: Тип ресурса workbookSessionInfo
description: Предоставляет сведения о сеансе книги.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 5d5b75d3062b087848f804c0f89726c67783c540
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015108"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="22d0e-103">Тип ресурса workbookSessionInfo</span><span class="sxs-lookup"><span data-stu-id="22d0e-103">workbookSessionInfo resource type</span></span>

<span data-ttu-id="22d0e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22d0e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="22d0e-105">Предоставляет сведения о сеансе книги.</span><span class="sxs-lookup"><span data-stu-id="22d0e-105">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="22d0e-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="22d0e-106">JSON representation</span></span>

<span data-ttu-id="22d0e-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="22d0e-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="22d0e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="22d0e-108">Properties</span></span>

| <span data-ttu-id="22d0e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="22d0e-109">Property</span></span> | <span data-ttu-id="22d0e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="22d0e-110">Type</span></span>  | <span data-ttu-id="22d0e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="22d0e-111">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="22d0e-112">id</span><span class="sxs-lookup"><span data-stu-id="22d0e-112">id</span></span>  | <span data-ttu-id="22d0e-113">string</span><span class="sxs-lookup"><span data-stu-id="22d0e-113">string</span></span> | <span data-ttu-id="22d0e-114">Идентификатор сеанса книги.</span><span class="sxs-lookup"><span data-stu-id="22d0e-114">Id of the workbook session.</span></span> |
| <span data-ttu-id="22d0e-115">persistChanges</span><span class="sxs-lookup"><span data-stu-id="22d0e-115">persistChanges</span></span> | <span data-ttu-id="22d0e-116">boolean</span><span class="sxs-lookup"><span data-stu-id="22d0e-116">boolean</span></span> |  <span data-ttu-id="22d0e-117">Имеет значение `true` для сохраняемого сеанса.</span><span class="sxs-lookup"><span data-stu-id="22d0e-117">`true` for persistent session.</span></span> <span data-ttu-id="22d0e-118">Имеет значение `false` для несохраняемого сеанса (режим просмотра)</span><span class="sxs-lookup"><span data-stu-id="22d0e-118">`false` for non-persistent session (view mode)</span></span> |


