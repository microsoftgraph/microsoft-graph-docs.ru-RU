---
title: Тип ресурса securityVendorInformation
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: e67a5306b1dd08933877dbe3e64cab766ccd6a96
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512180"
---
# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="49f14-104">Тип ресурса securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="49f14-104">securityVendorInformation resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49f14-105">Содержит сведения о безопасности продуктов и услуг поставщика, поставщик и subprovider (например, поставщика = корпорации Майкрософт; поставщика = ATP Защитник Windows; subProvider = AppLocker).</span><span class="sxs-lookup"><span data-stu-id="49f14-105">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="49f14-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="49f14-106">Properties</span></span>

| <span data-ttu-id="49f14-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="49f14-107">Property</span></span>   | <span data-ttu-id="49f14-108">Тип</span><span class="sxs-lookup"><span data-stu-id="49f14-108">Type</span></span>|<span data-ttu-id="49f14-109">Описание</span><span class="sxs-lookup"><span data-stu-id="49f14-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="49f14-110">Поставщик</span><span class="sxs-lookup"><span data-stu-id="49f14-110">provider</span></span> |<span data-ttu-id="49f14-111">String</span><span class="sxs-lookup"><span data-stu-id="49f14-111">String</span></span>|<span data-ttu-id="49f14-112">Определенного поставщика (продуктов и услуг - не поставщика организации); Например WindowsDefenderATP.</span><span class="sxs-lookup"><span data-stu-id="49f14-112">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="49f14-113">providerVersion</span><span class="sxs-lookup"><span data-stu-id="49f14-113">providerVersion</span></span>|<span data-ttu-id="49f14-114">String</span><span class="sxs-lookup"><span data-stu-id="49f14-114">String</span></span>|<span data-ttu-id="49f14-115">Версия поставщика или subprovider, если он существует, создавшее оповещение.</span><span class="sxs-lookup"><span data-stu-id="49f14-115">Version of the provider or subprovider, if it exists, that generated the alert.</span></span> <span data-ttu-id="49f14-116">*Required*</span><span class="sxs-lookup"><span data-stu-id="49f14-116">*Required*</span></span>|
|<span data-ttu-id="49f14-117">subProvider</span><span class="sxs-lookup"><span data-stu-id="49f14-117">subProvider</span></span>|<span data-ttu-id="49f14-118">String</span><span class="sxs-lookup"><span data-stu-id="49f14-118">String</span></span>|<span data-ttu-id="49f14-119">Определенные subprovider (в разделе статистической обработки поставщика); Например WindowsDefenderATP.SmartScreen.</span><span class="sxs-lookup"><span data-stu-id="49f14-119">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="49f14-120">поставщика</span><span class="sxs-lookup"><span data-stu-id="49f14-120">vendor</span></span> |<span data-ttu-id="49f14-121">String</span><span class="sxs-lookup"><span data-stu-id="49f14-121">String</span></span>|<span data-ttu-id="49f14-122">Имя оповещения поставщика (например, Microsoft, Dell, FireEye).</span><span class="sxs-lookup"><span data-stu-id="49f14-122">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span> <span data-ttu-id="49f14-123">*Required*</span><span class="sxs-lookup"><span data-stu-id="49f14-123">*Required*</span></span>|

## <a name="json-representation"></a><span data-ttu-id="49f14-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="49f14-124">JSON representation</span></span>

<span data-ttu-id="49f14-125">Соответствовать является представлением JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="49f14-125">The folllowing is a JSON representation of the resource.</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/resources/securityvendorinformation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
