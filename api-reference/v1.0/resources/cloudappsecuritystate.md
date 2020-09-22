---
title: Тип ресурса Клаудаппсекуритистате
description: Содержит сведения о состоянии облачного приложения (Дестинатионсервиценаме, Дестинатионсервицеип).
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 0f987f64960290c4104ed1c0746ce38591cb3ab6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48086797"
---
# <a name="cloudappsecuritystate-resource-type"></a><span data-ttu-id="16aed-103">Тип ресурса Клаудаппсекуритистате</span><span class="sxs-lookup"><span data-stu-id="16aed-103">cloudAppSecurityState resource type</span></span>

<span data-ttu-id="16aed-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16aed-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="16aed-105">Содержит сведения о состоянии облачного приложения (Дестинатионсервиценаме, Дестинатионсервицеип).</span><span class="sxs-lookup"><span data-stu-id="16aed-105">Contains stateful information about the cloud application (destinationServiceName, destinationServiceIp).</span></span>

## <a name="properties"></a><span data-ttu-id="16aed-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="16aed-106">Properties</span></span>

| <span data-ttu-id="16aed-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="16aed-107">Property</span></span>     | <span data-ttu-id="16aed-108">Тип</span><span class="sxs-lookup"><span data-stu-id="16aed-108">Type</span></span>        | <span data-ttu-id="16aed-109">Описание</span><span class="sxs-lookup"><span data-stu-id="16aed-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="16aed-110">дестинатионсервицеип</span><span class="sxs-lookup"><span data-stu-id="16aed-110">destinationServiceIp</span></span>|<span data-ttu-id="16aed-111">Строка</span><span class="sxs-lookup"><span data-stu-id="16aed-111">String</span></span>|<span data-ttu-id="16aed-112">Конечный IP-адрес подключения к облачному приложению или службе.</span><span class="sxs-lookup"><span data-stu-id="16aed-112">Destination IP Address of the connection to the cloud application/service.</span></span>|
|<span data-ttu-id="16aed-113">дестинатионсервиценаме</span><span class="sxs-lookup"><span data-stu-id="16aed-113">destinationServiceName</span></span>|<span data-ttu-id="16aed-114">Строка</span><span class="sxs-lookup"><span data-stu-id="16aed-114">String</span></span>|<span data-ttu-id="16aed-115">Имя облачного приложения или службы (например, "Salesforce", "DropBox" и т. д.).</span><span class="sxs-lookup"><span data-stu-id="16aed-115">Cloud application/service name (for example "Salesforce", "DropBox", etc.).</span></span>|
|<span data-ttu-id="16aed-116">riskScore</span><span class="sxs-lookup"><span data-stu-id="16aed-116">riskScore</span></span>|<span data-ttu-id="16aed-117">Строка</span><span class="sxs-lookup"><span data-stu-id="16aed-117">String</span></span>|<span data-ttu-id="16aed-118">Полученный поставщиком и вычисляемый показатель риска облачного приложения или службы.</span><span class="sxs-lookup"><span data-stu-id="16aed-118">Provider-generated/calculated risk score of the Cloud Application/Service.</span></span> <span data-ttu-id="16aed-119">Рекомендуемый диапазон значений 0-1, указывающий на процентное соотношение.</span><span class="sxs-lookup"><span data-stu-id="16aed-119">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="16aed-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="16aed-120">JSON representation</span></span>

<span data-ttu-id="16aed-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="16aed-121">The following is a JSON representation of the resource.</span></span>

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

