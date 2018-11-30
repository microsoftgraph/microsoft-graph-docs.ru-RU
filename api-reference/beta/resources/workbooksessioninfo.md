---
title: Тип ресурса workbookSessionInfo
description: Предоставляет сведения о сеансе книги.
ms.openlocfilehash: c04afe17c10edd8b136465d6d7ae3dbedb6307ed
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078162"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="c8818-103">Тип ресурса workbookSessionInfo</span><span class="sxs-lookup"><span data-stu-id="c8818-103">workbookSessionInfo resource type</span></span>

<span data-ttu-id="c8818-104">Предоставляет сведения о сеансе книги.</span><span class="sxs-lookup"><span data-stu-id="c8818-104">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="c8818-105">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c8818-105">JSON representation</span></span>

<span data-ttu-id="c8818-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="c8818-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="c8818-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c8818-107">Properties</span></span>

| <span data-ttu-id="c8818-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c8818-108">Property</span></span> | <span data-ttu-id="c8818-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c8818-109">Type</span></span>  | <span data-ttu-id="c8818-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c8818-110">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="c8818-111">id</span><span class="sxs-lookup"><span data-stu-id="c8818-111">id</span></span>  | <span data-ttu-id="c8818-112">строка</span><span class="sxs-lookup"><span data-stu-id="c8818-112">string</span></span> | <span data-ttu-id="c8818-113">Идентификатор сеанса книги.</span><span class="sxs-lookup"><span data-stu-id="c8818-113">Id of the workbook session.</span></span> |
| <span data-ttu-id="c8818-114">persistChanges</span><span class="sxs-lookup"><span data-stu-id="c8818-114">persistChanges</span></span> | <span data-ttu-id="c8818-115">строка</span><span class="sxs-lookup"><span data-stu-id="c8818-115">string</span></span> |  <span data-ttu-id="c8818-116">Имеет значение `true` для сохраняемого сеанса.</span><span class="sxs-lookup"><span data-stu-id="c8818-116">`true` for persistent session.</span></span> <span data-ttu-id="c8818-117">Имеет значение `false` для несохраняемого сеанса (режим просмотра)</span><span class="sxs-lookup"><span data-stu-id="c8818-117">`false` for non-persistent session (view mode)</span></span> |

