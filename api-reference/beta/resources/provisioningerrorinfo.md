---
title: тип ресурса provisioningErrorInfo
description: Описывает состояние события подготовка и связанные с ним ошибки.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: dddddfa793cf9aac7436fc85e0ce911df7b4ec3e
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52546975"
---
# <a name="provisioningerrorinfo-resource-type"></a><span data-ttu-id="8ff8e-103">тип ресурса provisioningErrorInfo</span><span class="sxs-lookup"><span data-stu-id="8ff8e-103">provisioningErrorInfo resource type</span></span>

<span data-ttu-id="8ff8e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ff8e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ff8e-105">Описывает состояние события подготовка и связанные с ним ошибки.</span><span class="sxs-lookup"><span data-stu-id="8ff8e-105">Describes the status of the provisioning event and the associated errors.</span></span> 

## <a name="properties"></a><span data-ttu-id="8ff8e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="8ff8e-106">Properties</span></span>

| <span data-ttu-id="8ff8e-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="8ff8e-107">Property</span></span>     | <span data-ttu-id="8ff8e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="8ff8e-108">Type</span></span>        | <span data-ttu-id="8ff8e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8ff8e-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8ff8e-110">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="8ff8e-110">additionalDetails</span></span>|<span data-ttu-id="8ff8e-111">String</span><span class="sxs-lookup"><span data-stu-id="8ff8e-111">String</span></span>|<span data-ttu-id="8ff8e-112">Дополнительные сведения в случае ошибки.</span><span class="sxs-lookup"><span data-stu-id="8ff8e-112">Additional details in case of error.</span></span>|
|<span data-ttu-id="8ff8e-113">errorCategory</span><span class="sxs-lookup"><span data-stu-id="8ff8e-113">errorCategory</span></span>|<span data-ttu-id="8ff8e-114">String</span><span class="sxs-lookup"><span data-stu-id="8ff8e-114">String</span></span>|<span data-ttu-id="8ff8e-115">Классифицировать код ошибки.</span><span class="sxs-lookup"><span data-stu-id="8ff8e-115">Categorizes the error code.</span></span> <span data-ttu-id="8ff8e-116">Возможные значения `failure` : `nonServiceFailure` , `success` , `unknownFutureValue`</span><span class="sxs-lookup"><span data-stu-id="8ff8e-116">Possible values are `failure`, `nonServiceFailure`, `success`, `unknownFutureValue`</span></span>|
|<span data-ttu-id="8ff8e-117">errorCode</span><span class="sxs-lookup"><span data-stu-id="8ff8e-117">errorCode</span></span>|<span data-ttu-id="8ff8e-118">String</span><span class="sxs-lookup"><span data-stu-id="8ff8e-118">String</span></span>|<span data-ttu-id="8ff8e-119">Уникальный код ошибки, если таковое произошло.</span><span class="sxs-lookup"><span data-stu-id="8ff8e-119">Unique error code if any occurred.</span></span> [<span data-ttu-id="8ff8e-120">Подробнее</span><span class="sxs-lookup"><span data-stu-id="8ff8e-120">Learn more</span></span>](/azure/active-directory/reports-monitoring/concept-provisioning-logs#error-codes)|
|<span data-ttu-id="8ff8e-121">reason</span><span class="sxs-lookup"><span data-stu-id="8ff8e-121">reason</span></span>|<span data-ttu-id="8ff8e-122">String</span><span class="sxs-lookup"><span data-stu-id="8ff8e-122">String</span></span>|<span data-ttu-id="8ff8e-123">Суммирует состояние и описывает причины, по которым произошел этот статус.</span><span class="sxs-lookup"><span data-stu-id="8ff8e-123">Summarizes the status and describes why the status happened.</span></span>|
|<span data-ttu-id="8ff8e-124">recommendedAction</span><span class="sxs-lookup"><span data-stu-id="8ff8e-124">recommendedAction</span></span>|<span data-ttu-id="8ff8e-125">String</span><span class="sxs-lookup"><span data-stu-id="8ff8e-125">String</span></span>|<span data-ttu-id="8ff8e-126">Обеспечивает разрешение соответствующей ошибки.</span><span class="sxs-lookup"><span data-stu-id="8ff8e-126">Provides the resolution for the corresponding error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8ff8e-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8ff8e-127">JSON representation</span></span>

<span data-ttu-id="8ff8e-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8ff8e-128">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningErrorInfo",
  "baseType": null
}-->

```json
{
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
  "description": "provisioningErrorInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


