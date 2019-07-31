---
title: Тип ресурса Клаудаппсекуритистате
description: Содержит сведения о состоянии облачного приложения (Дестинатионсервиценаме, Дестинатионсервицеип).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 515c567c2360d0d37ddcba6c805f6723312b8030
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012928"
---
# <a name="cloudappsecuritystate-resource-type"></a><span data-ttu-id="e3355-103">Тип ресурса Клаудаппсекуритистате</span><span class="sxs-lookup"><span data-stu-id="e3355-103">cloudAppSecurityState resource type</span></span>

<span data-ttu-id="e3355-104">Содержит сведения о состоянии облачного приложения (Дестинатионсервиценаме, Дестинатионсервицеип).</span><span class="sxs-lookup"><span data-stu-id="e3355-104">Contains stateful information about the cloud application (destinationServiceName, destinationServiceIp).</span></span>

## <a name="properties"></a><span data-ttu-id="e3355-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="e3355-105">Properties</span></span>

| <span data-ttu-id="e3355-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="e3355-106">Property</span></span>     | <span data-ttu-id="e3355-107">Тип</span><span class="sxs-lookup"><span data-stu-id="e3355-107">Type</span></span>        | <span data-ttu-id="e3355-108">Описание</span><span class="sxs-lookup"><span data-stu-id="e3355-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e3355-109">Дестинатионсервицеип</span><span class="sxs-lookup"><span data-stu-id="e3355-109">destinationServiceIp</span></span>|<span data-ttu-id="e3355-110">String</span><span class="sxs-lookup"><span data-stu-id="e3355-110">String</span></span>|<span data-ttu-id="e3355-111">Конечный IP-адрес подключения к облачному приложению или службе.</span><span class="sxs-lookup"><span data-stu-id="e3355-111">Destination IP Address of the connection to the cloud application/service.</span></span>|
|<span data-ttu-id="e3355-112">Дестинатионсервиценаме</span><span class="sxs-lookup"><span data-stu-id="e3355-112">destinationServiceName</span></span>|<span data-ttu-id="e3355-113">String</span><span class="sxs-lookup"><span data-stu-id="e3355-113">String</span></span>|<span data-ttu-id="e3355-114">Имя облачного приложения или службы (например, "Salesforce", "DropBox" и т. д.).</span><span class="sxs-lookup"><span data-stu-id="e3355-114">Cloud application/service name (for example "Salesforce", "DropBox", etc.).</span></span>|
|<span data-ttu-id="e3355-115">riskScore</span><span class="sxs-lookup"><span data-stu-id="e3355-115">riskScore</span></span>|<span data-ttu-id="e3355-116">String</span><span class="sxs-lookup"><span data-stu-id="e3355-116">String</span></span>|<span data-ttu-id="e3355-117">Полученный поставщиком и вычисляемый показатель риска облачного приложения или службы.</span><span class="sxs-lookup"><span data-stu-id="e3355-117">Provider-generated/calculated risk score of the Cloud Application/Service.</span></span> <span data-ttu-id="e3355-118">Рекомендуемый диапазон значений 0-1, указывающий на процентное соотношение.</span><span class="sxs-lookup"><span data-stu-id="e3355-118">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e3355-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e3355-119">JSON representation</span></span>

<span data-ttu-id="e3355-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e3355-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.cloudAppSecurityState"
}-->

```json
{
  "destinationServiceIp": "String",
  "destinationServiceName": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "cloudAppSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
