---
title: Тип ресурса securityVendorInformation
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
ms.openlocfilehash: 4016e274a82ad6a28101dbf5b053124b439a3cbf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080568"
---
# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="0be6c-104">Тип ресурса securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="0be6c-104">securityVendorInformation resource type</span></span>

 > <span data-ttu-id="0be6c-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0be6c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0be6c-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0be6c-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0be6c-107">Содержит сведения о безопасности продуктов и услуг поставщика, поставщик и subprovider (например, поставщика = корпорации Майкрософт; поставщика = ATP Защитник Windows; subProvider = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="0be6c-107">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="0be6c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0be6c-108">Properties</span></span>

| <span data-ttu-id="0be6c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0be6c-109">Property</span></span>   | <span data-ttu-id="0be6c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0be6c-110">Type</span></span>|<span data-ttu-id="0be6c-111">Description</span><span class="sxs-lookup"><span data-stu-id="0be6c-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0be6c-112">Поставщик</span><span class="sxs-lookup"><span data-stu-id="0be6c-112">provider</span></span> |<span data-ttu-id="0be6c-113">String</span><span class="sxs-lookup"><span data-stu-id="0be6c-113">String</span></span>|<span data-ttu-id="0be6c-114">Определенного поставщика (продуктов и услуг - не поставщика организации); Например WindowsDefenderATP.</span><span class="sxs-lookup"><span data-stu-id="0be6c-114">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="0be6c-115">providerVersion</span><span class="sxs-lookup"><span data-stu-id="0be6c-115">providerVersion</span></span>|<span data-ttu-id="0be6c-116">String</span><span class="sxs-lookup"><span data-stu-id="0be6c-116">String</span></span>|<span data-ttu-id="0be6c-117">Версия поставщика или subprovider, если он существует, создавшее оповещение.</span><span class="sxs-lookup"><span data-stu-id="0be6c-117">Version of the provider or subprovider, if it exists, that generated the alert.</span></span> <span data-ttu-id="0be6c-118">*Required*</span><span class="sxs-lookup"><span data-stu-id="0be6c-118">*Required*</span></span>|
|<span data-ttu-id="0be6c-119">subProvider</span><span class="sxs-lookup"><span data-stu-id="0be6c-119">subProvider</span></span>|<span data-ttu-id="0be6c-120">String</span><span class="sxs-lookup"><span data-stu-id="0be6c-120">String</span></span>|<span data-ttu-id="0be6c-121">Определенные subprovider (в разделе статистической обработки поставщика); Например WindowsDefenderATP.SmartScreen.</span><span class="sxs-lookup"><span data-stu-id="0be6c-121">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="0be6c-122">поставщика</span><span class="sxs-lookup"><span data-stu-id="0be6c-122">vendor</span></span> |<span data-ttu-id="0be6c-123">String</span><span class="sxs-lookup"><span data-stu-id="0be6c-123">String</span></span>|<span data-ttu-id="0be6c-124">Имя оповещения поставщика (например, Microsoft, Dell, FireEye).</span><span class="sxs-lookup"><span data-stu-id="0be6c-124">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span> <span data-ttu-id="0be6c-125">*Required*</span><span class="sxs-lookup"><span data-stu-id="0be6c-125">*Required*</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0be6c-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0be6c-126">JSON representation</span></span>

<span data-ttu-id="0be6c-127">Соответствовать является представлением JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="0be6c-127">The folllowing is a JSON representation of the resource.</span></span>
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
