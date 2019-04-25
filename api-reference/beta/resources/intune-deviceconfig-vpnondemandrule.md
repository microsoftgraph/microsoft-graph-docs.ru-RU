---
title: Тип ресурса Впнондемандруле
description: Определение правила VPN по запросу.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3209c91400b36adba772273cfa6768049adce448
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561931"
---
# <a name="vpnondemandrule-resource-type"></a><span data-ttu-id="6b1fc-103">Тип ресурса Впнондемандруле</span><span class="sxs-lookup"><span data-stu-id="6b1fc-103">vpnOnDemandRule resource type</span></span>

> <span data-ttu-id="6b1fc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b1fc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b1fc-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6b1fc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b1fc-106">Определение правила VPN по запросу.</span><span class="sxs-lookup"><span data-stu-id="6b1fc-106">VPN On-Demand Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="6b1fc-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6b1fc-107">Properties</span></span>
|<span data-ttu-id="6b1fc-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6b1fc-108">Property</span></span>|<span data-ttu-id="6b1fc-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6b1fc-109">Type</span></span>|<span data-ttu-id="6b1fc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6b1fc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b1fc-111">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="6b1fc-111">ssids</span></span>|<span data-ttu-id="6b1fc-112">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6b1fc-112">String collection</span></span>|<span data-ttu-id="6b1fc-113">Идентификаторы набора сетевых служб (SSID).</span><span class="sxs-lookup"><span data-stu-id="6b1fc-113">Network Service Set Identifiers (SSIDs).</span></span>|
|<span data-ttu-id="6b1fc-114">Днссеарчдомаинс</span><span class="sxs-lookup"><span data-stu-id="6b1fc-114">dnsSearchDomains</span></span>|<span data-ttu-id="6b1fc-115">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6b1fc-115">String collection</span></span>|<span data-ttu-id="6b1fc-116">Домены поиска DNS.</span><span class="sxs-lookup"><span data-stu-id="6b1fc-116">DNS Search Domains.</span></span>|
|<span data-ttu-id="6b1fc-117">Пробеурл</span><span class="sxs-lookup"><span data-stu-id="6b1fc-117">probeUrl</span></span>|<span data-ttu-id="6b1fc-118">String</span><span class="sxs-lookup"><span data-stu-id="6b1fc-118">String</span></span>|<span data-ttu-id="6b1fc-119">URL-адрес для зонда.</span><span class="sxs-lookup"><span data-stu-id="6b1fc-119">A URL to probe.</span></span> <span data-ttu-id="6b1fc-120">Если этот URL-адрес успешно извлекается (возвращается код состояния HTTP 200) без перенаправления, это правило соответствует этому правилу.</span><span class="sxs-lookup"><span data-stu-id="6b1fc-120">If this URL is successfully fetched (returning a 200 HTTP status code) without redirection, this rule matches.</span></span>|
|<span data-ttu-id="6b1fc-121">action</span><span class="sxs-lookup"><span data-stu-id="6b1fc-121">action</span></span>|[<span data-ttu-id="6b1fc-122">Впнондемандрулеконнектионактион</span><span class="sxs-lookup"><span data-stu-id="6b1fc-122">vpnOnDemandRuleConnectionAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectionaction.md)|<span data-ttu-id="6b1fc-123">Меры.</span><span class="sxs-lookup"><span data-stu-id="6b1fc-123">Action.</span></span> <span data-ttu-id="6b1fc-124">Возможные значения: `connect`, `evaluateConnection`, `ignore`, `disconnect`.</span><span class="sxs-lookup"><span data-stu-id="6b1fc-124">Possible values are: `connect`, `evaluateConnection`, `ignore`, `disconnect`.</span></span>|
|<span data-ttu-id="6b1fc-125">Домаинактион</span><span class="sxs-lookup"><span data-stu-id="6b1fc-125">domainAction</span></span>|[<span data-ttu-id="6b1fc-126">Впнондемандрулеконнектиондомаинактион</span><span class="sxs-lookup"><span data-stu-id="6b1fc-126">vpnOnDemandRuleConnectionDomainAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectiondomainaction.md)|<span data-ttu-id="6b1fc-127">Действие домена (применяется только при оценке подключения).</span><span class="sxs-lookup"><span data-stu-id="6b1fc-127">Domain Action (Only applicable when Action is evaluate connection).</span></span> <span data-ttu-id="6b1fc-128">Возможные значения: `connectIfNeeded`, `neverConnect`.</span><span class="sxs-lookup"><span data-stu-id="6b1fc-128">Possible values are: `connectIfNeeded`, `neverConnect`.</span></span>|
|<span data-ttu-id="6b1fc-129">домена</span><span class="sxs-lookup"><span data-stu-id="6b1fc-129">domains</span></span>|<span data-ttu-id="6b1fc-130">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="6b1fc-130">String collection</span></span>|<span data-ttu-id="6b1fc-131">Домены (применяется только при оценке подключения).</span><span class="sxs-lookup"><span data-stu-id="6b1fc-131">Domains (Only applicable when Action is evaluate connection).</span></span>|
|<span data-ttu-id="6b1fc-132">Проберекуиредурл</span><span class="sxs-lookup"><span data-stu-id="6b1fc-132">probeRequiredUrl</span></span>|<span data-ttu-id="6b1fc-133">String</span><span class="sxs-lookup"><span data-stu-id="6b1fc-133">String</span></span>|<span data-ttu-id="6b1fc-134">Обязательный URL-адрес для зонда (применяется только при оценке действия Connection и при необходимости Домаинактион подключается).</span><span class="sxs-lookup"><span data-stu-id="6b1fc-134">Probe Required Url (Only applicable when Action is evaluate connection and DomainAction is connect if needed).</span></span>|

## <a name="relationships"></a><span data-ttu-id="6b1fc-135">Отношения</span><span class="sxs-lookup"><span data-stu-id="6b1fc-135">Relationships</span></span>
<span data-ttu-id="6b1fc-136">Нет</span><span class="sxs-lookup"><span data-stu-id="6b1fc-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6b1fc-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6b1fc-137">JSON Representation</span></span>
<span data-ttu-id="6b1fc-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6b1fc-138">Here is a JSON representation of the resource.</span></span>
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





