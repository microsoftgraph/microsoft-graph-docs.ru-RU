---
title: Тип ресурса Акцессревиеврекурренцесеттингс
description: ''
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsofit-identity-platform
author: ''
ms.openlocfilehash: 807be44f256fa3a9080cc3cb458033726aadc107
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508473"
---
# <a name="accessreviewrecurrencesettings-resource-type"></a><span data-ttu-id="784ba-102">Тип ресурса Акцессревиеврекурренцесеттингс</span><span class="sxs-lookup"><span data-stu-id="784ba-102">accessReviewRecurrenceSettings resource type</span></span>

<span data-ttu-id="784ba-103">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="784ba-103">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="properties"></a><span data-ttu-id="784ba-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="784ba-104">Properties</span></span>
|<span data-ttu-id="784ba-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="784ba-105">Property</span></span>|<span data-ttu-id="784ba-106">Тип</span><span class="sxs-lookup"><span data-stu-id="784ba-106">Type</span></span>|<span data-ttu-id="784ba-107">Описание</span><span class="sxs-lookup"><span data-stu-id="784ba-107">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="784ba-108">recurrenceType</span><span class="sxs-lookup"><span data-stu-id="784ba-108">recurrenceType</span></span> | <span data-ttu-id="784ba-109">строка</span><span class="sxs-lookup"><span data-stu-id="784ba-109">string</span></span> |  |
| <span data-ttu-id="784ba-110">рекурренцеендтипе</span><span class="sxs-lookup"><span data-stu-id="784ba-110">recurrenceEndType</span></span> | <span data-ttu-id="784ba-111">строка</span><span class="sxs-lookup"><span data-stu-id="784ba-111">string</span></span> |  |
| <span data-ttu-id="784ba-112">дуратиониндайс</span><span class="sxs-lookup"><span data-stu-id="784ba-112">durationInDays</span></span> | <span data-ttu-id="784ba-113">Int32</span><span class="sxs-lookup"><span data-stu-id="784ba-113">Int32</span></span> |  |
| <span data-ttu-id="784ba-114">рекурренцекаунт</span><span class="sxs-lookup"><span data-stu-id="784ba-114">recurrenceCount</span></span> | <span data-ttu-id="784ba-115">Int32</span><span class="sxs-lookup"><span data-stu-id="784ba-115">Int32</span></span> |  |

## <a name="relationships"></a><span data-ttu-id="784ba-116">Связи</span><span class="sxs-lookup"><span data-stu-id="784ba-116">Relationships</span></span>
<span data-ttu-id="784ba-117">Нет</span><span class="sxs-lookup"><span data-stu-id="784ba-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="784ba-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="784ba-118">JSON Representation</span></span>
<span data-ttu-id="784ba-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="784ba-119">Here is a JSON representation of the resource.</span></span>
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



