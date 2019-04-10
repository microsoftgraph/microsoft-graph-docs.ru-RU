---
title: Тип ресурса Рискюсерхисторитем
description: ''
author: ''
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7143fffecee52747109674e81e5bfbd9860df7f9
ms.sourcegitcommit: 9fd437a77da99d8436d6c852edd99a9ba873f8cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/09/2019
ms.locfileid: "31688513"
---
# <a name="riskyuserhistoryitem-resource-type"></a><span data-ttu-id="b3c83-102">Тип ресурса Рискюсерхисторитем</span><span class="sxs-lookup"><span data-stu-id="b3c83-102">riskyUserHistoryItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="b3c83-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="b3c83-103">Properties</span></span>

| <span data-ttu-id="b3c83-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="b3c83-104">Property</span></span>       | <span data-ttu-id="b3c83-105">Тип</span><span class="sxs-lookup"><span data-stu-id="b3c83-105">Type</span></span>    | <span data-ttu-id="b3c83-106">Описание</span><span class="sxs-lookup"><span data-stu-id="b3c83-106">Description</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="b3c83-107">userId</span><span class="sxs-lookup"><span data-stu-id="b3c83-107">userId</span></span>         | <span data-ttu-id="b3c83-108">string</span><span class="sxs-lookup"><span data-stu-id="b3c83-108">string</span></span>  |             |
| <span data-ttu-id="b3c83-109">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="b3c83-109">initiatedBy</span></span>    | <span data-ttu-id="b3c83-110">bool</span><span class="sxs-lookup"><span data-stu-id="b3c83-110">bool</span></span>    |             |
| <span data-ttu-id="b3c83-111">activity</span><span class="sxs-lookup"><span data-stu-id="b3c83-111">activity</span></span>       | [<span data-ttu-id="b3c83-112">Рискусерактивити</span><span class="sxs-lookup"><span data-stu-id="b3c83-112">riskUserActivity</span></span>](riskuseractivity.md)| |

## <a name="json-representation"></a><span data-ttu-id="b3c83-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b3c83-113">JSON representation</span></span>

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
