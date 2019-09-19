---
title: Тип ресурса Конвертидресулт
description: Результат преобразования формата идентификатора, выполняемого функцией Транслатиксчанжеидс.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: svpsiva
ms.openlocfilehash: 405d663e4f1f7fb040e79cdd10669bc824e3edef
ms.sourcegitcommit: 471f07c30867658688bd932e06822be1bbcea360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2019
ms.locfileid: "37036447"
---
# <a name="convertidresult-resource-type"></a><span data-ttu-id="6131f-103">Тип ресурса Конвертидресулт</span><span class="sxs-lookup"><span data-stu-id="6131f-103">convertIdResult resource type</span></span>

<span data-ttu-id="6131f-104">Результат преобразования формата идентификатора, выполняемого функцией [транслатиксчанжеидс](../api/user-translateexchangeids.md) .</span><span class="sxs-lookup"><span data-stu-id="6131f-104">The result of an ID format conversion performed by the [translateExchangeIds](../api/user-translateexchangeids.md) function.</span></span>

## <a name="properties"></a><span data-ttu-id="6131f-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="6131f-105">Properties</span></span>

| <span data-ttu-id="6131f-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="6131f-106">Property</span></span> | <span data-ttu-id="6131f-107">Тип</span><span class="sxs-lookup"><span data-stu-id="6131f-107">Type</span></span> | <span data-ttu-id="6131f-108">Описание</span><span class="sxs-lookup"><span data-stu-id="6131f-108">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="6131f-109">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="6131f-109">sourceId</span></span> | <span data-ttu-id="6131f-110">String.</span><span class="sxs-lookup"><span data-stu-id="6131f-110">String</span></span> | <span data-ttu-id="6131f-111">Преобразованный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="6131f-111">The identifier that was converted.</span></span> <span data-ttu-id="6131f-112">Это значение является исходным непреобразуемым идентификатором.</span><span class="sxs-lookup"><span data-stu-id="6131f-112">This value is the original, un-converted identifier.</span></span> |
| <span data-ttu-id="6131f-113">targetId</span><span class="sxs-lookup"><span data-stu-id="6131f-113">targetId</span></span> | <span data-ttu-id="6131f-114">String.</span><span class="sxs-lookup"><span data-stu-id="6131f-114">String</span></span> | <span data-ttu-id="6131f-115">Преобразованный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="6131f-115">The converted identifier.</span></span> <span data-ttu-id="6131f-116">Это значение отсутствует, если произошел сбой преобразования.</span><span class="sxs-lookup"><span data-stu-id="6131f-116">This value is not present if the conversion failed.</span></span> |
| <span data-ttu-id="6131f-117">еррордетаилс</span><span class="sxs-lookup"><span data-stu-id="6131f-117">errorDetails</span></span> | [<span data-ttu-id="6131f-118">женерицеррор</span><span class="sxs-lookup"><span data-stu-id="6131f-118">genericError</span></span>](genericerror.md) | <span data-ttu-id="6131f-119">Объект Error, указывающий причину сбоя преобразования.</span><span class="sxs-lookup"><span data-stu-id="6131f-119">An error object indicating the reason for the conversion failure.</span></span> <span data-ttu-id="6131f-120">Это значение отсутствует, если преобразование выполнено успешно.</span><span class="sxs-lookup"><span data-stu-id="6131f-120">This value is not present if the conversion succeeded.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6131f-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6131f-121">JSON representation</span></span>

<span data-ttu-id="6131f-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6131f-122">Here is a JSON representation of the resource.</span></span>

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
