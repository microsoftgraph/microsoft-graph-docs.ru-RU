---
title: Тип ресурса Конвертидресулт
description: Результат преобразования формата идентификатора, выполняемого функцией Транслатиксчанжеидс.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 040b13ab83eacffb33e8903f7d11823adb6e1bf1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973209"
---
# <a name="convertidresult-resource-type"></a><span data-ttu-id="d98ca-103">Тип ресурса Конвертидресулт</span><span class="sxs-lookup"><span data-stu-id="d98ca-103">convertIdResult resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d98ca-104">Результат преобразования формата идентификатора, выполняемого функцией [транслатиксчанжеидс](../api/user-translateexchangeids.md) .</span><span class="sxs-lookup"><span data-stu-id="d98ca-104">The result of an ID format conversion performed by the [translateExchangeIds](../api/user-translateexchangeids.md) function.</span></span>

## <a name="properties"></a><span data-ttu-id="d98ca-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="d98ca-105">Properties</span></span>

| <span data-ttu-id="d98ca-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="d98ca-106">Property</span></span> | <span data-ttu-id="d98ca-107">Тип</span><span class="sxs-lookup"><span data-stu-id="d98ca-107">Type</span></span> | <span data-ttu-id="d98ca-108">Описание</span><span class="sxs-lookup"><span data-stu-id="d98ca-108">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="d98ca-109">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="d98ca-109">sourceId</span></span> | <span data-ttu-id="d98ca-110">String</span><span class="sxs-lookup"><span data-stu-id="d98ca-110">String</span></span> | <span data-ttu-id="d98ca-111">Преобразованный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="d98ca-111">The identifier that was converted.</span></span> <span data-ttu-id="d98ca-112">Это значение является исходным непреобразуемым идентификатором.</span><span class="sxs-lookup"><span data-stu-id="d98ca-112">This value is the original, un-converted identifier.</span></span> |
| <span data-ttu-id="d98ca-113">targetId</span><span class="sxs-lookup"><span data-stu-id="d98ca-113">targetId</span></span> | <span data-ttu-id="d98ca-114">String</span><span class="sxs-lookup"><span data-stu-id="d98ca-114">String</span></span> | <span data-ttu-id="d98ca-115">Преобразованный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="d98ca-115">The converted identifier.</span></span> <span data-ttu-id="d98ca-116">Это значение отсутствует, если произошел сбой преобразования.</span><span class="sxs-lookup"><span data-stu-id="d98ca-116">This value is not present if the conversion failed.</span></span> |
| <span data-ttu-id="d98ca-117">Еррордетаилс</span><span class="sxs-lookup"><span data-stu-id="d98ca-117">errorDetails</span></span> | [<span data-ttu-id="d98ca-118">Женерицеррор</span><span class="sxs-lookup"><span data-stu-id="d98ca-118">genericError</span></span>](genericerror.md) | <span data-ttu-id="d98ca-119">Объект Error, указывающий причину сбоя преобразования.</span><span class="sxs-lookup"><span data-stu-id="d98ca-119">An error object indicating the reason for the conversion failure.</span></span> <span data-ttu-id="d98ca-120">Это значение отсутствует, если преобразование выполнено успешно.</span><span class="sxs-lookup"><span data-stu-id="d98ca-120">This value is not present if the conversion succeeded.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d98ca-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d98ca-121">JSON representation</span></span>

<span data-ttu-id="d98ca-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d98ca-122">Here is a JSON representation of the resource.</span></span>

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
