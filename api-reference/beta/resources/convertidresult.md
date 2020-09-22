---
title: Тип ресурса Конвертидресулт
description: Результат преобразования формата идентификатора, выполняемого функцией Транслатиксчанжеидс.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: svpsiva
ms.openlocfilehash: 3579385fa4c42da3d14914d134dd817c4de08ba5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016756"
---
# <a name="convertidresult-resource-type"></a><span data-ttu-id="5a2ab-103">Тип ресурса Конвертидресулт</span><span class="sxs-lookup"><span data-stu-id="5a2ab-103">convertIdResult resource type</span></span>

<span data-ttu-id="5a2ab-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a2ab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a2ab-105">Результат преобразования формата идентификатора, выполняемого функцией [транслатиксчанжеидс](../api/user-translateexchangeids.md) .</span><span class="sxs-lookup"><span data-stu-id="5a2ab-105">The result of an ID format conversion performed by the [translateExchangeIds](../api/user-translateexchangeids.md) function.</span></span>

## <a name="properties"></a><span data-ttu-id="5a2ab-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="5a2ab-106">Properties</span></span>

| <span data-ttu-id="5a2ab-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="5a2ab-107">Property</span></span> | <span data-ttu-id="5a2ab-108">Тип</span><span class="sxs-lookup"><span data-stu-id="5a2ab-108">Type</span></span> | <span data-ttu-id="5a2ab-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5a2ab-109">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="5a2ab-110">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="5a2ab-110">sourceId</span></span> | <span data-ttu-id="5a2ab-111">String</span><span class="sxs-lookup"><span data-stu-id="5a2ab-111">String</span></span> | <span data-ttu-id="5a2ab-112">Преобразованный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="5a2ab-112">The identifier that was converted.</span></span> <span data-ttu-id="5a2ab-113">Это значение является исходным непреобразуемым идентификатором.</span><span class="sxs-lookup"><span data-stu-id="5a2ab-113">This value is the original, un-converted identifier.</span></span> |
| <span data-ttu-id="5a2ab-114">targetId</span><span class="sxs-lookup"><span data-stu-id="5a2ab-114">targetId</span></span> | <span data-ttu-id="5a2ab-115">String</span><span class="sxs-lookup"><span data-stu-id="5a2ab-115">String</span></span> | <span data-ttu-id="5a2ab-116">Преобразованный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="5a2ab-116">The converted identifier.</span></span> <span data-ttu-id="5a2ab-117">Это значение отсутствует, если произошел сбой преобразования.</span><span class="sxs-lookup"><span data-stu-id="5a2ab-117">This value is not present if the conversion failed.</span></span> |
| <span data-ttu-id="5a2ab-118">еррордетаилс</span><span class="sxs-lookup"><span data-stu-id="5a2ab-118">errorDetails</span></span> | [<span data-ttu-id="5a2ab-119">женерицеррор</span><span class="sxs-lookup"><span data-stu-id="5a2ab-119">genericError</span></span>](genericerror.md) | <span data-ttu-id="5a2ab-120">Объект Error, указывающий причину сбоя преобразования.</span><span class="sxs-lookup"><span data-stu-id="5a2ab-120">An error object indicating the reason for the conversion failure.</span></span> <span data-ttu-id="5a2ab-121">Это значение отсутствует, если преобразование выполнено успешно.</span><span class="sxs-lookup"><span data-stu-id="5a2ab-121">This value is not present if the conversion succeeded.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5a2ab-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5a2ab-122">JSON representation</span></span>

<span data-ttu-id="5a2ab-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5a2ab-123">Here is a JSON representation of the resource.</span></span>

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


