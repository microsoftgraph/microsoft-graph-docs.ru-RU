---
title: Тип ресурса Впнондемандруле
description: Определение правила VPN по запросу.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: aaa72419ce12195a042592abceb86ec754ea7341
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48049032"
---
# <a name="vpnondemandrule-resource-type"></a><span data-ttu-id="21bcb-103">Тип ресурса Впнондемандруле</span><span class="sxs-lookup"><span data-stu-id="21bcb-103">vpnOnDemandRule resource type</span></span>

<span data-ttu-id="21bcb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21bcb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="21bcb-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="21bcb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21bcb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="21bcb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21bcb-107">Определение правила VPN по запросу.</span><span class="sxs-lookup"><span data-stu-id="21bcb-107">VPN On-Demand Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="21bcb-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="21bcb-108">Properties</span></span>
|<span data-ttu-id="21bcb-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="21bcb-109">Property</span></span>|<span data-ttu-id="21bcb-110">Тип</span><span class="sxs-lookup"><span data-stu-id="21bcb-110">Type</span></span>|<span data-ttu-id="21bcb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="21bcb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21bcb-112">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="21bcb-112">ssids</span></span>|<span data-ttu-id="21bcb-113">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="21bcb-113">String collection</span></span>|<span data-ttu-id="21bcb-114">Идентификаторы набора сетевых служб (SSID).</span><span class="sxs-lookup"><span data-stu-id="21bcb-114">Network Service Set Identifiers (SSIDs).</span></span>|
|<span data-ttu-id="21bcb-115">днссеарчдомаинс</span><span class="sxs-lookup"><span data-stu-id="21bcb-115">dnsSearchDomains</span></span>|<span data-ttu-id="21bcb-116">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="21bcb-116">String collection</span></span>|<span data-ttu-id="21bcb-117">Домены поиска DNS.</span><span class="sxs-lookup"><span data-stu-id="21bcb-117">DNS Search Domains.</span></span>|
|<span data-ttu-id="21bcb-118">пробеурл</span><span class="sxs-lookup"><span data-stu-id="21bcb-118">probeUrl</span></span>|<span data-ttu-id="21bcb-119">Строка</span><span class="sxs-lookup"><span data-stu-id="21bcb-119">String</span></span>|<span data-ttu-id="21bcb-120">URL-адрес для зонда.</span><span class="sxs-lookup"><span data-stu-id="21bcb-120">A URL to probe.</span></span> <span data-ttu-id="21bcb-121">Если этот URL-адрес успешно извлекается (возвращается код состояния HTTP 200) без перенаправления, это правило соответствует этому правилу.</span><span class="sxs-lookup"><span data-stu-id="21bcb-121">If this URL is successfully fetched (returning a 200 HTTP status code) without redirection, this rule matches.</span></span>|
|<span data-ttu-id="21bcb-122">action</span><span class="sxs-lookup"><span data-stu-id="21bcb-122">action</span></span>|[<span data-ttu-id="21bcb-123">впнондемандрулеконнектионактион</span><span class="sxs-lookup"><span data-stu-id="21bcb-123">vpnOnDemandRuleConnectionAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectionaction.md)|<span data-ttu-id="21bcb-124">Меры.</span><span class="sxs-lookup"><span data-stu-id="21bcb-124">Action.</span></span> <span data-ttu-id="21bcb-125">Возможные значения: `connect`, `evaluateConnection`, `ignore`, `disconnect`.</span><span class="sxs-lookup"><span data-stu-id="21bcb-125">Possible values are: `connect`, `evaluateConnection`, `ignore`, `disconnect`.</span></span>|
|<span data-ttu-id="21bcb-126">домаинактион</span><span class="sxs-lookup"><span data-stu-id="21bcb-126">domainAction</span></span>|[<span data-ttu-id="21bcb-127">впнондемандрулеконнектиондомаинактион</span><span class="sxs-lookup"><span data-stu-id="21bcb-127">vpnOnDemandRuleConnectionDomainAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectiondomainaction.md)|<span data-ttu-id="21bcb-128">Действие домена (применяется только при оценке подключения).</span><span class="sxs-lookup"><span data-stu-id="21bcb-128">Domain Action (Only applicable when Action is evaluate connection).</span></span> <span data-ttu-id="21bcb-129">Возможные значения: `connectIfNeeded`, `neverConnect`.</span><span class="sxs-lookup"><span data-stu-id="21bcb-129">Possible values are: `connectIfNeeded`, `neverConnect`.</span></span>|
|<span data-ttu-id="21bcb-130">домена</span><span class="sxs-lookup"><span data-stu-id="21bcb-130">domains</span></span>|<span data-ttu-id="21bcb-131">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="21bcb-131">String collection</span></span>|<span data-ttu-id="21bcb-132">Домены (применяется только при оценке подключения).</span><span class="sxs-lookup"><span data-stu-id="21bcb-132">Domains (Only applicable when Action is evaluate connection).</span></span>|
|<span data-ttu-id="21bcb-133">проберекуиредурл</span><span class="sxs-lookup"><span data-stu-id="21bcb-133">probeRequiredUrl</span></span>|<span data-ttu-id="21bcb-134">Строка</span><span class="sxs-lookup"><span data-stu-id="21bcb-134">String</span></span>|<span data-ttu-id="21bcb-135">Обязательный URL-адрес для зонда (применяется только при оценке действия Connection и при необходимости Домаинактион подключается).</span><span class="sxs-lookup"><span data-stu-id="21bcb-135">Probe Required Url (Only applicable when Action is evaluate connection and DomainAction is connect if needed).</span></span>|

## <a name="relationships"></a><span data-ttu-id="21bcb-136">Отношения</span><span class="sxs-lookup"><span data-stu-id="21bcb-136">Relationships</span></span>
<span data-ttu-id="21bcb-137">Нет</span><span class="sxs-lookup"><span data-stu-id="21bcb-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="21bcb-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="21bcb-138">JSON Representation</span></span>
<span data-ttu-id="21bcb-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="21bcb-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnOnDemandRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnOnDemandRule",
  "ssids": [
    "String"
  ],
  "dnsSearchDomains": [
    "String"
  ],
  "probeUrl": "String",
  "action": "String",
  "domainAction": "String",
  "domains": [
    "String"
  ],
  "probeRequiredUrl": "String"
}
```






