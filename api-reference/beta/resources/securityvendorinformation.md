---
title: Тип ресурса Секуритивендоринформатион
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: d543bf16617ed28d50d2e7082372ff2014cd24c5
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343303"
---
# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="d22a1-104">Тип ресурса Секуритивендоринформатион</span><span class="sxs-lookup"><span data-stu-id="d22a1-104">securityVendorInformation resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d22a1-105">Содержит сведения о продуктах, поставщиках и подценнях безопасности (например, Vendor = Microsoft; Provider = защитник Windows ATP; подПредоставление = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="d22a1-105">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="d22a1-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="d22a1-106">Properties</span></span>

| <span data-ttu-id="d22a1-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="d22a1-107">Property</span></span>   | <span data-ttu-id="d22a1-108">Тип</span><span class="sxs-lookup"><span data-stu-id="d22a1-108">Type</span></span>|<span data-ttu-id="d22a1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d22a1-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d22a1-110">поставщики</span><span class="sxs-lookup"><span data-stu-id="d22a1-110">provider</span></span> |<span data-ttu-id="d22a1-111">String</span><span class="sxs-lookup"><span data-stu-id="d22a1-111">String</span></span>|<span data-ttu-id="d22a1-112">Конкретный поставщик (продукт или услуга — не компания поставщика); Например, Виндовсдефендератп.</span><span class="sxs-lookup"><span data-stu-id="d22a1-112">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="d22a1-113">Провидерверсион</span><span class="sxs-lookup"><span data-stu-id="d22a1-113">providerVersion</span></span>|<span data-ttu-id="d22a1-114">String</span><span class="sxs-lookup"><span data-stu-id="d22a1-114">String</span></span>|<span data-ttu-id="d22a1-115">Версия поставщика или подСистемы, если она существует, создавшего оповещение.</span><span class="sxs-lookup"><span data-stu-id="d22a1-115">Version of the provider or subprovider, if it exists, that generated the alert.</span></span> <span data-ttu-id="d22a1-116">**Required**</span><span class="sxs-lookup"><span data-stu-id="d22a1-116">**Required**</span></span>|
|<span data-ttu-id="d22a1-117">подПредоставление</span><span class="sxs-lookup"><span data-stu-id="d22a1-117">subProvider</span></span>|<span data-ttu-id="d22a1-118">String</span><span class="sxs-lookup"><span data-stu-id="d22a1-118">String</span></span>|<span data-ttu-id="d22a1-119">Конкретный подпредоставленный поставщик (в разделе Поставщик статистической обработки); Например, Виндовсдефендератп. SmartScreen.</span><span class="sxs-lookup"><span data-stu-id="d22a1-119">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="d22a1-120">поставщика</span><span class="sxs-lookup"><span data-stu-id="d22a1-120">vendor</span></span> |<span data-ttu-id="d22a1-121">String</span><span class="sxs-lookup"><span data-stu-id="d22a1-121">String</span></span>|<span data-ttu-id="d22a1-122">Имя поставщика оповещений (например, Microsoft, Dell, Фирие).</span><span class="sxs-lookup"><span data-stu-id="d22a1-122">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span> <span data-ttu-id="d22a1-123">**Required**</span><span class="sxs-lookup"><span data-stu-id="d22a1-123">**Required**</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d22a1-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d22a1-124">JSON representation</span></span>

<span data-ttu-id="d22a1-125">Следующем — это представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d22a1-125">The folllowing is a JSON representation of the resource.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "securityVendorInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
