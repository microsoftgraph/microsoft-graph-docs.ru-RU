---
title: Тип ресурса cloudAppSecurityState
description: Содержит информацию о состояниях об облачных приложений (destinationServiceName, destinationServiceIp).
localization_priority: Normal
ms.openlocfilehash: ff76adf1d3879c3dac3f19ae122d82c9523d5193
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850871"
---
# <a name="cloudappsecuritystate-resource-type"></a><span data-ttu-id="bb59c-103">Тип ресурса cloudAppSecurityState</span><span class="sxs-lookup"><span data-stu-id="bb59c-103">cloudAppSecurityState resource type</span></span>

<span data-ttu-id="bb59c-104">Содержит информацию о состояниях об облачных приложений (destinationServiceName, destinationServiceIp).</span><span class="sxs-lookup"><span data-stu-id="bb59c-104">Contains stateful information about the cloud application (destinationServiceName, destinationServiceIp).</span></span>

## <a name="properties"></a><span data-ttu-id="bb59c-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="bb59c-105">Properties</span></span>

| <span data-ttu-id="bb59c-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="bb59c-106">Property</span></span>     | <span data-ttu-id="bb59c-107">Тип</span><span class="sxs-lookup"><span data-stu-id="bb59c-107">Type</span></span>        | <span data-ttu-id="bb59c-108">Описание</span><span class="sxs-lookup"><span data-stu-id="bb59c-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bb59c-109">destinationServiceIp</span><span class="sxs-lookup"><span data-stu-id="bb59c-109">destinationServiceIp</span></span>|<span data-ttu-id="bb59c-110">Строка</span><span class="sxs-lookup"><span data-stu-id="bb59c-110">String</span></span>|<span data-ttu-id="bb59c-111">Конечный IP-адрес подключения для облачных приложений и служб.</span><span class="sxs-lookup"><span data-stu-id="bb59c-111">Destination IP Address of the connection to the cloud application/service.</span></span>|
|<span data-ttu-id="bb59c-112">destinationServiceName</span><span class="sxs-lookup"><span data-stu-id="bb59c-112">destinationServiceName</span></span>|<span data-ttu-id="bb59c-113">Строка</span><span class="sxs-lookup"><span data-stu-id="bb59c-113">String</span></span>|<span data-ttu-id="bb59c-114">Имя облачных приложений и служб (например «Salesforce», «Общего банка данных», и т.д.).</span><span class="sxs-lookup"><span data-stu-id="bb59c-114">Cloud application/service name (for example "Salesforce", "DropBox", etc.).</span></span>|
|<span data-ttu-id="bb59c-115">riskScore</span><span class="sxs-lookup"><span data-stu-id="bb59c-115">riskScore</span></span>|<span data-ttu-id="bb59c-116">Строка</span><span class="sxs-lookup"><span data-stu-id="bb59c-116">String</span></span>|<span data-ttu-id="bb59c-117">Оценка риска поставщика создается/вычисляемые из облачных приложений и служб.</span><span class="sxs-lookup"><span data-stu-id="bb59c-117">Provider-generated/calculated risk score of the Cloud Application/Service.</span></span> <span data-ttu-id="bb59c-118">Рекомендуемое значение диапазона 0-1, который соответствует в процентах.</span><span class="sxs-lookup"><span data-stu-id="bb59c-118">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bb59c-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bb59c-119">JSON representation</span></span>

<span data-ttu-id="bb59c-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bb59c-120">The following is a JSON representation of the resource.</span></span>

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
