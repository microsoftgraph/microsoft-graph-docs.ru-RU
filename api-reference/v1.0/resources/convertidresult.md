---
title: Тип ресурса Конвертидресулт
description: Результат преобразования формата идентификатора, выполняемого функцией Транслатиксчанжеидс.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: svpsiva
ms.openlocfilehash: aa663420dd7b6e1c79e03af675b1f505c08cb875
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091854"
---
# <a name="convertidresult-resource-type"></a><span data-ttu-id="900d7-103">Тип ресурса Конвертидресулт</span><span class="sxs-lookup"><span data-stu-id="900d7-103">convertIdResult resource type</span></span>

<span data-ttu-id="900d7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="900d7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="900d7-105">Результат преобразования формата идентификатора, выполняемого функцией [транслатиксчанжеидс](../api/user-translateexchangeids.md) .</span><span class="sxs-lookup"><span data-stu-id="900d7-105">The result of an ID format conversion performed by the [translateExchangeIds](../api/user-translateexchangeids.md) function.</span></span>

## <a name="properties"></a><span data-ttu-id="900d7-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="900d7-106">Properties</span></span>

| <span data-ttu-id="900d7-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="900d7-107">Property</span></span> | <span data-ttu-id="900d7-108">Тип</span><span class="sxs-lookup"><span data-stu-id="900d7-108">Type</span></span> | <span data-ttu-id="900d7-109">Описание</span><span class="sxs-lookup"><span data-stu-id="900d7-109">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="900d7-110">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="900d7-110">sourceId</span></span> | <span data-ttu-id="900d7-111">Строка</span><span class="sxs-lookup"><span data-stu-id="900d7-111">String</span></span> | <span data-ttu-id="900d7-112">Преобразованный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="900d7-112">The identifier that was converted.</span></span> <span data-ttu-id="900d7-113">Это значение является исходным непреобразуемым идентификатором.</span><span class="sxs-lookup"><span data-stu-id="900d7-113">This value is the original, un-converted identifier.</span></span> |
| <span data-ttu-id="900d7-114">targetId</span><span class="sxs-lookup"><span data-stu-id="900d7-114">targetId</span></span> | <span data-ttu-id="900d7-115">Строка</span><span class="sxs-lookup"><span data-stu-id="900d7-115">String</span></span> | <span data-ttu-id="900d7-116">Преобразованный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="900d7-116">The converted identifier.</span></span> <span data-ttu-id="900d7-117">Это значение отсутствует, если произошел сбой преобразования.</span><span class="sxs-lookup"><span data-stu-id="900d7-117">This value is not present if the conversion failed.</span></span> |
| <span data-ttu-id="900d7-118">еррордетаилс</span><span class="sxs-lookup"><span data-stu-id="900d7-118">errorDetails</span></span> | [<span data-ttu-id="900d7-119">женерицеррор</span><span class="sxs-lookup"><span data-stu-id="900d7-119">genericError</span></span>](genericerror.md) | <span data-ttu-id="900d7-120">Объект Error, указывающий причину сбоя преобразования.</span><span class="sxs-lookup"><span data-stu-id="900d7-120">An error object indicating the reason for the conversion failure.</span></span> <span data-ttu-id="900d7-121">Это значение отсутствует, если преобразование выполнено успешно.</span><span class="sxs-lookup"><span data-stu-id="900d7-121">This value is not present if the conversion succeeded.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="900d7-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="900d7-122">JSON representation</span></span>

<span data-ttu-id="900d7-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="900d7-123">Here is a JSON representation of the resource.</span></span>

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

