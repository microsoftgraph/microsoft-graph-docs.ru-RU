---
title: Тип ресурса convertIdResult
description: Результат преобразования формата код выполняется с помощью функции translateExchangeIds.
localization_priority: Normal
ms.openlocfilehash: 7e1878de3d3b7ddee36d799c928d6a130b578200
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821457"
---
# <a name="convertidresult-resource-type"></a><span data-ttu-id="e2098-103">Тип ресурса convertIdResult</span><span class="sxs-lookup"><span data-stu-id="e2098-103">convertIdResult resource type</span></span>

> <span data-ttu-id="e2098-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e2098-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e2098-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2098-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e2098-106">Результат преобразования формата код выполняется с помощью функции [translateExchangeIds](../api/user-translateexchangeids.md) .</span><span class="sxs-lookup"><span data-stu-id="e2098-106">The result of an ID format conversion performed by the [translateExchangeIds](../api/user-translateexchangeids.md) function.</span></span>

## <a name="properties"></a><span data-ttu-id="e2098-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e2098-107">Properties</span></span>

| <span data-ttu-id="e2098-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e2098-108">Property</span></span> | <span data-ttu-id="e2098-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e2098-109">Type</span></span> | <span data-ttu-id="e2098-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e2098-110">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="e2098-111">sourceId</span><span class="sxs-lookup"><span data-stu-id="e2098-111">sourceId</span></span> | <span data-ttu-id="e2098-112">Строка</span><span class="sxs-lookup"><span data-stu-id="e2098-112">String</span></span> | <span data-ttu-id="e2098-113">Идентификатор, который был преобразован.</span><span class="sxs-lookup"><span data-stu-id="e2098-113">The identifier that was converted.</span></span> <span data-ttu-id="e2098-114">Это значение является идентификатором исходного, без преобразованные.</span><span class="sxs-lookup"><span data-stu-id="e2098-114">This value is the original, un-converted identifier.</span></span> |
| <span data-ttu-id="e2098-115">targetId</span><span class="sxs-lookup"><span data-stu-id="e2098-115">targetId</span></span> | <span data-ttu-id="e2098-116">Строка</span><span class="sxs-lookup"><span data-stu-id="e2098-116">String</span></span> | <span data-ttu-id="e2098-117">Преобразованные идентификатор.</span><span class="sxs-lookup"><span data-stu-id="e2098-117">The converted identifier.</span></span> <span data-ttu-id="e2098-118">Это значение не задано, если не удалось выполнить преобразование.</span><span class="sxs-lookup"><span data-stu-id="e2098-118">This value is not present if the conversion failed.</span></span> |
| <span data-ttu-id="e2098-119">errorDetails</span><span class="sxs-lookup"><span data-stu-id="e2098-119">errorDetails</span></span> | [<span data-ttu-id="e2098-120">Общая ошибка</span><span class="sxs-lookup"><span data-stu-id="e2098-120">genericError</span></span>](genericerror.md) | <span data-ttu-id="e2098-121">Объект error, которое указывает причину сбоя преобразования.</span><span class="sxs-lookup"><span data-stu-id="e2098-121">An error object indicating the reason for the conversion failure.</span></span> <span data-ttu-id="e2098-122">Это значение не задано, если преобразование выполнено успешно.</span><span class="sxs-lookup"><span data-stu-id="e2098-122">This value is not present if the conversion succeeded.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e2098-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e2098-123">JSON representation</span></span>

<span data-ttu-id="e2098-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e2098-124">Here is a JSON representation of the resource.</span></span>

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
