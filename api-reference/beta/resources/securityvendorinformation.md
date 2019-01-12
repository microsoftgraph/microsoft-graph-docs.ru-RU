---
title: Тип ресурса securityVendorInformation
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 0137abd7a9df0df94f73e18d7efa201008031ff6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939926"
---
# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="0595d-104">Тип ресурса securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="0595d-104">securityVendorInformation resource type</span></span>

 > <span data-ttu-id="0595d-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0595d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0595d-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0595d-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0595d-107">Содержит сведения о безопасности продуктов и услуг поставщика, поставщик и subprovider (например, поставщика = корпорации Майкрософт; поставщика = ATP Защитник Windows; subProvider = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="0595d-107">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="0595d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0595d-108">Properties</span></span>

| <span data-ttu-id="0595d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0595d-109">Property</span></span>   | <span data-ttu-id="0595d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0595d-110">Type</span></span>|<span data-ttu-id="0595d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0595d-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0595d-112">Поставщик</span><span class="sxs-lookup"><span data-stu-id="0595d-112">provider</span></span> |<span data-ttu-id="0595d-113">Строка</span><span class="sxs-lookup"><span data-stu-id="0595d-113">String</span></span>|<span data-ttu-id="0595d-114">Определенного поставщика (продуктов и услуг - не поставщика организации); Например WindowsDefenderATP.</span><span class="sxs-lookup"><span data-stu-id="0595d-114">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="0595d-115">providerVersion</span><span class="sxs-lookup"><span data-stu-id="0595d-115">providerVersion</span></span>|<span data-ttu-id="0595d-116">Строка</span><span class="sxs-lookup"><span data-stu-id="0595d-116">String</span></span>|<span data-ttu-id="0595d-117">Версия поставщика или subprovider, если он существует, создавшее оповещение.</span><span class="sxs-lookup"><span data-stu-id="0595d-117">Version of the provider or subprovider, if it exists, that generated the alert.</span></span> <span data-ttu-id="0595d-118">*Required*</span><span class="sxs-lookup"><span data-stu-id="0595d-118">*Required*</span></span>|
|<span data-ttu-id="0595d-119">subProvider</span><span class="sxs-lookup"><span data-stu-id="0595d-119">subProvider</span></span>|<span data-ttu-id="0595d-120">Строка</span><span class="sxs-lookup"><span data-stu-id="0595d-120">String</span></span>|<span data-ttu-id="0595d-121">Определенные subprovider (в разделе статистической обработки поставщика); Например WindowsDefenderATP.SmartScreen.</span><span class="sxs-lookup"><span data-stu-id="0595d-121">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="0595d-122">поставщика</span><span class="sxs-lookup"><span data-stu-id="0595d-122">vendor</span></span> |<span data-ttu-id="0595d-123">Строка</span><span class="sxs-lookup"><span data-stu-id="0595d-123">String</span></span>|<span data-ttu-id="0595d-124">Имя оповещения поставщика (например, Microsoft, Dell, FireEye).</span><span class="sxs-lookup"><span data-stu-id="0595d-124">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span> <span data-ttu-id="0595d-125">*Required*</span><span class="sxs-lookup"><span data-stu-id="0595d-125">*Required*</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0595d-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0595d-126">JSON representation</span></span>

<span data-ttu-id="0595d-127">Соответствовать является представлением JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="0595d-127">The folllowing is a JSON representation of the resource.</span></span>
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
