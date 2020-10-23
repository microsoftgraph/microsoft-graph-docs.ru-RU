---
title: Тип ресурса Впнондемандруле
description: Определение правила VPN по запросу.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8429cb0a7870cb1ee756f5e2c02b218d5c768862
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728351"
---
# <a name="vpnondemandrule-resource-type"></a><span data-ttu-id="476a3-103">Тип ресурса Впнондемандруле</span><span class="sxs-lookup"><span data-stu-id="476a3-103">vpnOnDemandRule resource type</span></span>

<span data-ttu-id="476a3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="476a3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="476a3-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="476a3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="476a3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="476a3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="476a3-107">Определение правила VPN по запросу.</span><span class="sxs-lookup"><span data-stu-id="476a3-107">VPN On-Demand Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="476a3-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="476a3-108">Properties</span></span>
|<span data-ttu-id="476a3-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="476a3-109">Property</span></span>|<span data-ttu-id="476a3-110">Тип</span><span class="sxs-lookup"><span data-stu-id="476a3-110">Type</span></span>|<span data-ttu-id="476a3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="476a3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="476a3-112">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="476a3-112">ssids</span></span>|<span data-ttu-id="476a3-113">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="476a3-113">String collection</span></span>|<span data-ttu-id="476a3-114">Идентификаторы набора сетевых служб (SSID).</span><span class="sxs-lookup"><span data-stu-id="476a3-114">Network Service Set Identifiers (SSIDs).</span></span>|
|<span data-ttu-id="476a3-115">днссеарчдомаинс</span><span class="sxs-lookup"><span data-stu-id="476a3-115">dnsSearchDomains</span></span>|<span data-ttu-id="476a3-116">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="476a3-116">String collection</span></span>|<span data-ttu-id="476a3-117">Домены поиска DNS.</span><span class="sxs-lookup"><span data-stu-id="476a3-117">DNS Search Domains.</span></span>|
|<span data-ttu-id="476a3-118">пробеурл</span><span class="sxs-lookup"><span data-stu-id="476a3-118">probeUrl</span></span>|<span data-ttu-id="476a3-119">Строка</span><span class="sxs-lookup"><span data-stu-id="476a3-119">String</span></span>|<span data-ttu-id="476a3-120">URL-адрес для зонда.</span><span class="sxs-lookup"><span data-stu-id="476a3-120">A URL to probe.</span></span> <span data-ttu-id="476a3-121">Если этот URL-адрес успешно извлекается (возвращается код состояния HTTP 200) без перенаправления, это правило соответствует этому правилу.</span><span class="sxs-lookup"><span data-stu-id="476a3-121">If this URL is successfully fetched (returning a 200 HTTP status code) without redirection, this rule matches.</span></span>|
|<span data-ttu-id="476a3-122">action</span><span class="sxs-lookup"><span data-stu-id="476a3-122">action</span></span>|[<span data-ttu-id="476a3-123">впнондемандрулеконнектионактион</span><span class="sxs-lookup"><span data-stu-id="476a3-123">vpnOnDemandRuleConnectionAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectionaction.md)|<span data-ttu-id="476a3-124">Меры.</span><span class="sxs-lookup"><span data-stu-id="476a3-124">Action.</span></span> <span data-ttu-id="476a3-125">Возможные значения: `connect`, `evaluateConnection`, `ignore`, `disconnect`.</span><span class="sxs-lookup"><span data-stu-id="476a3-125">Possible values are: `connect`, `evaluateConnection`, `ignore`, `disconnect`.</span></span>|
|<span data-ttu-id="476a3-126">домаинактион</span><span class="sxs-lookup"><span data-stu-id="476a3-126">domainAction</span></span>|[<span data-ttu-id="476a3-127">впнондемандрулеконнектиондомаинактион</span><span class="sxs-lookup"><span data-stu-id="476a3-127">vpnOnDemandRuleConnectionDomainAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectiondomainaction.md)|<span data-ttu-id="476a3-128">Действие домена (применяется только при оценке подключения).</span><span class="sxs-lookup"><span data-stu-id="476a3-128">Domain Action (Only applicable when Action is evaluate connection).</span></span> <span data-ttu-id="476a3-129">Возможные значения: `connectIfNeeded`, `neverConnect`.</span><span class="sxs-lookup"><span data-stu-id="476a3-129">Possible values are: `connectIfNeeded`, `neverConnect`.</span></span>|
|<span data-ttu-id="476a3-130">домена</span><span class="sxs-lookup"><span data-stu-id="476a3-130">domains</span></span>|<span data-ttu-id="476a3-131">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="476a3-131">String collection</span></span>|<span data-ttu-id="476a3-132">Домены (применяется только при оценке подключения).</span><span class="sxs-lookup"><span data-stu-id="476a3-132">Domains (Only applicable when Action is evaluate connection).</span></span>|
|<span data-ttu-id="476a3-133">проберекуиредурл</span><span class="sxs-lookup"><span data-stu-id="476a3-133">probeRequiredUrl</span></span>|<span data-ttu-id="476a3-134">Строка</span><span class="sxs-lookup"><span data-stu-id="476a3-134">String</span></span>|<span data-ttu-id="476a3-135">Обязательный URL-адрес для зонда (применяется только при оценке действия Connection и при необходимости Домаинактион подключается).</span><span class="sxs-lookup"><span data-stu-id="476a3-135">Probe Required Url (Only applicable when Action is evaluate connection and DomainAction is connect if needed).</span></span>|

## <a name="relationships"></a><span data-ttu-id="476a3-136">Связи</span><span class="sxs-lookup"><span data-stu-id="476a3-136">Relationships</span></span>
<span data-ttu-id="476a3-137">Нет</span><span class="sxs-lookup"><span data-stu-id="476a3-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="476a3-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="476a3-138">JSON Representation</span></span>
<span data-ttu-id="476a3-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="476a3-139">Here is a JSON representation of the resource.</span></span>
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





