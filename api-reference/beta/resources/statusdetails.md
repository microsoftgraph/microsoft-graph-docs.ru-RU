---
title: Тип ресурса Статусдетаилс
description: Описывает состояние события подготовки и связанных с ним ошибок.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 16f014ebc3a188644784434a69e13917f05beaae
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029024"
---
# <a name="statusdetails-resource-type"></a><span data-ttu-id="36d9a-103">Тип ресурса Статусдетаилс</span><span class="sxs-lookup"><span data-stu-id="36d9a-103">statusDetails resource type</span></span>

<span data-ttu-id="36d9a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36d9a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36d9a-105">Описывает состояние события подготовки и связанных с ним ошибок.</span><span class="sxs-lookup"><span data-stu-id="36d9a-105">Describes the status of the provisioning event and the associated errors.</span></span> <span data-ttu-id="36d9a-106">Он наследуется от [статусбасе](/graph/api/resources/statusbase?view=graph-rest-beta) и используется только в том случае, если для параметра Status задано значение "failure".</span><span class="sxs-lookup"><span data-stu-id="36d9a-106">It is inherited from [statusBase](/graph/api/resources/statusbase?view=graph-rest-beta) and only used when status is set to 'failure'.</span></span>  

## <a name="properties"></a><span data-ttu-id="36d9a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="36d9a-107">Properties</span></span>

| <span data-ttu-id="36d9a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="36d9a-108">Property</span></span>     | <span data-ttu-id="36d9a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="36d9a-109">Type</span></span>        | <span data-ttu-id="36d9a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="36d9a-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="36d9a-111">status</span><span class="sxs-lookup"><span data-stu-id="36d9a-111">status</span></span>|<span data-ttu-id="36d9a-112">String</span><span class="sxs-lookup"><span data-stu-id="36d9a-112">String</span></span>|<span data-ttu-id="36d9a-113">Возможные значения: `success`, `failure`, `skipped`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="36d9a-113">Possible values are: `success`, `failure`, `skipped`, `unknownFutureValue`.</span></span> <span data-ttu-id="36d9a-114">Наследуется от Статусбасе.</span><span class="sxs-lookup"><span data-stu-id="36d9a-114">Inherited from statusBase.</span></span>|
|<span data-ttu-id="36d9a-115">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="36d9a-115">additionalDetails</span></span>|<span data-ttu-id="36d9a-116">String</span><span class="sxs-lookup"><span data-stu-id="36d9a-116">String</span></span>|<span data-ttu-id="36d9a-117">Дополнительные сведения в случае ошибки.</span><span class="sxs-lookup"><span data-stu-id="36d9a-117">Additional details in case of error.</span></span>|
|<span data-ttu-id="36d9a-118">errorCategory</span><span class="sxs-lookup"><span data-stu-id="36d9a-118">errorCategory</span></span>|<span data-ttu-id="36d9a-119">String</span><span class="sxs-lookup"><span data-stu-id="36d9a-119">String</span></span>|<span data-ttu-id="36d9a-120">Классификация кода ошибки.</span><span class="sxs-lookup"><span data-stu-id="36d9a-120">Categorizes the error code.</span></span>|
|<span data-ttu-id="36d9a-121">errorCode</span><span class="sxs-lookup"><span data-stu-id="36d9a-121">errorCode</span></span>|<span data-ttu-id="36d9a-122">String</span><span class="sxs-lookup"><span data-stu-id="36d9a-122">String</span></span>|<span data-ttu-id="36d9a-123">Уникальный код ошибки (при возникновении ошибки).</span><span class="sxs-lookup"><span data-stu-id="36d9a-123">Unique error code if any occurred.</span></span>|
|<span data-ttu-id="36d9a-124">reason</span><span class="sxs-lookup"><span data-stu-id="36d9a-124">reason</span></span>|<span data-ttu-id="36d9a-125">String</span><span class="sxs-lookup"><span data-stu-id="36d9a-125">String</span></span>|<span data-ttu-id="36d9a-126">Сводка состояния и описание причин возникновения состояния.</span><span class="sxs-lookup"><span data-stu-id="36d9a-126">Summarizes the status and describes why the status happened.</span></span>|
|<span data-ttu-id="36d9a-127">рекоммендедактион</span><span class="sxs-lookup"><span data-stu-id="36d9a-127">recommendedAction</span></span>|<span data-ttu-id="36d9a-128">String</span><span class="sxs-lookup"><span data-stu-id="36d9a-128">String</span></span>|<span data-ttu-id="36d9a-129">Предоставляет решение для соответствующей ошибки.</span><span class="sxs-lookup"><span data-stu-id="36d9a-129">Provides the resolution for the corresponding error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="36d9a-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="36d9a-130">JSON representation</span></span>

<span data-ttu-id="36d9a-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="36d9a-131">The following is a JSON representation of the resource.</span></span>

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


