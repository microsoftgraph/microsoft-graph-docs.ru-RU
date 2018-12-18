---
title: Тип ресурса vpnOnDemandRule
description: Определение правила по запросу VPN.
author: tfitzmac
ms.openlocfilehash: 72b85971dc9c613026bb9e720ca55165845e0c9e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352194"
---
# <a name="vpnondemandrule-resource-type"></a><span data-ttu-id="5594c-103">Тип ресурса vpnOnDemandRule</span><span class="sxs-lookup"><span data-stu-id="5594c-103">vpnOnDemandRule resource type</span></span>

> <span data-ttu-id="5594c-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5594c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5594c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5594c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5594c-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5594c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5594c-107">Определение правила по запросу VPN.</span><span class="sxs-lookup"><span data-stu-id="5594c-107">VPN On-Demand Rule definition.</span></span>
## <a name="properties"></a><span data-ttu-id="5594c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="5594c-108">Properties</span></span>
|<span data-ttu-id="5594c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="5594c-109">Property</span></span>|<span data-ttu-id="5594c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="5594c-110">Type</span></span>|<span data-ttu-id="5594c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5594c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5594c-112">идентификаторов SSID</span><span class="sxs-lookup"><span data-stu-id="5594c-112">ssids</span></span>|<span data-ttu-id="5594c-113">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5594c-113">String collection</span></span>|<span data-ttu-id="5594c-114">Сетевая служба задайте идентификаторов SSID.</span><span class="sxs-lookup"><span data-stu-id="5594c-114">Network Service Set Identifiers (SSIDs).</span></span>|
|<span data-ttu-id="5594c-115">dnsSearchDomains</span><span class="sxs-lookup"><span data-stu-id="5594c-115">dnsSearchDomains</span></span>|<span data-ttu-id="5594c-116">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5594c-116">String collection</span></span>|<span data-ttu-id="5594c-117">Домены поиска DNS.</span><span class="sxs-lookup"><span data-stu-id="5594c-117">DNS Search Domains.</span></span>|
|<span data-ttu-id="5594c-118">probeUrl</span><span class="sxs-lookup"><span data-stu-id="5594c-118">probeUrl</span></span>|<span data-ttu-id="5594c-119">String.</span><span class="sxs-lookup"><span data-stu-id="5594c-119">String</span></span>|<span data-ttu-id="5594c-120">URL-адрес для поиска.</span><span class="sxs-lookup"><span data-stu-id="5594c-120">A URL to probe.</span></span> <span data-ttu-id="5594c-121">Если этот URL-адрес был успешно извлечь (возврат 200 код состояния HTTP) без в режиме одобрения администратором, соответствует данное правило.</span><span class="sxs-lookup"><span data-stu-id="5594c-121">If this URL is successfully fetched (returning a 200 HTTP status code) without redirection, this rule matches.</span></span>|
|<span data-ttu-id="5594c-122">action</span><span class="sxs-lookup"><span data-stu-id="5594c-122">action</span></span>|[<span data-ttu-id="5594c-123">vpnOnDemandRuleConnectionAction</span><span class="sxs-lookup"><span data-stu-id="5594c-123">vpnOnDemandRuleConnectionAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectionaction.md)|<span data-ttu-id="5594c-124">Действие.</span><span class="sxs-lookup"><span data-stu-id="5594c-124">Action.</span></span> <span data-ttu-id="5594c-125">Возможные значения: `connect`, `evaluateConnection`, `ignore`, `disconnect`.</span><span class="sxs-lookup"><span data-stu-id="5594c-125">Possible values are: `connect`, `evaluateConnection`, `ignore`, `disconnect`.</span></span>|
|<span data-ttu-id="5594c-126">domainAction</span><span class="sxs-lookup"><span data-stu-id="5594c-126">domainAction</span></span>|[<span data-ttu-id="5594c-127">vpnOnDemandRuleConnectionDomainAction</span><span class="sxs-lookup"><span data-stu-id="5594c-127">vpnOnDemandRuleConnectionDomainAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectiondomainaction.md)|<span data-ttu-id="5594c-128">Действие домена (возможно, только когда действие оценка подключения).</span><span class="sxs-lookup"><span data-stu-id="5594c-128">Domain Action (Only applicable when Action is evaluate connection).</span></span> <span data-ttu-id="5594c-129">Возможные значения: `connectIfNeeded`, `neverConnect`.</span><span class="sxs-lookup"><span data-stu-id="5594c-129">Possible values are: `connectIfNeeded`, `neverConnect`.</span></span>|
|<span data-ttu-id="5594c-130">домены</span><span class="sxs-lookup"><span data-stu-id="5594c-130">domains</span></span>|<span data-ttu-id="5594c-131">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="5594c-131">String collection</span></span>|<span data-ttu-id="5594c-132">Домены (возможно, только когда действие оценка подключения).</span><span class="sxs-lookup"><span data-stu-id="5594c-132">Domains (Only applicable when Action is evaluate connection).</span></span>|
|<span data-ttu-id="5594c-133">probeRequiredUrl</span><span class="sxs-lookup"><span data-stu-id="5594c-133">probeRequiredUrl</span></span>|<span data-ttu-id="5594c-134">String.</span><span class="sxs-lookup"><span data-stu-id="5594c-134">String</span></span>|<span data-ttu-id="5594c-135">Поиск необходимых URL-адреса (возможно, только если действие оценка подключения и DomainAction — это подключение при необходимости).</span><span class="sxs-lookup"><span data-stu-id="5594c-135">Probe Required Url (Only applicable when Action is evaluate connection and DomainAction is connect if needed).</span></span>|

## <a name="relationships"></a><span data-ttu-id="5594c-136">Связи</span><span class="sxs-lookup"><span data-stu-id="5594c-136">Relationships</span></span>
<span data-ttu-id="5594c-137">Нет</span><span class="sxs-lookup"><span data-stu-id="5594c-137">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5594c-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5594c-138">JSON Representation</span></span>
<span data-ttu-id="5594c-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5594c-139">Here is a JSON representation of the resource.</span></span>
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





