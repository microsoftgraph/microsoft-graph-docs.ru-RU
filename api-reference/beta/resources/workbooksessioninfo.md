---
title: Тип ресурса workbookSessionInfo
description: Предоставляет сведения о сеансе книги.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 6d0565edea02d0333f6aa3b97b376ea3c7f32c68
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519150"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="61757-103">Тип ресурса workbookSessionInfo</span><span class="sxs-lookup"><span data-stu-id="61757-103">workbookSessionInfo resource type</span></span>

<span data-ttu-id="61757-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="61757-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="61757-105">Предоставляет сведения о сеансе книги.</span><span class="sxs-lookup"><span data-stu-id="61757-105">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="61757-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="61757-106">JSON representation</span></span>

<span data-ttu-id="61757-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="61757-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="61757-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="61757-108">Properties</span></span>

| <span data-ttu-id="61757-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="61757-109">Property</span></span> | <span data-ttu-id="61757-110">Тип</span><span class="sxs-lookup"><span data-stu-id="61757-110">Type</span></span>  | <span data-ttu-id="61757-111">Описание</span><span class="sxs-lookup"><span data-stu-id="61757-111">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="61757-112">id</span><span class="sxs-lookup"><span data-stu-id="61757-112">id</span></span>  | <span data-ttu-id="61757-113">строка</span><span class="sxs-lookup"><span data-stu-id="61757-113">string</span></span> | <span data-ttu-id="61757-114">Идентификатор сеанса книги.</span><span class="sxs-lookup"><span data-stu-id="61757-114">Id of the workbook session.</span></span> |
| <span data-ttu-id="61757-115">persistChanges</span><span class="sxs-lookup"><span data-stu-id="61757-115">persistChanges</span></span> | <span data-ttu-id="61757-116">строка</span><span class="sxs-lookup"><span data-stu-id="61757-116">string</span></span> |  <span data-ttu-id="61757-117">Имеет значение `true` для сохраняемого сеанса.</span><span class="sxs-lookup"><span data-stu-id="61757-117">`true` for persistent session.</span></span> <span data-ttu-id="61757-118">Имеет значение `false` для несохраняемого сеанса (режим просмотра)</span><span class="sxs-lookup"><span data-stu-id="61757-118">`false` for non-persistent session (view mode)</span></span> |

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
