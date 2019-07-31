---
title: Тип ресурса Акцессревиеврекурренцесеттингс
description: ''
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsofit-identity-platform
author: ''
ms.openlocfilehash: 2bf71fe1c715eb96e98b0caf7720cc0d637ee33b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974545"
---
# <a name="accessreviewrecurrencesettings-resource-type"></a><span data-ttu-id="4c3d2-102">Тип ресурса Акцессревиеврекурренцесеттингс</span><span class="sxs-lookup"><span data-stu-id="4c3d2-102">accessReviewRecurrenceSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="properties"></a><span data-ttu-id="4c3d2-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="4c3d2-103">Properties</span></span>
|<span data-ttu-id="4c3d2-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c3d2-104">Property</span></span>|<span data-ttu-id="4c3d2-105">Тип</span><span class="sxs-lookup"><span data-stu-id="4c3d2-105">Type</span></span>|<span data-ttu-id="4c3d2-106">Описание</span><span class="sxs-lookup"><span data-stu-id="4c3d2-106">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="4c3d2-107">recurrenceType</span><span class="sxs-lookup"><span data-stu-id="4c3d2-107">recurrenceType</span></span> | <span data-ttu-id="4c3d2-108">string</span><span class="sxs-lookup"><span data-stu-id="4c3d2-108">string</span></span> |  |
| <span data-ttu-id="4c3d2-109">Рекурренцеендтипе</span><span class="sxs-lookup"><span data-stu-id="4c3d2-109">recurrenceEndType</span></span> | <span data-ttu-id="4c3d2-110">string</span><span class="sxs-lookup"><span data-stu-id="4c3d2-110">string</span></span> |  |
| <span data-ttu-id="4c3d2-111">Дуратиониндайс</span><span class="sxs-lookup"><span data-stu-id="4c3d2-111">durationInDays</span></span> | <span data-ttu-id="4c3d2-112">Int32</span><span class="sxs-lookup"><span data-stu-id="4c3d2-112">Int32</span></span> |  |
| <span data-ttu-id="4c3d2-113">Рекурренцекаунт</span><span class="sxs-lookup"><span data-stu-id="4c3d2-113">recurrenceCount</span></span> | <span data-ttu-id="4c3d2-114">Int32</span><span class="sxs-lookup"><span data-stu-id="4c3d2-114">Int32</span></span> |  |

## <a name="relationships"></a><span data-ttu-id="4c3d2-115">Отношения</span><span class="sxs-lookup"><span data-stu-id="4c3d2-115">Relationships</span></span>
<span data-ttu-id="4c3d2-116">Нет</span><span class="sxs-lookup"><span data-stu-id="4c3d2-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4c3d2-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4c3d2-117">JSON Representation</span></span>
<span data-ttu-id="4c3d2-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4c3d2-118">Here is a JSON representation of the resource.</span></span>
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



