---
title: Тип ресурса workbookSessionInfo
description: Предоставляет сведения о сеансе книги.
ms.openlocfilehash: 84d0306a7a25aaa29e4f1eb9b87708cc97d6b50f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026290"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="a3582-103">Тип ресурса workbookSessionInfo</span><span class="sxs-lookup"><span data-stu-id="a3582-103">workbookSessionInfo resource type</span></span>

<span data-ttu-id="a3582-104">Предоставляет сведения о сеансе книги.</span><span class="sxs-lookup"><span data-stu-id="a3582-104">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="a3582-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a3582-105">JSON representation</span></span>

<span data-ttu-id="a3582-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="a3582-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="a3582-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a3582-107">Properties</span></span>

| <span data-ttu-id="a3582-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a3582-108">Property</span></span> | <span data-ttu-id="a3582-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a3582-109">Type</span></span>  | <span data-ttu-id="a3582-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a3582-110">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="a3582-111">id</span><span class="sxs-lookup"><span data-stu-id="a3582-111">id</span></span>  | <span data-ttu-id="a3582-112">строка</span><span class="sxs-lookup"><span data-stu-id="a3582-112">string</span></span> | <span data-ttu-id="a3582-113">Идентификатор сеанса книги.</span><span class="sxs-lookup"><span data-stu-id="a3582-113">Id of the workbook session.</span></span> |
| <span data-ttu-id="a3582-114">persistChanges</span><span class="sxs-lookup"><span data-stu-id="a3582-114">persistChanges</span></span> | <span data-ttu-id="a3582-115">boolean</span><span class="sxs-lookup"><span data-stu-id="a3582-115">boolean</span></span> |  <span data-ttu-id="a3582-116">Имеет значение `true` для сохраняемого сеанса.</span><span class="sxs-lookup"><span data-stu-id="a3582-116">`true` for persistent session.</span></span> <span data-ttu-id="a3582-117">Имеет значение `false` для несохраняемого сеанса (режим просмотра)</span><span class="sxs-lookup"><span data-stu-id="a3582-117">`false` for non-persistent session (view mode)</span></span> |

