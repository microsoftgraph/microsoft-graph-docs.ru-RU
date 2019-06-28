---
title: Тип ресурса Статусдетаилс
description: Описывает состояние события подготовки и связанных с ним ошибок.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d3c22e67af690a28bb974a0334af7891f0c25cfb
ms.sourcegitcommit: e0de4e41773e361752870411d1b1a74270738127
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/28/2019
ms.locfileid: "35349445"
---
# <a name="statusdetails-resource-type"></a><span data-ttu-id="6dd0c-103">Тип ресурса Статусдетаилс</span><span class="sxs-lookup"><span data-stu-id="6dd0c-103">statusDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6dd0c-104">Описывает состояние события подготовки и связанных с ним ошибок.</span><span class="sxs-lookup"><span data-stu-id="6dd0c-104">Describes the status of the provisioning event and the associated errors.</span></span> <span data-ttu-id="6dd0c-105">Он наследуется от [статусбасе](/graph/api/resources/statusBase?view=graph-rest-beta) и используется только в том случае, если для параметра Status задано значение "failure".</span><span class="sxs-lookup"><span data-stu-id="6dd0c-105">It is inherited from [statusBase](/graph/api/resources/statusBase?view=graph-rest-beta) and only used when status is set to 'failure'.</span></span>  

## <a name="properties"></a><span data-ttu-id="6dd0c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="6dd0c-106">Properties</span></span>

| <span data-ttu-id="6dd0c-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="6dd0c-107">Property</span></span>     | <span data-ttu-id="6dd0c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="6dd0c-108">Type</span></span>        | <span data-ttu-id="6dd0c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6dd0c-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6dd0c-110">status</span><span class="sxs-lookup"><span data-stu-id="6dd0c-110">status</span></span>|<span data-ttu-id="6dd0c-111">String</span><span class="sxs-lookup"><span data-stu-id="6dd0c-111">String</span></span>|<span data-ttu-id="6dd0c-112">Возможные значения: `success`, `failure`, `skipped`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="6dd0c-112">Possible values are: `success`, `failure`, `skipped`, `unknownFutureValue`.</span></span> <span data-ttu-id="6dd0c-113">Наследуется от Статусбасе.</span><span class="sxs-lookup"><span data-stu-id="6dd0c-113">Inherited from statusBase.</span></span>|
|<span data-ttu-id="6dd0c-114">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="6dd0c-114">additionalDetails</span></span>|<span data-ttu-id="6dd0c-115">String</span><span class="sxs-lookup"><span data-stu-id="6dd0c-115">String</span></span>|<span data-ttu-id="6dd0c-116">Дополнительные сведения в случае ошибки.</span><span class="sxs-lookup"><span data-stu-id="6dd0c-116">Additional details in case of error.</span></span>|
|<span data-ttu-id="6dd0c-117">errorCategory</span><span class="sxs-lookup"><span data-stu-id="6dd0c-117">errorCategory</span></span>|<span data-ttu-id="6dd0c-118">String</span><span class="sxs-lookup"><span data-stu-id="6dd0c-118">String</span></span>|<span data-ttu-id="6dd0c-119">Классификация кода ошибки.</span><span class="sxs-lookup"><span data-stu-id="6dd0c-119">Categorizes the error code.</span></span>|
|<span data-ttu-id="6dd0c-120">errorCode</span><span class="sxs-lookup"><span data-stu-id="6dd0c-120">errorCode</span></span>|<span data-ttu-id="6dd0c-121">String</span><span class="sxs-lookup"><span data-stu-id="6dd0c-121">String</span></span>|<span data-ttu-id="6dd0c-122">Уникальный код ошибки (при возникновении ошибки).</span><span class="sxs-lookup"><span data-stu-id="6dd0c-122">Unique error code if any occurred.</span></span>|
|<span data-ttu-id="6dd0c-123">причиной</span><span class="sxs-lookup"><span data-stu-id="6dd0c-123">reason</span></span>|<span data-ttu-id="6dd0c-124">String</span><span class="sxs-lookup"><span data-stu-id="6dd0c-124">String</span></span>|<span data-ttu-id="6dd0c-125">Сводка состояния и описание причин возникновения состояния.</span><span class="sxs-lookup"><span data-stu-id="6dd0c-125">Summarizes the status and describes why the status happened.</span></span>|
|<span data-ttu-id="6dd0c-126">Рекоммендедактион</span><span class="sxs-lookup"><span data-stu-id="6dd0c-126">recommendedAction</span></span>|<span data-ttu-id="6dd0c-127">String</span><span class="sxs-lookup"><span data-stu-id="6dd0c-127">String</span></span>|<span data-ttu-id="6dd0c-128">Предоставляет решение для соответствующей ошибки.</span><span class="sxs-lookup"><span data-stu-id="6dd0c-128">Provides the resolution for the corresponding error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6dd0c-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6dd0c-129">JSON representation</span></span>

<span data-ttu-id="6dd0c-130">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6dd0c-130">The following is a JSON representation of the resource.</span></span>

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
