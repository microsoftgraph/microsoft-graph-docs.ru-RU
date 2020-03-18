---
title: Тип ресурса Впнондемандруле
description: Определение правила VPN по запросу.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cb1274dd966553ecde0514e0603619b6ed803c77
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42787364"
---
# <a name="vpnondemandrule-resource-type"></a><span data-ttu-id="a3893-103">Тип ресурса Впнондемандруле</span><span class="sxs-lookup"><span data-stu-id="a3893-103">vpnOnDemandRule resource type</span></span>

> <span data-ttu-id="a3893-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a3893-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3893-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a3893-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3893-106">Определение правила VPN по запросу.</span><span class="sxs-lookup"><span data-stu-id="a3893-106">VPN On-Demand Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="a3893-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a3893-107">Properties</span></span>
|<span data-ttu-id="a3893-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a3893-108">Property</span></span>|<span data-ttu-id="a3893-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a3893-109">Type</span></span>|<span data-ttu-id="a3893-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a3893-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3893-111">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="a3893-111">ssids</span></span>|<span data-ttu-id="a3893-112">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a3893-112">String collection</span></span>|<span data-ttu-id="a3893-113">Идентификаторы набора сетевых служб (SSID).</span><span class="sxs-lookup"><span data-stu-id="a3893-113">Network Service Set Identifiers (SSIDs).</span></span>|
|<span data-ttu-id="a3893-114">днссеарчдомаинс</span><span class="sxs-lookup"><span data-stu-id="a3893-114">dnsSearchDomains</span></span>|<span data-ttu-id="a3893-115">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a3893-115">String collection</span></span>|<span data-ttu-id="a3893-116">Домены поиска DNS.</span><span class="sxs-lookup"><span data-stu-id="a3893-116">DNS Search Domains.</span></span>|
|<span data-ttu-id="a3893-117">пробеурл</span><span class="sxs-lookup"><span data-stu-id="a3893-117">probeUrl</span></span>|<span data-ttu-id="a3893-118">String</span><span class="sxs-lookup"><span data-stu-id="a3893-118">String</span></span>|<span data-ttu-id="a3893-119">URL-адрес для зонда.</span><span class="sxs-lookup"><span data-stu-id="a3893-119">A URL to probe.</span></span> <span data-ttu-id="a3893-120">Если этот URL-адрес успешно извлекается (возвращается код состояния HTTP 200) без перенаправления, это правило соответствует этому правилу.</span><span class="sxs-lookup"><span data-stu-id="a3893-120">If this URL is successfully fetched (returning a 200 HTTP status code) without redirection, this rule matches.</span></span>|
|<span data-ttu-id="a3893-121">action</span><span class="sxs-lookup"><span data-stu-id="a3893-121">action</span></span>|[<span data-ttu-id="a3893-122">впнондемандрулеконнектионактион</span><span class="sxs-lookup"><span data-stu-id="a3893-122">vpnOnDemandRuleConnectionAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectionaction.md)|<span data-ttu-id="a3893-123">Меры.</span><span class="sxs-lookup"><span data-stu-id="a3893-123">Action.</span></span> <span data-ttu-id="a3893-124">Возможные значения: `connect`, `evaluateConnection`, `ignore`, `disconnect`.</span><span class="sxs-lookup"><span data-stu-id="a3893-124">Possible values are: `connect`, `evaluateConnection`, `ignore`, `disconnect`.</span></span>|
|<span data-ttu-id="a3893-125">домаинактион</span><span class="sxs-lookup"><span data-stu-id="a3893-125">domainAction</span></span>|[<span data-ttu-id="a3893-126">впнондемандрулеконнектиондомаинактион</span><span class="sxs-lookup"><span data-stu-id="a3893-126">vpnOnDemandRuleConnectionDomainAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectiondomainaction.md)|<span data-ttu-id="a3893-127">Действие домена (применяется только при оценке подключения).</span><span class="sxs-lookup"><span data-stu-id="a3893-127">Domain Action (Only applicable when Action is evaluate connection).</span></span> <span data-ttu-id="a3893-128">Возможные значения: `connectIfNeeded`, `neverConnect`.</span><span class="sxs-lookup"><span data-stu-id="a3893-128">Possible values are: `connectIfNeeded`, `neverConnect`.</span></span>|
|<span data-ttu-id="a3893-129">домена</span><span class="sxs-lookup"><span data-stu-id="a3893-129">domains</span></span>|<span data-ttu-id="a3893-130">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a3893-130">String collection</span></span>|<span data-ttu-id="a3893-131">Домены (применяется только при оценке подключения).</span><span class="sxs-lookup"><span data-stu-id="a3893-131">Domains (Only applicable when Action is evaluate connection).</span></span>|
|<span data-ttu-id="a3893-132">проберекуиредурл</span><span class="sxs-lookup"><span data-stu-id="a3893-132">probeRequiredUrl</span></span>|<span data-ttu-id="a3893-133">String</span><span class="sxs-lookup"><span data-stu-id="a3893-133">String</span></span>|<span data-ttu-id="a3893-134">Обязательный URL-адрес для зонда (применяется только при оценке действия Connection и при необходимости Домаинактион подключается).</span><span class="sxs-lookup"><span data-stu-id="a3893-134">Probe Required Url (Only applicable when Action is evaluate connection and DomainAction is connect if needed).</span></span>|

## <a name="relationships"></a><span data-ttu-id="a3893-135">Связи</span><span class="sxs-lookup"><span data-stu-id="a3893-135">Relationships</span></span>
<span data-ttu-id="a3893-136">Нет</span><span class="sxs-lookup"><span data-stu-id="a3893-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a3893-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a3893-137">JSON Representation</span></span>
<span data-ttu-id="a3893-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a3893-138">Here is a JSON representation of the resource.</span></span>
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



