---
title: Тип ресурса Статусдетаилс
description: Описывает состояние события подготовки и связанных с ним ошибок.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 88880fbe88c0bd702eefeac5bed9668aac12a356
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35455184"
---
# <a name="statusdetails-resource-type"></a><span data-ttu-id="feecd-103">Тип ресурса Статусдетаилс</span><span class="sxs-lookup"><span data-stu-id="feecd-103">statusDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="feecd-104">Описывает состояние события подготовки и связанных с ним ошибок.</span><span class="sxs-lookup"><span data-stu-id="feecd-104">Describes the status of the provisioning event and the associated errors.</span></span> <span data-ttu-id="feecd-105">Он наследуется от [статусбасе](/graph/api/resources/statusbase?view=graph-rest-beta) и используется только в том случае, если для параметра Status задано значение "failure".</span><span class="sxs-lookup"><span data-stu-id="feecd-105">It is inherited from [statusBase](/graph/api/resources/statusbase?view=graph-rest-beta) and only used when status is set to 'failure'.</span></span>  

## <a name="properties"></a><span data-ttu-id="feecd-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="feecd-106">Properties</span></span>

| <span data-ttu-id="feecd-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="feecd-107">Property</span></span>     | <span data-ttu-id="feecd-108">Тип</span><span class="sxs-lookup"><span data-stu-id="feecd-108">Type</span></span>        | <span data-ttu-id="feecd-109">Описание</span><span class="sxs-lookup"><span data-stu-id="feecd-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="feecd-110">status</span><span class="sxs-lookup"><span data-stu-id="feecd-110">status</span></span>|<span data-ttu-id="feecd-111">String</span><span class="sxs-lookup"><span data-stu-id="feecd-111">String</span></span>|<span data-ttu-id="feecd-112">Возможные значения: `success`, `failure`, `skipped`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="feecd-112">Possible values are: `success`, `failure`, `skipped`, `unknownFutureValue`.</span></span> <span data-ttu-id="feecd-113">Наследуется от Статусбасе.</span><span class="sxs-lookup"><span data-stu-id="feecd-113">Inherited from statusBase.</span></span>|
|<span data-ttu-id="feecd-114">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="feecd-114">additionalDetails</span></span>|<span data-ttu-id="feecd-115">String</span><span class="sxs-lookup"><span data-stu-id="feecd-115">String</span></span>|<span data-ttu-id="feecd-116">Дополнительные сведения в случае ошибки.</span><span class="sxs-lookup"><span data-stu-id="feecd-116">Additional details in case of error.</span></span>|
|<span data-ttu-id="feecd-117">errorCategory</span><span class="sxs-lookup"><span data-stu-id="feecd-117">errorCategory</span></span>|<span data-ttu-id="feecd-118">String</span><span class="sxs-lookup"><span data-stu-id="feecd-118">String</span></span>|<span data-ttu-id="feecd-119">Классификация кода ошибки.</span><span class="sxs-lookup"><span data-stu-id="feecd-119">Categorizes the error code.</span></span>|
|<span data-ttu-id="feecd-120">errorCode</span><span class="sxs-lookup"><span data-stu-id="feecd-120">errorCode</span></span>|<span data-ttu-id="feecd-121">String</span><span class="sxs-lookup"><span data-stu-id="feecd-121">String</span></span>|<span data-ttu-id="feecd-122">Уникальный код ошибки (при возникновении ошибки).</span><span class="sxs-lookup"><span data-stu-id="feecd-122">Unique error code if any occurred.</span></span>|
|<span data-ttu-id="feecd-123">причиной</span><span class="sxs-lookup"><span data-stu-id="feecd-123">reason</span></span>|<span data-ttu-id="feecd-124">String</span><span class="sxs-lookup"><span data-stu-id="feecd-124">String</span></span>|<span data-ttu-id="feecd-125">Сводка состояния и описание причин возникновения состояния.</span><span class="sxs-lookup"><span data-stu-id="feecd-125">Summarizes the status and describes why the status happened.</span></span>|
|<span data-ttu-id="feecd-126">Рекоммендедактион</span><span class="sxs-lookup"><span data-stu-id="feecd-126">recommendedAction</span></span>|<span data-ttu-id="feecd-127">String</span><span class="sxs-lookup"><span data-stu-id="feecd-127">String</span></span>|<span data-ttu-id="feecd-128">Предоставляет решение для соответствующей ошибки.</span><span class="sxs-lookup"><span data-stu-id="feecd-128">Provides the resolution for the corresponding error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="feecd-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="feecd-129">JSON representation</span></span>

<span data-ttu-id="feecd-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="feecd-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.statusDetails",
  "baseType": "microsoft.graph.statusBase"
}-->

```json
{
  "status": "failure",
  "additionalDetails": "String",
  "errorCategory": "String",
  "errorCode": "String",
  "reason": "String",
  "recommendedAction": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "statusDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
