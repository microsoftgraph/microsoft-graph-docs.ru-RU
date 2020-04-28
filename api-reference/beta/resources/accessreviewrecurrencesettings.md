---
title: Тип ресурса Акцессревиеврекурренцесеттингс
description: ''
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsofit-identity-platform
author: markwahl-msft
ms.openlocfilehash: 7c45a0b57d869acdb49c5a37f235232c70e8ec6f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43472238"
---
# <a name="accessreviewrecurrencesettings-resource-type"></a><span data-ttu-id="ad2e8-102">Тип ресурса Акцессревиеврекурренцесеттингс</span><span class="sxs-lookup"><span data-stu-id="ad2e8-102">accessReviewRecurrenceSettings resource type</span></span>

<span data-ttu-id="ad2e8-103">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad2e8-103">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="properties"></a><span data-ttu-id="ad2e8-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="ad2e8-104">Properties</span></span>
|<span data-ttu-id="ad2e8-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="ad2e8-105">Property</span></span>|<span data-ttu-id="ad2e8-106">Тип</span><span class="sxs-lookup"><span data-stu-id="ad2e8-106">Type</span></span>|<span data-ttu-id="ad2e8-107">Описание</span><span class="sxs-lookup"><span data-stu-id="ad2e8-107">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="ad2e8-108">recurrenceType</span><span class="sxs-lookup"><span data-stu-id="ad2e8-108">recurrenceType</span></span> | <span data-ttu-id="ad2e8-109">string</span><span class="sxs-lookup"><span data-stu-id="ad2e8-109">string</span></span> |  |
| <span data-ttu-id="ad2e8-110">рекурренцеендтипе</span><span class="sxs-lookup"><span data-stu-id="ad2e8-110">recurrenceEndType</span></span> | <span data-ttu-id="ad2e8-111">string</span><span class="sxs-lookup"><span data-stu-id="ad2e8-111">string</span></span> |  |
| <span data-ttu-id="ad2e8-112">дуратиониндайс</span><span class="sxs-lookup"><span data-stu-id="ad2e8-112">durationInDays</span></span> | <span data-ttu-id="ad2e8-113">Int32</span><span class="sxs-lookup"><span data-stu-id="ad2e8-113">Int32</span></span> |  |
| <span data-ttu-id="ad2e8-114">рекурренцекаунт</span><span class="sxs-lookup"><span data-stu-id="ad2e8-114">recurrenceCount</span></span> | <span data-ttu-id="ad2e8-115">Int32</span><span class="sxs-lookup"><span data-stu-id="ad2e8-115">Int32</span></span> |  |

## <a name="relationships"></a><span data-ttu-id="ad2e8-116">Связи</span><span class="sxs-lookup"><span data-stu-id="ad2e8-116">Relationships</span></span>
<span data-ttu-id="ad2e8-117">Нет</span><span class="sxs-lookup"><span data-stu-id="ad2e8-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ad2e8-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ad2e8-118">JSON Representation</span></span>
<span data-ttu-id="ad2e8-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ad2e8-119">Here is a JSON representation of the resource.</span></span>
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



