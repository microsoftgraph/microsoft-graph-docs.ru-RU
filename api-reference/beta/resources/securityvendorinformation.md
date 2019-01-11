---
title: Тип ресурса securityVendorInformation
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
ms.openlocfilehash: 34e565a69f716f0d167240ab753e5d192758508a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884387"
---
# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="196f8-104">Тип ресурса securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="196f8-104">securityVendorInformation resource type</span></span>

 > <span data-ttu-id="196f8-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="196f8-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="196f8-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="196f8-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="196f8-107">Содержит сведения о безопасности продуктов и услуг поставщика, поставщик и subprovider (например, поставщика = корпорации Майкрософт; поставщика = ATP Защитник Windows; subProvider = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="196f8-107">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="196f8-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="196f8-108">Properties</span></span>

| <span data-ttu-id="196f8-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="196f8-109">Property</span></span>   | <span data-ttu-id="196f8-110">Тип</span><span class="sxs-lookup"><span data-stu-id="196f8-110">Type</span></span>|<span data-ttu-id="196f8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="196f8-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="196f8-112">Поставщик</span><span class="sxs-lookup"><span data-stu-id="196f8-112">provider</span></span> |<span data-ttu-id="196f8-113">Строка</span><span class="sxs-lookup"><span data-stu-id="196f8-113">String</span></span>|<span data-ttu-id="196f8-114">Определенного поставщика (продуктов и услуг - не поставщика организации); Например WindowsDefenderATP.</span><span class="sxs-lookup"><span data-stu-id="196f8-114">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="196f8-115">providerVersion</span><span class="sxs-lookup"><span data-stu-id="196f8-115">providerVersion</span></span>|<span data-ttu-id="196f8-116">Строка</span><span class="sxs-lookup"><span data-stu-id="196f8-116">String</span></span>|<span data-ttu-id="196f8-117">Версия поставщика или subprovider, если он существует, создавшее оповещение.</span><span class="sxs-lookup"><span data-stu-id="196f8-117">Version of the provider or subprovider, if it exists, that generated the alert.</span></span> <span data-ttu-id="196f8-118">*Required*</span><span class="sxs-lookup"><span data-stu-id="196f8-118">*Required*</span></span>|
|<span data-ttu-id="196f8-119">subProvider</span><span class="sxs-lookup"><span data-stu-id="196f8-119">subProvider</span></span>|<span data-ttu-id="196f8-120">Строка</span><span class="sxs-lookup"><span data-stu-id="196f8-120">String</span></span>|<span data-ttu-id="196f8-121">Определенные subprovider (в разделе статистической обработки поставщика); Например WindowsDefenderATP.SmartScreen.</span><span class="sxs-lookup"><span data-stu-id="196f8-121">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="196f8-122">поставщика</span><span class="sxs-lookup"><span data-stu-id="196f8-122">vendor</span></span> |<span data-ttu-id="196f8-123">Строка</span><span class="sxs-lookup"><span data-stu-id="196f8-123">String</span></span>|<span data-ttu-id="196f8-124">Имя оповещения поставщика (например, Microsoft, Dell, FireEye).</span><span class="sxs-lookup"><span data-stu-id="196f8-124">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span> <span data-ttu-id="196f8-125">*Required*</span><span class="sxs-lookup"><span data-stu-id="196f8-125">*Required*</span></span>|

## <a name="json-representation"></a><span data-ttu-id="196f8-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="196f8-126">JSON representation</span></span>

<span data-ttu-id="196f8-127">Соответствовать является представлением JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="196f8-127">The folllowing is a JSON representation of the resource.</span></span>
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
