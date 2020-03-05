---
title: Тип ресурса workbookSessionInfo
description: Предоставляет сведения о сеансе книги.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 1e9746f27a23b12a3bfdf3168cd271c7f2cbc0d2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446694"
---
# <a name="workbooksessioninfo-resource-type"></a><span data-ttu-id="d6bcc-103">Тип ресурса workbookSessionInfo</span><span class="sxs-lookup"><span data-stu-id="d6bcc-103">workbookSessionInfo resource type</span></span>

<span data-ttu-id="d6bcc-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d6bcc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d6bcc-105">Предоставляет сведения о сеансе книги.</span><span class="sxs-lookup"><span data-stu-id="d6bcc-105">Provides information about workbook session.</span></span>


## <a name="json-representation"></a><span data-ttu-id="d6bcc-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d6bcc-106">JSON representation</span></span>

<span data-ttu-id="d6bcc-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="d6bcc-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="d6bcc-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d6bcc-108">Properties</span></span>

| <span data-ttu-id="d6bcc-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d6bcc-109">Property</span></span> | <span data-ttu-id="d6bcc-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d6bcc-110">Type</span></span>  | <span data-ttu-id="d6bcc-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d6bcc-111">Description</span></span>                               |
|:---------|:------|:------------------------------------------|
| <span data-ttu-id="d6bcc-112">id</span><span class="sxs-lookup"><span data-stu-id="d6bcc-112">id</span></span>  | <span data-ttu-id="d6bcc-113">строка</span><span class="sxs-lookup"><span data-stu-id="d6bcc-113">string</span></span> | <span data-ttu-id="d6bcc-114">Идентификатор сеанса книги.</span><span class="sxs-lookup"><span data-stu-id="d6bcc-114">Id of the workbook session.</span></span> |
| <span data-ttu-id="d6bcc-115">persistChanges</span><span class="sxs-lookup"><span data-stu-id="d6bcc-115">persistChanges</span></span> | <span data-ttu-id="d6bcc-116">boolean</span><span class="sxs-lookup"><span data-stu-id="d6bcc-116">boolean</span></span> |  <span data-ttu-id="d6bcc-117">Имеет значение `true` для сохраняемого сеанса.</span><span class="sxs-lookup"><span data-stu-id="d6bcc-117">`true` for persistent session.</span></span> <span data-ttu-id="d6bcc-118">Имеет значение `false` для несохраняемого сеанса (режим просмотра)</span><span class="sxs-lookup"><span data-stu-id="d6bcc-118">`false` for non-persistent session (view mode)</span></span> |

