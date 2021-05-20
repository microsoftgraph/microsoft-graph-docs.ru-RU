---
title: предоставление типа ресурса «ЭррорИнфо»
description: Описывает состояние события подготовки и связанные с ним ошибки.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: a682e176b40d58e2dc0a794b58b8561f8948d5a5
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547157"
---
# <a name="provisioningerrorinfo-resource-type"></a><span data-ttu-id="69fa6-103">предоставление типа ресурса «ЭррорИнфо»</span><span class="sxs-lookup"><span data-stu-id="69fa6-103">provisioningErrorInfo resource type</span></span>

<span data-ttu-id="69fa6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69fa6-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="69fa6-105">Описывает состояние события подготовки и связанные с ним ошибки.</span><span class="sxs-lookup"><span data-stu-id="69fa6-105">Describes the status of the provisioning event and the associated errors.</span></span> 

## <a name="properties"></a><span data-ttu-id="69fa6-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="69fa6-106">Properties</span></span>

| <span data-ttu-id="69fa6-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="69fa6-107">Property</span></span>     | <span data-ttu-id="69fa6-108">Тип</span><span class="sxs-lookup"><span data-stu-id="69fa6-108">Type</span></span>        | <span data-ttu-id="69fa6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="69fa6-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="69fa6-110">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="69fa6-110">additionalDetails</span></span>|<span data-ttu-id="69fa6-111">String</span><span class="sxs-lookup"><span data-stu-id="69fa6-111">String</span></span>|<span data-ttu-id="69fa6-112">Дополнительные сведения в случае ошибки.</span><span class="sxs-lookup"><span data-stu-id="69fa6-112">Additional details in case of error.</span></span>|
|<span data-ttu-id="69fa6-113">ошибкаКатегория</span><span class="sxs-lookup"><span data-stu-id="69fa6-113">errorCategory</span></span>|<span data-ttu-id="69fa6-114">положениеСтатусЭррорКатегория</span><span class="sxs-lookup"><span data-stu-id="69fa6-114">provisioningStatusErrorCategory</span></span>|<span data-ttu-id="69fa6-115">Классифицирует код ошибки.</span><span class="sxs-lookup"><span data-stu-id="69fa6-115">Categorizes the error code.</span></span> <span data-ttu-id="69fa6-116">Возможные `failure` значения, `nonServiceFailure` `success` , `unknownFutureValue`</span><span class="sxs-lookup"><span data-stu-id="69fa6-116">Possible values are `failure`, `nonServiceFailure`, `success`, `unknownFutureValue`</span></span>|
|<span data-ttu-id="69fa6-117">errorCode</span><span class="sxs-lookup"><span data-stu-id="69fa6-117">errorCode</span></span>|<span data-ttu-id="69fa6-118">String</span><span class="sxs-lookup"><span data-stu-id="69fa6-118">String</span></span>|<span data-ttu-id="69fa6-119">Уникальный код ошибки, если таковые имели место.</span><span class="sxs-lookup"><span data-stu-id="69fa6-119">Unique error code if any occurred.</span></span> [<span data-ttu-id="69fa6-120">Подробнее</span><span class="sxs-lookup"><span data-stu-id="69fa6-120">Learn more</span></span>](/azure/active-directory/reports-monitoring/concept-provisioning-logs#error-codes)|
|<span data-ttu-id="69fa6-121">reason</span><span class="sxs-lookup"><span data-stu-id="69fa6-121">reason</span></span>|<span data-ttu-id="69fa6-122">String</span><span class="sxs-lookup"><span data-stu-id="69fa6-122">String</span></span>|<span data-ttu-id="69fa6-123">Суммирует статус и описывает, почему статус произошел.</span><span class="sxs-lookup"><span data-stu-id="69fa6-123">Summarizes the status and describes why the status happened.</span></span>|
|<span data-ttu-id="69fa6-124">рекомендуемая Действий</span><span class="sxs-lookup"><span data-stu-id="69fa6-124">recommendedAction</span></span>|<span data-ttu-id="69fa6-125">String</span><span class="sxs-lookup"><span data-stu-id="69fa6-125">String</span></span>|<span data-ttu-id="69fa6-126">Предоставляет разрешение для соответствующей ошибки.</span><span class="sxs-lookup"><span data-stu-id="69fa6-126">Provides the resolution for the corresponding error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="69fa6-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="69fa6-127">JSON representation</span></span>

<span data-ttu-id="69fa6-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="69fa6-128">The following is a JSON representation of the resource.</span></span>

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


