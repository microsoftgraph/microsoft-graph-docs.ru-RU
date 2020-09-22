---
title: Тип ресурса Секуритивендоринформатион
description: " поддается подпредоставлению = AppLocker)."
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 536ed37cfe8ba190a22ef86e190af2b171d352ae
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47983986"
---
# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="94109-103">Тип ресурса Секуритивендоринформатион</span><span class="sxs-lookup"><span data-stu-id="94109-103">securityVendorInformation resource type</span></span>

<span data-ttu-id="94109-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94109-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="94109-105">Содержит сведения о продуктах, поставщиках и подценнях безопасности (например, Vendor = Microsoft; Provider = защитник Windows ATP; подпредоставление = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="94109-105">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="94109-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="94109-106">Properties</span></span>

| <span data-ttu-id="94109-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="94109-107">Property</span></span>   | <span data-ttu-id="94109-108">Тип</span><span class="sxs-lookup"><span data-stu-id="94109-108">Type</span></span>|<span data-ttu-id="94109-109">Описание</span><span class="sxs-lookup"><span data-stu-id="94109-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="94109-110">поставщики</span><span class="sxs-lookup"><span data-stu-id="94109-110">provider</span></span> |<span data-ttu-id="94109-111">String</span><span class="sxs-lookup"><span data-stu-id="94109-111">String</span></span>|<span data-ttu-id="94109-112">Конкретный поставщик (продукт или услуга — не компания поставщика); Например, Виндовсдефендератп.</span><span class="sxs-lookup"><span data-stu-id="94109-112">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="94109-113">провидерверсион</span><span class="sxs-lookup"><span data-stu-id="94109-113">providerVersion</span></span>|<span data-ttu-id="94109-114">String</span><span class="sxs-lookup"><span data-stu-id="94109-114">String</span></span>|<span data-ttu-id="94109-115">Версия поставщика или подсистемы, если она существует, создавшего оповещение.</span><span class="sxs-lookup"><span data-stu-id="94109-115">Version of the provider or subprovider, if it exists, that generated the alert.</span></span> <span data-ttu-id="94109-116">*Required*</span><span class="sxs-lookup"><span data-stu-id="94109-116">*Required*</span></span>|
|<span data-ttu-id="94109-117">подпредоставление</span><span class="sxs-lookup"><span data-stu-id="94109-117">subProvider</span></span>|<span data-ttu-id="94109-118">String</span><span class="sxs-lookup"><span data-stu-id="94109-118">String</span></span>|<span data-ttu-id="94109-119">Конкретный подпредоставленный поставщик (в разделе Поставщик статистической обработки); Например, Виндовсдефендератп. SmartScreen.</span><span class="sxs-lookup"><span data-stu-id="94109-119">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="94109-120">поставщика</span><span class="sxs-lookup"><span data-stu-id="94109-120">vendor</span></span> |<span data-ttu-id="94109-121">String</span><span class="sxs-lookup"><span data-stu-id="94109-121">String</span></span>|<span data-ttu-id="94109-122">Имя поставщика оповещений (например, Microsoft, Dell, Фирие).</span><span class="sxs-lookup"><span data-stu-id="94109-122">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span> <span data-ttu-id="94109-123">*Required*</span><span class="sxs-lookup"><span data-stu-id="94109-123">*Required*</span></span>|


## <a name="json-representation"></a><span data-ttu-id="94109-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="94109-124">JSON representation</span></span>

<span data-ttu-id="94109-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="94109-125">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.securityVendorInformation"
}-->

```json
{
  "provider": "String",
  "providerVersion": "String",
  "subProvider": "String",
  "vendor": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityVendorInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

