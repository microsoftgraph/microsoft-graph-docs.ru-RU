---
title: Тип ресурса cloudAppSecurityState
description: Содержит информацию о состояниях об облачных приложений (destinationServiceName, destinationServiceIp).
ms.openlocfilehash: 915044c3084e3d9a9435d602ecc7ec809d2168f2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079236"
---
# <a name="cloudappsecuritystate-resource-type"></a><span data-ttu-id="3b9e2-103">Тип ресурса cloudAppSecurityState</span><span class="sxs-lookup"><span data-stu-id="3b9e2-103">cloudAppSecurityState resource type</span></span>

<span data-ttu-id="3b9e2-104">Содержит информацию о состояниях об облачных приложений (destinationServiceName, destinationServiceIp).</span><span class="sxs-lookup"><span data-stu-id="3b9e2-104">Contains stateful information about the cloud application (destinationServiceName, destinationServiceIp).</span></span>

## <a name="properties"></a><span data-ttu-id="3b9e2-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="3b9e2-105">Properties</span></span>

| <span data-ttu-id="3b9e2-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="3b9e2-106">Property</span></span>     | <span data-ttu-id="3b9e2-107">Тип</span><span class="sxs-lookup"><span data-stu-id="3b9e2-107">Type</span></span>        | <span data-ttu-id="3b9e2-108">Description</span><span class="sxs-lookup"><span data-stu-id="3b9e2-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3b9e2-109">destinationServiceIp</span><span class="sxs-lookup"><span data-stu-id="3b9e2-109">destinationServiceIp</span></span>|<span data-ttu-id="3b9e2-110">String</span><span class="sxs-lookup"><span data-stu-id="3b9e2-110">String</span></span>|<span data-ttu-id="3b9e2-111">Конечный IP-адрес подключения для облачных приложений и служб.</span><span class="sxs-lookup"><span data-stu-id="3b9e2-111">Destination IP Address of the connection to the cloud application/service.</span></span>|
|<span data-ttu-id="3b9e2-112">destinationServiceName</span><span class="sxs-lookup"><span data-stu-id="3b9e2-112">destinationServiceName</span></span>|<span data-ttu-id="3b9e2-113">String</span><span class="sxs-lookup"><span data-stu-id="3b9e2-113">String</span></span>|<span data-ttu-id="3b9e2-114">Имя облачных приложений и служб (например «Salesforce», «Общего банка данных», и т.д.).</span><span class="sxs-lookup"><span data-stu-id="3b9e2-114">Cloud application/service name (for example "Salesforce", "DropBox", etc.).</span></span>|
|<span data-ttu-id="3b9e2-115">riskScore</span><span class="sxs-lookup"><span data-stu-id="3b9e2-115">riskScore</span></span>|<span data-ttu-id="3b9e2-116">String</span><span class="sxs-lookup"><span data-stu-id="3b9e2-116">String</span></span>|<span data-ttu-id="3b9e2-117">Оценка риска поставщика создается/вычисляемые из облачных приложений и служб.</span><span class="sxs-lookup"><span data-stu-id="3b9e2-117">Provider-generated/calculated risk score of the Cloud Application/Service.</span></span> <span data-ttu-id="3b9e2-118">Рекомендуемое значение диапазона 0-1, который соответствует в процентах.</span><span class="sxs-lookup"><span data-stu-id="3b9e2-118">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3b9e2-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3b9e2-119">JSON representation</span></span>

<span data-ttu-id="3b9e2-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3b9e2-120">The following is a JSON representation of the resource.</span></span>

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