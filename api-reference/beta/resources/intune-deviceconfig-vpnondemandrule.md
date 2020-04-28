---
title: Тип ресурса Впнондемандруле
description: Определение правила VPN по запросу.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dd5724e4c2c1cfb5ca185dd8420011853812305a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43412149"
---
# <a name="vpnondemandrule-resource-type"></a><span data-ttu-id="2e53b-103">Тип ресурса Впнондемандруле</span><span class="sxs-lookup"><span data-stu-id="2e53b-103">vpnOnDemandRule resource type</span></span>

<span data-ttu-id="2e53b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e53b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2e53b-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2e53b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2e53b-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2e53b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e53b-107">Определение правила VPN по запросу.</span><span class="sxs-lookup"><span data-stu-id="2e53b-107">VPN On-Demand Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="2e53b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="2e53b-108">Properties</span></span>
|<span data-ttu-id="2e53b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="2e53b-109">Property</span></span>|<span data-ttu-id="2e53b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="2e53b-110">Type</span></span>|<span data-ttu-id="2e53b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2e53b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e53b-112">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="2e53b-112">ssids</span></span>|<span data-ttu-id="2e53b-113">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="2e53b-113">String collection</span></span>|<span data-ttu-id="2e53b-114">Идентификаторы набора сетевых служб (SSID).</span><span class="sxs-lookup"><span data-stu-id="2e53b-114">Network Service Set Identifiers (SSIDs).</span></span>|
|<span data-ttu-id="2e53b-115">днссеарчдомаинс</span><span class="sxs-lookup"><span data-stu-id="2e53b-115">dnsSearchDomains</span></span>|<span data-ttu-id="2e53b-116">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="2e53b-116">String collection</span></span>|<span data-ttu-id="2e53b-117">Домены поиска DNS.</span><span class="sxs-lookup"><span data-stu-id="2e53b-117">DNS Search Domains.</span></span>|
|<span data-ttu-id="2e53b-118">пробеурл</span><span class="sxs-lookup"><span data-stu-id="2e53b-118">probeUrl</span></span>|<span data-ttu-id="2e53b-119">String</span><span class="sxs-lookup"><span data-stu-id="2e53b-119">String</span></span>|<span data-ttu-id="2e53b-120">URL-адрес для зонда.</span><span class="sxs-lookup"><span data-stu-id="2e53b-120">A URL to probe.</span></span> <span data-ttu-id="2e53b-121">Если этот URL-адрес успешно извлекается (возвращается код состояния HTTP 200) без перенаправления, это правило соответствует этому правилу.</span><span class="sxs-lookup"><span data-stu-id="2e53b-121">If this URL is successfully fetched (returning a 200 HTTP status code) without redirection, this rule matches.</span></span>|
|<span data-ttu-id="2e53b-122">action</span><span class="sxs-lookup"><span data-stu-id="2e53b-122">action</span></span>|[<span data-ttu-id="2e53b-123">впнондемандрулеконнектионактион</span><span class="sxs-lookup"><span data-stu-id="2e53b-123">vpnOnDemandRuleConnectionAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectionaction.md)|<span data-ttu-id="2e53b-124">Меры.</span><span class="sxs-lookup"><span data-stu-id="2e53b-124">Action.</span></span> <span data-ttu-id="2e53b-125">Возможные значения: `connect`, `evaluateConnection`, `ignore`, `disconnect`.</span><span class="sxs-lookup"><span data-stu-id="2e53b-125">Possible values are: `connect`, `evaluateConnection`, `ignore`, `disconnect`.</span></span>|
|<span data-ttu-id="2e53b-126">домаинактион</span><span class="sxs-lookup"><span data-stu-id="2e53b-126">domainAction</span></span>|[<span data-ttu-id="2e53b-127">впнондемандрулеконнектиондомаинактион</span><span class="sxs-lookup"><span data-stu-id="2e53b-127">vpnOnDemandRuleConnectionDomainAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectiondomainaction.md)|<span data-ttu-id="2e53b-128">Действие домена (применяется только при оценке подключения).</span><span class="sxs-lookup"><span data-stu-id="2e53b-128">Domain Action (Only applicable when Action is evaluate connection).</span></span> <span data-ttu-id="2e53b-129">Возможные значения: `connectIfNeeded`, `neverConnect`.</span><span class="sxs-lookup"><span data-stu-id="2e53b-129">Possible values are: `connectIfNeeded`, `neverConnect`.</span></span>|
|<span data-ttu-id="2e53b-130">домена</span><span class="sxs-lookup"><span data-stu-id="2e53b-130">domains</span></span>|<span data-ttu-id="2e53b-131">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="2e53b-131">String collection</span></span>|<span data-ttu-id="2e53b-132">Домены (применяется только при оценке подключения).</span><span class="sxs-lookup"><span data-stu-id="2e53b-132">Domains (Only applicable when Action is evaluate connection).</span></span>|
|<span data-ttu-id="2e53b-133">проберекуиредурл</span><span class="sxs-lookup"><span data-stu-id="2e53b-133">probeRequiredUrl</span></span>|<span data-ttu-id="2e53b-134">String</span><span class="sxs-lookup"><span data-stu-id="2e53b-134">String</span></span>|<span data-ttu-id="2e53b-135">Обязательный URL-адрес для зонда (применяется только при оценке действия Connection и при необходимости Домаинактион подключается).</span><span class="sxs-lookup"><span data-stu-id="2e53b-135">Probe Required Url (Only applicable when Action is evaluate connection and DomainAction is connect if needed).</span></span>|

## <a name="relationships"></a><span data-ttu-id="2e53b-136">Связи</span><span class="sxs-lookup"><span data-stu-id="2e53b-136">Relationships</span></span>
<span data-ttu-id="2e53b-137">Нет</span><span class="sxs-lookup"><span data-stu-id="2e53b-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2e53b-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2e53b-138">JSON Representation</span></span>
<span data-ttu-id="2e53b-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2e53b-139">Here is a JSON representation of the resource.</span></span>
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



