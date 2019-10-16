---
title: Тип ресурса Секуритивендоринформатион
description: " поддается подпредоставлению = AppLocker)."
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: d7af6e0903e3d178bacdd7c86b4a2cab04285171
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536099"
---
# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="eb7f1-103">Тип ресурса Секуритивендоринформатион</span><span class="sxs-lookup"><span data-stu-id="eb7f1-103">securityVendorInformation resource type</span></span>

<span data-ttu-id="eb7f1-104">Содержит сведения о продуктах, поставщиках и подценнях безопасности (например, Vendor = Microsoft; Provider = защитник Windows ATP; подпредоставление = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="eb7f1-104">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="eb7f1-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="eb7f1-105">Properties</span></span>

| <span data-ttu-id="eb7f1-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="eb7f1-106">Property</span></span>   | <span data-ttu-id="eb7f1-107">Тип</span><span class="sxs-lookup"><span data-stu-id="eb7f1-107">Type</span></span>|<span data-ttu-id="eb7f1-108">Описание</span><span class="sxs-lookup"><span data-stu-id="eb7f1-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eb7f1-109">поставщики</span><span class="sxs-lookup"><span data-stu-id="eb7f1-109">provider</span></span> |<span data-ttu-id="eb7f1-110">String</span><span class="sxs-lookup"><span data-stu-id="eb7f1-110">String</span></span>|<span data-ttu-id="eb7f1-111">Конкретный поставщик (продукт или услуга — не компания поставщика); Например, Виндовсдефендератп.</span><span class="sxs-lookup"><span data-stu-id="eb7f1-111">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="eb7f1-112">провидерверсион</span><span class="sxs-lookup"><span data-stu-id="eb7f1-112">providerVersion</span></span>|<span data-ttu-id="eb7f1-113">String</span><span class="sxs-lookup"><span data-stu-id="eb7f1-113">String</span></span>|<span data-ttu-id="eb7f1-114">Версия поставщика или подсистемы, если она существует, создавшего оповещение.</span><span class="sxs-lookup"><span data-stu-id="eb7f1-114">Version of the provider or subprovider, if it exists, that generated the alert.</span></span> <span data-ttu-id="eb7f1-115">*Required*</span><span class="sxs-lookup"><span data-stu-id="eb7f1-115">*Required*</span></span>|
|<span data-ttu-id="eb7f1-116">подпредоставление</span><span class="sxs-lookup"><span data-stu-id="eb7f1-116">subProvider</span></span>|<span data-ttu-id="eb7f1-117">String</span><span class="sxs-lookup"><span data-stu-id="eb7f1-117">String</span></span>|<span data-ttu-id="eb7f1-118">Конкретный подпредоставленный поставщик (в разделе Поставщик статистической обработки); Например, Виндовсдефендератп. SmartScreen.</span><span class="sxs-lookup"><span data-stu-id="eb7f1-118">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="eb7f1-119">поставщика</span><span class="sxs-lookup"><span data-stu-id="eb7f1-119">vendor</span></span> |<span data-ttu-id="eb7f1-120">String</span><span class="sxs-lookup"><span data-stu-id="eb7f1-120">String</span></span>|<span data-ttu-id="eb7f1-121">Имя поставщика оповещений (например, Microsoft, Dell, Фирие).</span><span class="sxs-lookup"><span data-stu-id="eb7f1-121">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span> <span data-ttu-id="eb7f1-122">*Required*</span><span class="sxs-lookup"><span data-stu-id="eb7f1-122">*Required*</span></span>|


## <a name="json-representation"></a><span data-ttu-id="eb7f1-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eb7f1-123">JSON representation</span></span>

<span data-ttu-id="eb7f1-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eb7f1-124">The following is a JSON representation of the resource.</span></span>
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
