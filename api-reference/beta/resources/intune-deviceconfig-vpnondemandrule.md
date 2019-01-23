---
title: Тип ресурса vpnOnDemandRule
description: Определение правила по запросу VPN.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8164d1c12aeb172120bb9803d7f3dd98366ec948
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421461"
---
# <a name="vpnondemandrule-resource-type"></a><span data-ttu-id="a004e-103">Тип ресурса vpnOnDemandRule</span><span class="sxs-lookup"><span data-stu-id="a004e-103">vpnOnDemandRule resource type</span></span>

> <span data-ttu-id="a004e-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a004e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a004e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a004e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a004e-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a004e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a004e-107">Определение правила по запросу VPN.</span><span class="sxs-lookup"><span data-stu-id="a004e-107">VPN On-Demand Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="a004e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a004e-108">Properties</span></span>
|<span data-ttu-id="a004e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a004e-109">Property</span></span>|<span data-ttu-id="a004e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a004e-110">Type</span></span>|<span data-ttu-id="a004e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a004e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a004e-112">идентификаторов SSID</span><span class="sxs-lookup"><span data-stu-id="a004e-112">ssids</span></span>|<span data-ttu-id="a004e-113">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a004e-113">String collection</span></span>|<span data-ttu-id="a004e-114">Сетевая служба задайте идентификаторов SSID.</span><span class="sxs-lookup"><span data-stu-id="a004e-114">Network Service Set Identifiers (SSIDs).</span></span>|
|<span data-ttu-id="a004e-115">dnsSearchDomains</span><span class="sxs-lookup"><span data-stu-id="a004e-115">dnsSearchDomains</span></span>|<span data-ttu-id="a004e-116">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a004e-116">String collection</span></span>|<span data-ttu-id="a004e-117">Домены поиска DNS.</span><span class="sxs-lookup"><span data-stu-id="a004e-117">DNS Search Domains.</span></span>|
|<span data-ttu-id="a004e-118">probeUrl</span><span class="sxs-lookup"><span data-stu-id="a004e-118">probeUrl</span></span>|<span data-ttu-id="a004e-119">String</span><span class="sxs-lookup"><span data-stu-id="a004e-119">String</span></span>|<span data-ttu-id="a004e-120">URL-адрес для поиска.</span><span class="sxs-lookup"><span data-stu-id="a004e-120">A URL to probe.</span></span> <span data-ttu-id="a004e-121">Если этот URL-адрес был успешно извлечь (возврат 200 код состояния HTTP) без в режиме одобрения администратором, соответствует данное правило.</span><span class="sxs-lookup"><span data-stu-id="a004e-121">If this URL is successfully fetched (returning a 200 HTTP status code) without redirection, this rule matches.</span></span>|
|<span data-ttu-id="a004e-122">action</span><span class="sxs-lookup"><span data-stu-id="a004e-122">action</span></span>|[<span data-ttu-id="a004e-123">vpnOnDemandRuleConnectionAction</span><span class="sxs-lookup"><span data-stu-id="a004e-123">vpnOnDemandRuleConnectionAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectionaction.md)|<span data-ttu-id="a004e-124">Действие.</span><span class="sxs-lookup"><span data-stu-id="a004e-124">Action.</span></span> <span data-ttu-id="a004e-125">Возможные значения: `connect`, `evaluateConnection`, `ignore`, `disconnect`.</span><span class="sxs-lookup"><span data-stu-id="a004e-125">Possible values are: `connect`, `evaluateConnection`, `ignore`, `disconnect`.</span></span>|
|<span data-ttu-id="a004e-126">domainAction</span><span class="sxs-lookup"><span data-stu-id="a004e-126">domainAction</span></span>|[<span data-ttu-id="a004e-127">vpnOnDemandRuleConnectionDomainAction</span><span class="sxs-lookup"><span data-stu-id="a004e-127">vpnOnDemandRuleConnectionDomainAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectiondomainaction.md)|<span data-ttu-id="a004e-128">Действие домена (возможно, только когда действие оценка подключения).</span><span class="sxs-lookup"><span data-stu-id="a004e-128">Domain Action (Only applicable when Action is evaluate connection).</span></span> <span data-ttu-id="a004e-129">Возможные значения: `connectIfNeeded`, `neverConnect`.</span><span class="sxs-lookup"><span data-stu-id="a004e-129">Possible values are: `connectIfNeeded`, `neverConnect`.</span></span>|
|<span data-ttu-id="a004e-130">домены</span><span class="sxs-lookup"><span data-stu-id="a004e-130">domains</span></span>|<span data-ttu-id="a004e-131">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a004e-131">String collection</span></span>|<span data-ttu-id="a004e-132">Домены (возможно, только когда действие оценка подключения).</span><span class="sxs-lookup"><span data-stu-id="a004e-132">Domains (Only applicable when Action is evaluate connection).</span></span>|
|<span data-ttu-id="a004e-133">probeRequiredUrl</span><span class="sxs-lookup"><span data-stu-id="a004e-133">probeRequiredUrl</span></span>|<span data-ttu-id="a004e-134">String</span><span class="sxs-lookup"><span data-stu-id="a004e-134">String</span></span>|<span data-ttu-id="a004e-135">Поиск необходимых URL-адреса (возможно, только если действие оценка подключения и DomainAction — это подключение при необходимости).</span><span class="sxs-lookup"><span data-stu-id="a004e-135">Probe Required Url (Only applicable when Action is evaluate connection and DomainAction is connect if needed).</span></span>|

## <a name="relationships"></a><span data-ttu-id="a004e-136">Отношения</span><span class="sxs-lookup"><span data-stu-id="a004e-136">Relationships</span></span>
<span data-ttu-id="a004e-137">Нет</span><span class="sxs-lookup"><span data-stu-id="a004e-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a004e-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a004e-138">JSON Representation</span></span>
<span data-ttu-id="a004e-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a004e-139">Here is a JSON representation of the resource.</span></span>
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




