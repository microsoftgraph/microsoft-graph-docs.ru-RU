---
title: Тип ресурса Статусдетаилс
description: Описывает состояние события подготовки и связанных с ним ошибок.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8f931d14a026a6809e70b4cc83e5b8e55e72e63a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43411860"
---
# <a name="statusdetails-resource-type"></a><span data-ttu-id="dd204-103">Тип ресурса Статусдетаилс</span><span class="sxs-lookup"><span data-stu-id="dd204-103">statusDetails resource type</span></span>

<span data-ttu-id="dd204-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd204-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd204-105">Описывает состояние события подготовки и связанных с ним ошибок.</span><span class="sxs-lookup"><span data-stu-id="dd204-105">Describes the status of the provisioning event and the associated errors.</span></span> <span data-ttu-id="dd204-106">Он наследуется от [статусбасе](/graph/api/resources/statusbase?view=graph-rest-beta) и используется только в том случае, если для параметра Status задано значение "failure".</span><span class="sxs-lookup"><span data-stu-id="dd204-106">It is inherited from [statusBase](/graph/api/resources/statusbase?view=graph-rest-beta) and only used when status is set to 'failure'.</span></span>  

## <a name="properties"></a><span data-ttu-id="dd204-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="dd204-107">Properties</span></span>

| <span data-ttu-id="dd204-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="dd204-108">Property</span></span>     | <span data-ttu-id="dd204-109">Тип</span><span class="sxs-lookup"><span data-stu-id="dd204-109">Type</span></span>        | <span data-ttu-id="dd204-110">Описание</span><span class="sxs-lookup"><span data-stu-id="dd204-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="dd204-111">status</span><span class="sxs-lookup"><span data-stu-id="dd204-111">status</span></span>|<span data-ttu-id="dd204-112">String</span><span class="sxs-lookup"><span data-stu-id="dd204-112">String</span></span>|<span data-ttu-id="dd204-113">Возможные значения: `success`, `failure`, `skipped`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="dd204-113">Possible values are: `success`, `failure`, `skipped`, `unknownFutureValue`.</span></span> <span data-ttu-id="dd204-114">Наследуется от Статусбасе.</span><span class="sxs-lookup"><span data-stu-id="dd204-114">Inherited from statusBase.</span></span>|
|<span data-ttu-id="dd204-115">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="dd204-115">additionalDetails</span></span>|<span data-ttu-id="dd204-116">String</span><span class="sxs-lookup"><span data-stu-id="dd204-116">String</span></span>|<span data-ttu-id="dd204-117">Дополнительные сведения в случае ошибки.</span><span class="sxs-lookup"><span data-stu-id="dd204-117">Additional details in case of error.</span></span>|
|<span data-ttu-id="dd204-118">errorCategory</span><span class="sxs-lookup"><span data-stu-id="dd204-118">errorCategory</span></span>|<span data-ttu-id="dd204-119">String</span><span class="sxs-lookup"><span data-stu-id="dd204-119">String</span></span>|<span data-ttu-id="dd204-120">Классификация кода ошибки.</span><span class="sxs-lookup"><span data-stu-id="dd204-120">Categorizes the error code.</span></span>|
|<span data-ttu-id="dd204-121">errorCode</span><span class="sxs-lookup"><span data-stu-id="dd204-121">errorCode</span></span>|<span data-ttu-id="dd204-122">String</span><span class="sxs-lookup"><span data-stu-id="dd204-122">String</span></span>|<span data-ttu-id="dd204-123">Уникальный код ошибки (при возникновении ошибки).</span><span class="sxs-lookup"><span data-stu-id="dd204-123">Unique error code if any occurred.</span></span>|
|<span data-ttu-id="dd204-124">reason</span><span class="sxs-lookup"><span data-stu-id="dd204-124">reason</span></span>|<span data-ttu-id="dd204-125">String</span><span class="sxs-lookup"><span data-stu-id="dd204-125">String</span></span>|<span data-ttu-id="dd204-126">Сводка состояния и описание причин возникновения состояния.</span><span class="sxs-lookup"><span data-stu-id="dd204-126">Summarizes the status and describes why the status happened.</span></span>|
|<span data-ttu-id="dd204-127">рекоммендедактион</span><span class="sxs-lookup"><span data-stu-id="dd204-127">recommendedAction</span></span>|<span data-ttu-id="dd204-128">String</span><span class="sxs-lookup"><span data-stu-id="dd204-128">String</span></span>|<span data-ttu-id="dd204-129">Предоставляет решение для соответствующей ошибки.</span><span class="sxs-lookup"><span data-stu-id="dd204-129">Provides the resolution for the corresponding error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dd204-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dd204-130">JSON representation</span></span>

<span data-ttu-id="dd204-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dd204-131">The following is a JSON representation of the resource.</span></span>

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
