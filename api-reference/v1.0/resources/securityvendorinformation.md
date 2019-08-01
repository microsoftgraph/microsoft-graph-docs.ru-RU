---
title: Тип ресурса Секуритивендоринформатион
description: " поддается подпредоставлению = AppLocker)."
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 3fb959da2d6af10632f9113a33eb942492b679ef
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034428"
---
# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="363d2-103">Тип ресурса Секуритивендоринформатион</span><span class="sxs-lookup"><span data-stu-id="363d2-103">securityVendorInformation resource type</span></span>

<span data-ttu-id="363d2-104">Содержит сведения о продуктах, поставщиках и подценнях безопасности (например, Vendor = Microsoft; Provider = защитник Windows ATP; подпредоставление = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="363d2-104">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="363d2-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="363d2-105">Properties</span></span>

| <span data-ttu-id="363d2-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="363d2-106">Property</span></span>   | <span data-ttu-id="363d2-107">Тип</span><span class="sxs-lookup"><span data-stu-id="363d2-107">Type</span></span>|<span data-ttu-id="363d2-108">Описание</span><span class="sxs-lookup"><span data-stu-id="363d2-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="363d2-109">поставщики</span><span class="sxs-lookup"><span data-stu-id="363d2-109">provider</span></span> |<span data-ttu-id="363d2-110">String</span><span class="sxs-lookup"><span data-stu-id="363d2-110">String</span></span>|<span data-ttu-id="363d2-111">Конкретный поставщик (продукт или услуга — не компания поставщика); Например, Виндовсдефендератп.</span><span class="sxs-lookup"><span data-stu-id="363d2-111">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="363d2-112">Провидерверсион</span><span class="sxs-lookup"><span data-stu-id="363d2-112">providerVersion</span></span>|<span data-ttu-id="363d2-113">String</span><span class="sxs-lookup"><span data-stu-id="363d2-113">String</span></span>|<span data-ttu-id="363d2-114">Версия поставщика или подсистемы, если она существует, создавшего оповещение.</span><span class="sxs-lookup"><span data-stu-id="363d2-114">Version of the provider or subprovider, if it exists, that generated the alert.</span></span> <span data-ttu-id="363d2-115">*Required*</span><span class="sxs-lookup"><span data-stu-id="363d2-115">*Required*</span></span>|
|<span data-ttu-id="363d2-116">подпредоставление</span><span class="sxs-lookup"><span data-stu-id="363d2-116">subProvider</span></span>|<span data-ttu-id="363d2-117">String</span><span class="sxs-lookup"><span data-stu-id="363d2-117">String</span></span>|<span data-ttu-id="363d2-118">Конкретный подпредоставленный поставщик (в разделе Поставщик статистической обработки); Например, Виндовсдефендератп. SmartScreen.</span><span class="sxs-lookup"><span data-stu-id="363d2-118">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="363d2-119">поставщика</span><span class="sxs-lookup"><span data-stu-id="363d2-119">vendor</span></span> |<span data-ttu-id="363d2-120">String</span><span class="sxs-lookup"><span data-stu-id="363d2-120">String</span></span>|<span data-ttu-id="363d2-121">Имя поставщика оповещений (например, Microsoft, Dell, Фирие).</span><span class="sxs-lookup"><span data-stu-id="363d2-121">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span> <span data-ttu-id="363d2-122">*Required*</span><span class="sxs-lookup"><span data-stu-id="363d2-122">*Required*</span></span>|


## <a name="json-representation"></a><span data-ttu-id="363d2-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="363d2-123">JSON representation</span></span>

<span data-ttu-id="363d2-124">Следующем — это представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="363d2-124">The folllowing is a JSON representation of the resource.</span></span>
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
