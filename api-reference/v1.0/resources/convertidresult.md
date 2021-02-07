---
title: Тип ресурса convertIdResult
description: Результат преобразования формата ID, выполненного функцией translateExchangeIds.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: abheek-das
ms.openlocfilehash: 1710c437421426b4bd072e3c654df7d076d0f9f7
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135156"
---
# <a name="convertidresult-resource-type"></a><span data-ttu-id="a5da3-103">Тип ресурса convertIdResult</span><span class="sxs-lookup"><span data-stu-id="a5da3-103">convertIdResult resource type</span></span>

<span data-ttu-id="a5da3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5da3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a5da3-105">Результат преобразования формата ID, выполненного [функцией translateExchangeIds.](../api/user-translateexchangeids.md)</span><span class="sxs-lookup"><span data-stu-id="a5da3-105">The result of an ID format conversion performed by the [translateExchangeIds](../api/user-translateexchangeids.md) function.</span></span>

## <a name="properties"></a><span data-ttu-id="a5da3-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a5da3-106">Properties</span></span>

| <span data-ttu-id="a5da3-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a5da3-107">Property</span></span> | <span data-ttu-id="a5da3-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a5da3-108">Type</span></span> | <span data-ttu-id="a5da3-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a5da3-109">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="a5da3-110">sourceId</span><span class="sxs-lookup"><span data-stu-id="a5da3-110">sourceId</span></span> | <span data-ttu-id="a5da3-111">String</span><span class="sxs-lookup"><span data-stu-id="a5da3-111">String</span></span> | <span data-ttu-id="a5da3-112">Идентификатор, который был преобразован.</span><span class="sxs-lookup"><span data-stu-id="a5da3-112">The identifier that was converted.</span></span> <span data-ttu-id="a5da3-113">Это значение является исходным, не преобразованным идентификатором.</span><span class="sxs-lookup"><span data-stu-id="a5da3-113">This value is the original, un-converted identifier.</span></span> |
| <span data-ttu-id="a5da3-114">targetId</span><span class="sxs-lookup"><span data-stu-id="a5da3-114">targetId</span></span> | <span data-ttu-id="a5da3-115">String</span><span class="sxs-lookup"><span data-stu-id="a5da3-115">String</span></span> | <span data-ttu-id="a5da3-116">Преобразованный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="a5da3-116">The converted identifier.</span></span> <span data-ttu-id="a5da3-117">Это значение не будет представлено, если преобразование не удалось.</span><span class="sxs-lookup"><span data-stu-id="a5da3-117">This value is not present if the conversion failed.</span></span> |
| <span data-ttu-id="a5da3-118">errorDetails</span><span class="sxs-lookup"><span data-stu-id="a5da3-118">errorDetails</span></span> | [<span data-ttu-id="a5da3-119">genericError</span><span class="sxs-lookup"><span data-stu-id="a5da3-119">genericError</span></span>](genericerror.md) | <span data-ttu-id="a5da3-120">Объект ошибки, указывающий причину сбоя преобразования.</span><span class="sxs-lookup"><span data-stu-id="a5da3-120">An error object indicating the reason for the conversion failure.</span></span> <span data-ttu-id="a5da3-121">Это значение не будет представлено, если преобразование успешно.</span><span class="sxs-lookup"><span data-stu-id="a5da3-121">This value is not present if the conversion succeeded.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a5da3-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a5da3-122">JSON representation</span></span>

<span data-ttu-id="a5da3-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a5da3-123">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "targetId",
    "errorDetails"
  ],
  "@odata.type": "microsoft.graph.convertIdResult"
}-->

```json
{
  "sourceId": "String",
  "targetId": "String",
  "errorDetails": {
    "@odata.type": "microsoft.graph.genericError"
  }
}
```

