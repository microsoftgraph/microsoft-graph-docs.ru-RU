---
title: тип ресурса provisioningErrorInfo
description: Описывает состояние события подготовка и связанные с ним ошибки.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 839370e0dc15ee247997b6d934107e27f62cc87a
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232995"
---
# <a name="provisioningerrorinfo-resource-type"></a><span data-ttu-id="d18ce-103">тип ресурса provisioningErrorInfo</span><span class="sxs-lookup"><span data-stu-id="d18ce-103">provisioningErrorInfo resource type</span></span>

<span data-ttu-id="d18ce-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d18ce-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d18ce-105">Описывает состояние события подготовка и связанные с ним ошибки.</span><span class="sxs-lookup"><span data-stu-id="d18ce-105">Describes the status of the provisioning event and the associated errors.</span></span> 

## <a name="properties"></a><span data-ttu-id="d18ce-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="d18ce-106">Properties</span></span>

| <span data-ttu-id="d18ce-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="d18ce-107">Property</span></span>     | <span data-ttu-id="d18ce-108">Тип</span><span class="sxs-lookup"><span data-stu-id="d18ce-108">Type</span></span>        | <span data-ttu-id="d18ce-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d18ce-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d18ce-110">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="d18ce-110">additionalDetails</span></span>|<span data-ttu-id="d18ce-111">String</span><span class="sxs-lookup"><span data-stu-id="d18ce-111">String</span></span>|<span data-ttu-id="d18ce-112">Дополнительные сведения в случае ошибки.</span><span class="sxs-lookup"><span data-stu-id="d18ce-112">Additional details in case of error.</span></span>|
|<span data-ttu-id="d18ce-113">errorCategory</span><span class="sxs-lookup"><span data-stu-id="d18ce-113">errorCategory</span></span>|<span data-ttu-id="d18ce-114">String</span><span class="sxs-lookup"><span data-stu-id="d18ce-114">String</span></span>|<span data-ttu-id="d18ce-115">Классифицировать код ошибки.</span><span class="sxs-lookup"><span data-stu-id="d18ce-115">Categorizes the error code.</span></span> <span data-ttu-id="d18ce-116">Возможные значения `failure` : `nonServiceFailure` , `success` , `unknownFutureValue`</span><span class="sxs-lookup"><span data-stu-id="d18ce-116">Possible values are `failure`, `nonServiceFailure`, `success`, `unknownFutureValue`</span></span>|
|<span data-ttu-id="d18ce-117">errorCode</span><span class="sxs-lookup"><span data-stu-id="d18ce-117">errorCode</span></span>|<span data-ttu-id="d18ce-118">String</span><span class="sxs-lookup"><span data-stu-id="d18ce-118">String</span></span>|<span data-ttu-id="d18ce-119">Уникальный код ошибки, если таковое произошло.</span><span class="sxs-lookup"><span data-stu-id="d18ce-119">Unique error code if any occurred.</span></span> [<span data-ttu-id="d18ce-120">Подробнее</span><span class="sxs-lookup"><span data-stu-id="d18ce-120">Learn more</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs#error-codes)|
|<span data-ttu-id="d18ce-121">reason</span><span class="sxs-lookup"><span data-stu-id="d18ce-121">reason</span></span>|<span data-ttu-id="d18ce-122">String</span><span class="sxs-lookup"><span data-stu-id="d18ce-122">String</span></span>|<span data-ttu-id="d18ce-123">Суммирует состояние и описывает причины, по которым произошел этот статус.</span><span class="sxs-lookup"><span data-stu-id="d18ce-123">Summarizes the status and describes why the status happened.</span></span>|
|<span data-ttu-id="d18ce-124">recommendedAction</span><span class="sxs-lookup"><span data-stu-id="d18ce-124">recommendedAction</span></span>|<span data-ttu-id="d18ce-125">String</span><span class="sxs-lookup"><span data-stu-id="d18ce-125">String</span></span>|<span data-ttu-id="d18ce-126">Обеспечивает разрешение соответствующей ошибки.</span><span class="sxs-lookup"><span data-stu-id="d18ce-126">Provides the resolution for the corresponding error.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d18ce-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d18ce-127">JSON representation</span></span>

<span data-ttu-id="d18ce-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d18ce-128">The following is a JSON representation of the resource.</span></span>

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


