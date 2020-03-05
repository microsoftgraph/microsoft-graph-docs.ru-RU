---
title: Тип ресурса Конвертидресулт
description: Результат преобразования формата идентификатора, выполняемого функцией Транслатиксчанжеидс.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: svpsiva
ms.openlocfilehash: 6c4cd63316747b51474dd5c61912c0f155c047c8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507389"
---
# <a name="convertidresult-resource-type"></a><span data-ttu-id="69d88-103">Тип ресурса Конвертидресулт</span><span class="sxs-lookup"><span data-stu-id="69d88-103">convertIdResult resource type</span></span>

<span data-ttu-id="69d88-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="69d88-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69d88-105">Результат преобразования формата идентификатора, выполняемого функцией [транслатиксчанжеидс](../api/user-translateexchangeids.md) .</span><span class="sxs-lookup"><span data-stu-id="69d88-105">The result of an ID format conversion performed by the [translateExchangeIds](../api/user-translateexchangeids.md) function.</span></span>

## <a name="properties"></a><span data-ttu-id="69d88-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="69d88-106">Properties</span></span>

| <span data-ttu-id="69d88-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="69d88-107">Property</span></span> | <span data-ttu-id="69d88-108">Тип</span><span class="sxs-lookup"><span data-stu-id="69d88-108">Type</span></span> | <span data-ttu-id="69d88-109">Описание</span><span class="sxs-lookup"><span data-stu-id="69d88-109">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="69d88-110">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="69d88-110">sourceId</span></span> | <span data-ttu-id="69d88-111">String</span><span class="sxs-lookup"><span data-stu-id="69d88-111">String</span></span> | <span data-ttu-id="69d88-112">Преобразованный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="69d88-112">The identifier that was converted.</span></span> <span data-ttu-id="69d88-113">Это значение является исходным непреобразуемым идентификатором.</span><span class="sxs-lookup"><span data-stu-id="69d88-113">This value is the original, un-converted identifier.</span></span> |
| <span data-ttu-id="69d88-114">targetId</span><span class="sxs-lookup"><span data-stu-id="69d88-114">targetId</span></span> | <span data-ttu-id="69d88-115">String</span><span class="sxs-lookup"><span data-stu-id="69d88-115">String</span></span> | <span data-ttu-id="69d88-116">Преобразованный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="69d88-116">The converted identifier.</span></span> <span data-ttu-id="69d88-117">Это значение отсутствует, если произошел сбой преобразования.</span><span class="sxs-lookup"><span data-stu-id="69d88-117">This value is not present if the conversion failed.</span></span> |
| <span data-ttu-id="69d88-118">еррордетаилс</span><span class="sxs-lookup"><span data-stu-id="69d88-118">errorDetails</span></span> | [<span data-ttu-id="69d88-119">женерицеррор</span><span class="sxs-lookup"><span data-stu-id="69d88-119">genericError</span></span>](genericerror.md) | <span data-ttu-id="69d88-120">Объект Error, указывающий причину сбоя преобразования.</span><span class="sxs-lookup"><span data-stu-id="69d88-120">An error object indicating the reason for the conversion failure.</span></span> <span data-ttu-id="69d88-121">Это значение отсутствует, если преобразование выполнено успешно.</span><span class="sxs-lookup"><span data-stu-id="69d88-121">This value is not present if the conversion succeeded.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="69d88-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="69d88-122">JSON representation</span></span>

<span data-ttu-id="69d88-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="69d88-123">Here is a JSON representation of the resource.</span></span>

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
