---
title: Тип ресурса Секуритивендоринформатион
description: " подДается подПредоставлению = AppLocker)."
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: fb5dee36da08332fd5c36f7ee4e578cc9fb7deaa
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549701"
---
# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="14ace-103">Тип ресурса Секуритивендоринформатион</span><span class="sxs-lookup"><span data-stu-id="14ace-103">securityVendorInformation resource type</span></span>

<span data-ttu-id="14ace-104">Содержит сведения о продуктах, поставщиках и подценнях безопасности (например, Vendor = Microsoft; Provider = защитник Windows ATP; подПредоставление = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="14ace-104">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="14ace-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="14ace-105">Properties</span></span>

| <span data-ttu-id="14ace-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="14ace-106">Property</span></span>   | <span data-ttu-id="14ace-107">Тип</span><span class="sxs-lookup"><span data-stu-id="14ace-107">Type</span></span>|<span data-ttu-id="14ace-108">Описание</span><span class="sxs-lookup"><span data-stu-id="14ace-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="14ace-109">поставщики</span><span class="sxs-lookup"><span data-stu-id="14ace-109">provider</span></span> |<span data-ttu-id="14ace-110">String</span><span class="sxs-lookup"><span data-stu-id="14ace-110">String</span></span>|<span data-ttu-id="14ace-111">Конкретный поставщик (продукт или услуга — не компания поставщика); Например, Виндовсдефендератп.</span><span class="sxs-lookup"><span data-stu-id="14ace-111">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="14ace-112">Провидерверсион</span><span class="sxs-lookup"><span data-stu-id="14ace-112">providerVersion</span></span>|<span data-ttu-id="14ace-113">String</span><span class="sxs-lookup"><span data-stu-id="14ace-113">String</span></span>|<span data-ttu-id="14ace-114">Версия поставщика или подСистемы, если она существует, создавшего оповещение.</span><span class="sxs-lookup"><span data-stu-id="14ace-114">Version of the provider or subprovider, if it exists, that generated the alert.</span></span> <span data-ttu-id="14ace-115">*Required*</span><span class="sxs-lookup"><span data-stu-id="14ace-115">*Required*</span></span>|
|<span data-ttu-id="14ace-116">подПредоставление</span><span class="sxs-lookup"><span data-stu-id="14ace-116">subProvider</span></span>|<span data-ttu-id="14ace-117">String</span><span class="sxs-lookup"><span data-stu-id="14ace-117">String</span></span>|<span data-ttu-id="14ace-118">Конкретный подпредоставленный поставщик (в разделе Поставщик статистической обработки); Например, Виндовсдефендератп. SmartScreen.</span><span class="sxs-lookup"><span data-stu-id="14ace-118">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="14ace-119">поставщика</span><span class="sxs-lookup"><span data-stu-id="14ace-119">vendor</span></span> |<span data-ttu-id="14ace-120">String</span><span class="sxs-lookup"><span data-stu-id="14ace-120">String</span></span>|<span data-ttu-id="14ace-121">Имя поставщика оповещений (например, Microsoft, Dell, Фирие).</span><span class="sxs-lookup"><span data-stu-id="14ace-121">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span> <span data-ttu-id="14ace-122">*Required*</span><span class="sxs-lookup"><span data-stu-id="14ace-122">*Required*</span></span>|


## <a name="json-representation"></a><span data-ttu-id="14ace-123">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="14ace-123">JSON representation</span></span>

<span data-ttu-id="14ace-124">Следующем — это представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="14ace-124">The folllowing is a JSON representation of the resource.</span></span>
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
