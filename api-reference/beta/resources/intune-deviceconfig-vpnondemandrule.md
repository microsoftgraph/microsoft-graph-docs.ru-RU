---
title: Тип ресурса Впнондемандруле
description: Определение правила VPN по запросу.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c75a8b725c95449868767ce6a08a43876c16ab62
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525770"
---
# <a name="vpnondemandrule-resource-type"></a><span data-ttu-id="527aa-103">Тип ресурса Впнондемандруле</span><span class="sxs-lookup"><span data-stu-id="527aa-103">vpnOnDemandRule resource type</span></span>

<span data-ttu-id="527aa-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="527aa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="527aa-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="527aa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="527aa-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="527aa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="527aa-107">Определение правила VPN по запросу.</span><span class="sxs-lookup"><span data-stu-id="527aa-107">VPN On-Demand Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="527aa-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="527aa-108">Properties</span></span>
|<span data-ttu-id="527aa-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="527aa-109">Property</span></span>|<span data-ttu-id="527aa-110">Тип</span><span class="sxs-lookup"><span data-stu-id="527aa-110">Type</span></span>|<span data-ttu-id="527aa-111">Описание</span><span class="sxs-lookup"><span data-stu-id="527aa-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="527aa-112">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="527aa-112">ssids</span></span>|<span data-ttu-id="527aa-113">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="527aa-113">String collection</span></span>|<span data-ttu-id="527aa-114">Идентификаторы набора сетевых служб (SSID).</span><span class="sxs-lookup"><span data-stu-id="527aa-114">Network Service Set Identifiers (SSIDs).</span></span>|
|<span data-ttu-id="527aa-115">днссеарчдомаинс</span><span class="sxs-lookup"><span data-stu-id="527aa-115">dnsSearchDomains</span></span>|<span data-ttu-id="527aa-116">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="527aa-116">String collection</span></span>|<span data-ttu-id="527aa-117">Домены поиска DNS.</span><span class="sxs-lookup"><span data-stu-id="527aa-117">DNS Search Domains.</span></span>|
|<span data-ttu-id="527aa-118">пробеурл</span><span class="sxs-lookup"><span data-stu-id="527aa-118">probeUrl</span></span>|<span data-ttu-id="527aa-119">String</span><span class="sxs-lookup"><span data-stu-id="527aa-119">String</span></span>|<span data-ttu-id="527aa-120">URL-адрес для зонда.</span><span class="sxs-lookup"><span data-stu-id="527aa-120">A URL to probe.</span></span> <span data-ttu-id="527aa-121">Если этот URL-адрес успешно извлекается (возвращается код состояния HTTP 200) без перенаправления, это правило соответствует этому правилу.</span><span class="sxs-lookup"><span data-stu-id="527aa-121">If this URL is successfully fetched (returning a 200 HTTP status code) without redirection, this rule matches.</span></span>|
|<span data-ttu-id="527aa-122">action</span><span class="sxs-lookup"><span data-stu-id="527aa-122">action</span></span>|[<span data-ttu-id="527aa-123">впнондемандрулеконнектионактион</span><span class="sxs-lookup"><span data-stu-id="527aa-123">vpnOnDemandRuleConnectionAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectionaction.md)|<span data-ttu-id="527aa-124">Меры.</span><span class="sxs-lookup"><span data-stu-id="527aa-124">Action.</span></span> <span data-ttu-id="527aa-125">Возможные значения: `connect`, `evaluateConnection`, `ignore`, `disconnect`.</span><span class="sxs-lookup"><span data-stu-id="527aa-125">Possible values are: `connect`, `evaluateConnection`, `ignore`, `disconnect`.</span></span>|
|<span data-ttu-id="527aa-126">домаинактион</span><span class="sxs-lookup"><span data-stu-id="527aa-126">domainAction</span></span>|[<span data-ttu-id="527aa-127">впнондемандрулеконнектиондомаинактион</span><span class="sxs-lookup"><span data-stu-id="527aa-127">vpnOnDemandRuleConnectionDomainAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectiondomainaction.md)|<span data-ttu-id="527aa-128">Действие домена (применяется только при оценке подключения).</span><span class="sxs-lookup"><span data-stu-id="527aa-128">Domain Action (Only applicable when Action is evaluate connection).</span></span> <span data-ttu-id="527aa-129">Возможные значения: `connectIfNeeded`, `neverConnect`.</span><span class="sxs-lookup"><span data-stu-id="527aa-129">Possible values are: `connectIfNeeded`, `neverConnect`.</span></span>|
|<span data-ttu-id="527aa-130">домена</span><span class="sxs-lookup"><span data-stu-id="527aa-130">domains</span></span>|<span data-ttu-id="527aa-131">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="527aa-131">String collection</span></span>|<span data-ttu-id="527aa-132">Домены (применяется только при оценке подключения).</span><span class="sxs-lookup"><span data-stu-id="527aa-132">Domains (Only applicable when Action is evaluate connection).</span></span>|
|<span data-ttu-id="527aa-133">проберекуиредурл</span><span class="sxs-lookup"><span data-stu-id="527aa-133">probeRequiredUrl</span></span>|<span data-ttu-id="527aa-134">String</span><span class="sxs-lookup"><span data-stu-id="527aa-134">String</span></span>|<span data-ttu-id="527aa-135">Обязательный URL-адрес для зонда (применяется только при оценке действия Connection и при необходимости Домаинактион подключается).</span><span class="sxs-lookup"><span data-stu-id="527aa-135">Probe Required Url (Only applicable when Action is evaluate connection and DomainAction is connect if needed).</span></span>|

## <a name="relationships"></a><span data-ttu-id="527aa-136">Связи</span><span class="sxs-lookup"><span data-stu-id="527aa-136">Relationships</span></span>
<span data-ttu-id="527aa-137">Нет</span><span class="sxs-lookup"><span data-stu-id="527aa-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="527aa-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="527aa-138">JSON Representation</span></span>
<span data-ttu-id="527aa-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="527aa-139">Here is a JSON representation of the resource.</span></span>
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



