---
title: Тип ресурса Акцессревиеврекурренцесеттингс
description: ''
localization_priority: Normal
ms.openlocfilehash: 1a5235639209830d36cf69c027cfd309fab09c3e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348421"
---
# <a name="accessreviewrecurrencesettings-resource-type"></a><span data-ttu-id="c1648-102">Тип ресурса Акцессревиеврекурренцесеттингс</span><span class="sxs-lookup"><span data-stu-id="c1648-102">accessReviewRecurrenceSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="properties"></a><span data-ttu-id="c1648-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="c1648-103">Properties</span></span>
|<span data-ttu-id="c1648-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="c1648-104">Property</span></span>|<span data-ttu-id="c1648-105">Тип</span><span class="sxs-lookup"><span data-stu-id="c1648-105">Type</span></span>|<span data-ttu-id="c1648-106">Описание</span><span class="sxs-lookup"><span data-stu-id="c1648-106">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="c1648-107">recurrenceType</span><span class="sxs-lookup"><span data-stu-id="c1648-107">recurrenceType</span></span> | <span data-ttu-id="c1648-108">string</span><span class="sxs-lookup"><span data-stu-id="c1648-108">string</span></span> |  |
| <span data-ttu-id="c1648-109">Рекурренцеендтипе</span><span class="sxs-lookup"><span data-stu-id="c1648-109">recurrenceEndType</span></span> | <span data-ttu-id="c1648-110">string</span><span class="sxs-lookup"><span data-stu-id="c1648-110">string</span></span> |  |
| <span data-ttu-id="c1648-111">Дуратиониндайс</span><span class="sxs-lookup"><span data-stu-id="c1648-111">durationInDays</span></span> | <span data-ttu-id="c1648-112">Int32</span><span class="sxs-lookup"><span data-stu-id="c1648-112">Int32</span></span> |  |
| <span data-ttu-id="c1648-113">Рекурренцекаунт</span><span class="sxs-lookup"><span data-stu-id="c1648-113">recurrenceCount</span></span> | <span data-ttu-id="c1648-114">Int32</span><span class="sxs-lookup"><span data-stu-id="c1648-114">Int32</span></span> |  |

## <a name="relationships"></a><span data-ttu-id="c1648-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="c1648-115">Relationships</span></span>
<span data-ttu-id="c1648-116">Нет</span><span class="sxs-lookup"><span data-stu-id="c1648-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c1648-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c1648-117">JSON Representation</span></span>
<span data-ttu-id="c1648-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c1648-118">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewRecurrenceSettings"
}-->
``` json
{
    "recurrenceType":"string",
    "recurrenceEndType":"string",
    "durationInDays":"Int32",
    "recurrenceCount":"Int32"
}
```



