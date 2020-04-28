---
title: Тип ресурса Секуритивендоринформатион
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 517213e3e2266681eee0f6bdca53b0b9ce5a0bb3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520810"
---
# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="daaa9-104">Тип ресурса Секуритивендоринформатион</span><span class="sxs-lookup"><span data-stu-id="daaa9-104">securityVendorInformation resource type</span></span>

<span data-ttu-id="daaa9-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="daaa9-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="daaa9-106">Содержит сведения о продуктах, поставщиках и подценнях безопасности (например, Vendor = Microsoft; Provider = защитник Windows ATP; подпредоставление = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="daaa9-106">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="daaa9-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="daaa9-107">Properties</span></span>

| <span data-ttu-id="daaa9-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="daaa9-108">Property</span></span>   | <span data-ttu-id="daaa9-109">Тип</span><span class="sxs-lookup"><span data-stu-id="daaa9-109">Type</span></span>|<span data-ttu-id="daaa9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="daaa9-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="daaa9-111">поставщики</span><span class="sxs-lookup"><span data-stu-id="daaa9-111">provider</span></span> |<span data-ttu-id="daaa9-112">String</span><span class="sxs-lookup"><span data-stu-id="daaa9-112">String</span></span>|<span data-ttu-id="daaa9-113">Конкретный поставщик (продукт или услуга — не компания поставщика); Например, Виндовсдефендератп.</span><span class="sxs-lookup"><span data-stu-id="daaa9-113">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="daaa9-114">провидерверсион</span><span class="sxs-lookup"><span data-stu-id="daaa9-114">providerVersion</span></span>|<span data-ttu-id="daaa9-115">String</span><span class="sxs-lookup"><span data-stu-id="daaa9-115">String</span></span>|<span data-ttu-id="daaa9-116">Версия поставщика или подсистемы, если она существует, создавшего оповещение.</span><span class="sxs-lookup"><span data-stu-id="daaa9-116">Version of the provider or subprovider, if it exists, that generated the alert.</span></span> <span data-ttu-id="daaa9-117">**Required**</span><span class="sxs-lookup"><span data-stu-id="daaa9-117">**Required**</span></span>|
|<span data-ttu-id="daaa9-118">подпредоставление</span><span class="sxs-lookup"><span data-stu-id="daaa9-118">subProvider</span></span>|<span data-ttu-id="daaa9-119">String</span><span class="sxs-lookup"><span data-stu-id="daaa9-119">String</span></span>|<span data-ttu-id="daaa9-120">Конкретный подпредоставленный поставщик (в разделе Поставщик статистической обработки); Например, Виндовсдефендератп. SmartScreen.</span><span class="sxs-lookup"><span data-stu-id="daaa9-120">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="daaa9-121">поставщика</span><span class="sxs-lookup"><span data-stu-id="daaa9-121">vendor</span></span> |<span data-ttu-id="daaa9-122">String</span><span class="sxs-lookup"><span data-stu-id="daaa9-122">String</span></span>|<span data-ttu-id="daaa9-123">Имя поставщика оповещений (например, Microsoft, Dell, Фирие).</span><span class="sxs-lookup"><span data-stu-id="daaa9-123">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span> <span data-ttu-id="daaa9-124">**Required**</span><span class="sxs-lookup"><span data-stu-id="daaa9-124">**Required**</span></span>|

## <a name="json-representation"></a><span data-ttu-id="daaa9-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="daaa9-125">JSON representation</span></span>

<span data-ttu-id="daaa9-126">Следующем — это представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="daaa9-126">The folllowing is a JSON representation of the resource.</span></span>
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
