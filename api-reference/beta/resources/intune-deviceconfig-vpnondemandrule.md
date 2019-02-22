---
title: Тип ресурса Впнондемандруле
description: Определение правила VPN по запросу.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b1bccd015e45291b344e7c77df4ac5c0a0af07d0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161588"
---
# <a name="vpnondemandrule-resource-type"></a><span data-ttu-id="b03a6-103">Тип ресурса Впнондемандруле</span><span class="sxs-lookup"><span data-stu-id="b03a6-103">vpnOnDemandRule resource type</span></span>

> <span data-ttu-id="b03a6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b03a6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b03a6-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b03a6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b03a6-106">Определение правила VPN по запросу.</span><span class="sxs-lookup"><span data-stu-id="b03a6-106">VPN On-Demand Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="b03a6-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b03a6-107">Properties</span></span>
|<span data-ttu-id="b03a6-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b03a6-108">Property</span></span>|<span data-ttu-id="b03a6-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b03a6-109">Type</span></span>|<span data-ttu-id="b03a6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b03a6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b03a6-111">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="b03a6-111">ssids</span></span>|<span data-ttu-id="b03a6-112">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b03a6-112">String collection</span></span>|<span data-ttu-id="b03a6-113">Идентификаторы набора сетевых служб (SSID).</span><span class="sxs-lookup"><span data-stu-id="b03a6-113">Network Service Set Identifiers (SSIDs).</span></span>|
|<span data-ttu-id="b03a6-114">Днссеарчдомаинс</span><span class="sxs-lookup"><span data-stu-id="b03a6-114">dnsSearchDomains</span></span>|<span data-ttu-id="b03a6-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b03a6-115">String collection</span></span>|<span data-ttu-id="b03a6-116">Домены поиска DNS.</span><span class="sxs-lookup"><span data-stu-id="b03a6-116">DNS Search Domains.</span></span>|
|<span data-ttu-id="b03a6-117">Пробеурл</span><span class="sxs-lookup"><span data-stu-id="b03a6-117">probeUrl</span></span>|<span data-ttu-id="b03a6-118">String</span><span class="sxs-lookup"><span data-stu-id="b03a6-118">String</span></span>|<span data-ttu-id="b03a6-119">URL-адрес для зонда.</span><span class="sxs-lookup"><span data-stu-id="b03a6-119">A URL to probe.</span></span> <span data-ttu-id="b03a6-120">Если этот URL-адрес успешно извлекается (возвращается код состояния HTTP 200) без перенаправления, это правило соответствует этому правилу.</span><span class="sxs-lookup"><span data-stu-id="b03a6-120">If this URL is successfully fetched (returning a 200 HTTP status code) without redirection, this rule matches.</span></span>|
|<span data-ttu-id="b03a6-121">action</span><span class="sxs-lookup"><span data-stu-id="b03a6-121">action</span></span>|[<span data-ttu-id="b03a6-122">Впнондемандрулеконнектионактион</span><span class="sxs-lookup"><span data-stu-id="b03a6-122">vpnOnDemandRuleConnectionAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectionaction.md)|<span data-ttu-id="b03a6-123">Меры.</span><span class="sxs-lookup"><span data-stu-id="b03a6-123">Action.</span></span> <span data-ttu-id="b03a6-124">Возможные значения: `connect`, `evaluateConnection`, `ignore`, `disconnect`.</span><span class="sxs-lookup"><span data-stu-id="b03a6-124">Possible values are: `connect`, `evaluateConnection`, `ignore`, `disconnect`.</span></span>|
|<span data-ttu-id="b03a6-125">Домаинактион</span><span class="sxs-lookup"><span data-stu-id="b03a6-125">domainAction</span></span>|[<span data-ttu-id="b03a6-126">Впнондемандрулеконнектиондомаинактион</span><span class="sxs-lookup"><span data-stu-id="b03a6-126">vpnOnDemandRuleConnectionDomainAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectiondomainaction.md)|<span data-ttu-id="b03a6-127">Действие домена (применяется только при оценке подключения).</span><span class="sxs-lookup"><span data-stu-id="b03a6-127">Domain Action (Only applicable when Action is evaluate connection).</span></span> <span data-ttu-id="b03a6-128">Возможные значения: `connectIfNeeded`, `neverConnect`.</span><span class="sxs-lookup"><span data-stu-id="b03a6-128">Possible values are: `connectIfNeeded`, `neverConnect`.</span></span>|
|<span data-ttu-id="b03a6-129">домена</span><span class="sxs-lookup"><span data-stu-id="b03a6-129">domains</span></span>|<span data-ttu-id="b03a6-130">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b03a6-130">String collection</span></span>|<span data-ttu-id="b03a6-131">Домены (применяется только при оценке подключения).</span><span class="sxs-lookup"><span data-stu-id="b03a6-131">Domains (Only applicable when Action is evaluate connection).</span></span>|
|<span data-ttu-id="b03a6-132">Проберекуиредурл</span><span class="sxs-lookup"><span data-stu-id="b03a6-132">probeRequiredUrl</span></span>|<span data-ttu-id="b03a6-133">String</span><span class="sxs-lookup"><span data-stu-id="b03a6-133">String</span></span>|<span data-ttu-id="b03a6-134">Обязательный URL-адрес для зонда (применяется только при оценке действия Connection и при необходимости Домаинактион подключается).</span><span class="sxs-lookup"><span data-stu-id="b03a6-134">Probe Required Url (Only applicable when Action is evaluate connection and DomainAction is connect if needed).</span></span>|

## <a name="relationships"></a><span data-ttu-id="b03a6-135">Отношения</span><span class="sxs-lookup"><span data-stu-id="b03a6-135">Relationships</span></span>
<span data-ttu-id="b03a6-136">Нет</span><span class="sxs-lookup"><span data-stu-id="b03a6-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b03a6-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b03a6-137">JSON Representation</span></span>
<span data-ttu-id="b03a6-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b03a6-138">Here is a JSON representation of the resource.</span></span>
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




