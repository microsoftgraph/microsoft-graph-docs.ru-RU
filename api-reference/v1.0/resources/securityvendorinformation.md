---
title: Тип ресурса securityVendorInformation
description: " subProvider = AppLocker)."
localization_priority: Normal
ms.openlocfilehash: e9d8551c085c05007388bf0c6e33143994c6969b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820148"
---
# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="ee3c5-103">Тип ресурса securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="ee3c5-103">securityVendorInformation resource type</span></span>

<span data-ttu-id="ee3c5-104">Содержит сведения о безопасности продуктов и услуг поставщика, поставщик и subprovider (например, поставщика = корпорации Майкрософт; поставщика = ATP Защитник Windows; subProvider = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="ee3c5-104">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="ee3c5-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="ee3c5-105">Properties</span></span>

| <span data-ttu-id="ee3c5-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="ee3c5-106">Property</span></span>   | <span data-ttu-id="ee3c5-107">Тип</span><span class="sxs-lookup"><span data-stu-id="ee3c5-107">Type</span></span>|<span data-ttu-id="ee3c5-108">Описание</span><span class="sxs-lookup"><span data-stu-id="ee3c5-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ee3c5-109">Поставщик</span><span class="sxs-lookup"><span data-stu-id="ee3c5-109">provider</span></span> |<span data-ttu-id="ee3c5-110">Строка</span><span class="sxs-lookup"><span data-stu-id="ee3c5-110">String</span></span>|<span data-ttu-id="ee3c5-111">Определенного поставщика (продуктов и услуг - не поставщика организации); Например WindowsDefenderATP.</span><span class="sxs-lookup"><span data-stu-id="ee3c5-111">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="ee3c5-112">providerVersion</span><span class="sxs-lookup"><span data-stu-id="ee3c5-112">providerVersion</span></span>|<span data-ttu-id="ee3c5-113">Строка</span><span class="sxs-lookup"><span data-stu-id="ee3c5-113">String</span></span>|<span data-ttu-id="ee3c5-114">Версия поставщика или subprovider, если он существует, создавшее оповещение.</span><span class="sxs-lookup"><span data-stu-id="ee3c5-114">Version of the provider or subprovider, if it exists, that generated the alert.</span></span> <span data-ttu-id="ee3c5-115">*Required*</span><span class="sxs-lookup"><span data-stu-id="ee3c5-115">*Required*</span></span>|
|<span data-ttu-id="ee3c5-116">subProvider</span><span class="sxs-lookup"><span data-stu-id="ee3c5-116">subProvider</span></span>|<span data-ttu-id="ee3c5-117">Строка</span><span class="sxs-lookup"><span data-stu-id="ee3c5-117">String</span></span>|<span data-ttu-id="ee3c5-118">Определенные subprovider (в разделе статистической обработки поставщика); Например WindowsDefenderATP.SmartScreen.</span><span class="sxs-lookup"><span data-stu-id="ee3c5-118">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="ee3c5-119">поставщика</span><span class="sxs-lookup"><span data-stu-id="ee3c5-119">vendor</span></span> |<span data-ttu-id="ee3c5-120">Строка</span><span class="sxs-lookup"><span data-stu-id="ee3c5-120">String</span></span>|<span data-ttu-id="ee3c5-121">Имя оповещения поставщика (например, Microsoft, Dell, FireEye).</span><span class="sxs-lookup"><span data-stu-id="ee3c5-121">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span> <span data-ttu-id="ee3c5-122">*Required*</span><span class="sxs-lookup"><span data-stu-id="ee3c5-122">*Required*</span></span>|


## <a name="json-representation"></a><span data-ttu-id="ee3c5-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ee3c5-123">JSON representation</span></span>

<span data-ttu-id="ee3c5-124">Соответствовать является представлением JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="ee3c5-124">The folllowing is a JSON representation of the resource.</span></span>
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
