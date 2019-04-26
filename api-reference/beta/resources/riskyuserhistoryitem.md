---
title: Тип ресурса Рискюсерхисторитем
description: ''
author: ''
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7143fffecee52747109674e81e5bfbd9860df7f9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343558"
---
# <a name="riskyuserhistoryitem-resource-type"></a><span data-ttu-id="ce42f-102">Тип ресурса Рискюсерхисторитем</span><span class="sxs-lookup"><span data-stu-id="ce42f-102">riskyUserHistoryItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="ce42f-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="ce42f-103">Properties</span></span>

| <span data-ttu-id="ce42f-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="ce42f-104">Property</span></span>       | <span data-ttu-id="ce42f-105">Тип</span><span class="sxs-lookup"><span data-stu-id="ce42f-105">Type</span></span>    | <span data-ttu-id="ce42f-106">Описание</span><span class="sxs-lookup"><span data-stu-id="ce42f-106">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="ce42f-107">userId</span><span class="sxs-lookup"><span data-stu-id="ce42f-107">userId</span></span>         | <span data-ttu-id="ce42f-108">string</span><span class="sxs-lookup"><span data-stu-id="ce42f-108">string</span></span>  |             |
| <span data-ttu-id="ce42f-109">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="ce42f-109">initiatedBy</span></span>    | <span data-ttu-id="ce42f-110">bool</span><span class="sxs-lookup"><span data-stu-id="ce42f-110">bool</span></span>    |             |
| <span data-ttu-id="ce42f-111">activity</span><span class="sxs-lookup"><span data-stu-id="ce42f-111">activity</span></span>       | [<span data-ttu-id="ce42f-112">Рискусерактивити</span><span class="sxs-lookup"><span data-stu-id="ce42f-112">riskUserActivity</span></span>](riskuseractivity.md)| |

## <a name="json-representation"></a><span data-ttu-id="ce42f-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ce42f-113">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.riskyUserHistoryItem",
  "baseType": "microsoft.graph.riskyUser"
}-->

```json
{
    "userId": "string",
    "initiatedBy": "bool",
    "activity": {"@odata.type": "microsoft.graph.riskUserActivity"}
}
```


<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
   
  ]
}
-->
