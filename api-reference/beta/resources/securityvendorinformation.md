---
title: Тип ресурса Секуритивендоринформатион
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: f0c0142333237c1c4700353b01f75b9867b85ad7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988830"
---
# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="590f0-104">Тип ресурса Секуритивендоринформатион</span><span class="sxs-lookup"><span data-stu-id="590f0-104">securityVendorInformation resource type</span></span>

<span data-ttu-id="590f0-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="590f0-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="590f0-106">Содержит сведения о продуктах, поставщиках и подценнях безопасности (например, Vendor = Microsoft; Provider = защитник Windows ATP; подпредоставление = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="590f0-106">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="590f0-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="590f0-107">Properties</span></span>

| <span data-ttu-id="590f0-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="590f0-108">Property</span></span>   | <span data-ttu-id="590f0-109">Тип</span><span class="sxs-lookup"><span data-stu-id="590f0-109">Type</span></span>|<span data-ttu-id="590f0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="590f0-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="590f0-111">поставщики</span><span class="sxs-lookup"><span data-stu-id="590f0-111">provider</span></span> |<span data-ttu-id="590f0-112">String</span><span class="sxs-lookup"><span data-stu-id="590f0-112">String</span></span>|<span data-ttu-id="590f0-113">Конкретный поставщик (продукт или услуга — не компания поставщика); Например, Виндовсдефендератп.</span><span class="sxs-lookup"><span data-stu-id="590f0-113">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="590f0-114">провидерверсион</span><span class="sxs-lookup"><span data-stu-id="590f0-114">providerVersion</span></span>|<span data-ttu-id="590f0-115">String</span><span class="sxs-lookup"><span data-stu-id="590f0-115">String</span></span>|<span data-ttu-id="590f0-116">Версия поставщика или подсистемы, если она существует, создавшего оповещение.</span><span class="sxs-lookup"><span data-stu-id="590f0-116">Version of the provider or subprovider, if it exists, that generated the alert.</span></span> <span data-ttu-id="590f0-117">**Required**</span><span class="sxs-lookup"><span data-stu-id="590f0-117">**Required**</span></span>|
|<span data-ttu-id="590f0-118">подпредоставление</span><span class="sxs-lookup"><span data-stu-id="590f0-118">subProvider</span></span>|<span data-ttu-id="590f0-119">String</span><span class="sxs-lookup"><span data-stu-id="590f0-119">String</span></span>|<span data-ttu-id="590f0-120">Конкретный подпредоставленный поставщик (в разделе Поставщик статистической обработки); Например, Виндовсдефендератп. SmartScreen.</span><span class="sxs-lookup"><span data-stu-id="590f0-120">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="590f0-121">поставщика</span><span class="sxs-lookup"><span data-stu-id="590f0-121">vendor</span></span> |<span data-ttu-id="590f0-122">String</span><span class="sxs-lookup"><span data-stu-id="590f0-122">String</span></span>|<span data-ttu-id="590f0-123">Имя поставщика оповещений (например, Microsoft, Dell, Фирие).</span><span class="sxs-lookup"><span data-stu-id="590f0-123">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span> <span data-ttu-id="590f0-124">**Required**</span><span class="sxs-lookup"><span data-stu-id="590f0-124">**Required**</span></span>|

## <a name="json-representation"></a><span data-ttu-id="590f0-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="590f0-125">JSON representation</span></span>

<span data-ttu-id="590f0-126">Следующем — это представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="590f0-126">The folllowing is a JSON representation of the resource.</span></span>
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


