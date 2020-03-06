---
title: Тип ресурса Хостсекуритистате
description: Содержит сведения о состоянии узла (включая устройства, компьютеры и т. д.).
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 8993e9ac301bc1cc0ae4da4ec66cc131a3e06c18
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531349"
---
# <a name="hostsecuritystate-resource-type"></a><span data-ttu-id="5333c-103">Тип ресурса Хостсекуритистате</span><span class="sxs-lookup"><span data-stu-id="5333c-103">hostSecurityState resource type</span></span>

<span data-ttu-id="5333c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5333c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5333c-105">Содержит сведения о состоянии узла (включая устройства, компьютеры и т. д.).</span><span class="sxs-lookup"><span data-stu-id="5333c-105">Contains stateful information about the host (including devices, computers, and so on).</span></span>

## <a name="properties"></a><span data-ttu-id="5333c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="5333c-106">Properties</span></span>

| <span data-ttu-id="5333c-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="5333c-107">Property</span></span>   | <span data-ttu-id="5333c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="5333c-108">Type</span></span>|<span data-ttu-id="5333c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5333c-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5333c-110">полным</span><span class="sxs-lookup"><span data-stu-id="5333c-110">fqdn</span></span>|<span data-ttu-id="5333c-111">Строка</span><span class="sxs-lookup"><span data-stu-id="5333c-111">String</span></span>|<span data-ttu-id="5333c-112">ПОЛНОЕ доменное имя узла (полное доменное имя) ( `machine.company.com`например,).</span><span class="sxs-lookup"><span data-stu-id="5333c-112">Host FQDN (Fully Qualified Domain Name) (for example, `machine.company.com`).</span></span>|
|<span data-ttu-id="5333c-113">исазуреааджоинед</span><span class="sxs-lookup"><span data-stu-id="5333c-113">isAzureAadJoined</span></span>|<span data-ttu-id="5333c-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="5333c-114">Boolean</span></span>|<span data-ttu-id="5333c-115">True, если узел подключен к доменным службам Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5333c-115">True if the host is domain joined to Azure Active Directory Domain Services.</span></span>|
|<span data-ttu-id="5333c-116">исазуреаадрегистеред</span><span class="sxs-lookup"><span data-stu-id="5333c-116">isAzureAadRegistered</span></span>|<span data-ttu-id="5333c-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="5333c-117">Boolean</span></span>|<span data-ttu-id="5333c-118">True, если узел зарегистрирован с регистрацией устройств Azure Active Directory (BYOD Devices — то есть, не полностью управляется предприятием).</span><span class="sxs-lookup"><span data-stu-id="5333c-118">True if the host registered with Azure Active Directory Device Registration (BYOD devices - that is, not fully managed by enterprise).</span></span>|
|<span data-ttu-id="5333c-119">ишибридазуредомаинжоинед</span><span class="sxs-lookup"><span data-stu-id="5333c-119">isHybridAzureDomainJoined</span></span>|<span data-ttu-id="5333c-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="5333c-120">Boolean</span></span>|<span data-ttu-id="5333c-121">True, если узел является доменом, присоединенным к локальному домену Active Directory.</span><span class="sxs-lookup"><span data-stu-id="5333c-121">True if the host is domain joined to an on-premises Active Directory domain.</span></span>|
|<span data-ttu-id="5333c-122">нетбиоснаме</span><span class="sxs-lookup"><span data-stu-id="5333c-122">netBiosName</span></span>|<span data-ttu-id="5333c-123">Строка</span><span class="sxs-lookup"><span data-stu-id="5333c-123">String</span></span>|<span data-ttu-id="5333c-124">Имя локального узла без DNS-имени домена.</span><span class="sxs-lookup"><span data-stu-id="5333c-124">The local host name, without the DNS domain name.</span></span>|
|<span data-ttu-id="5333c-125">совместим</span><span class="sxs-lookup"><span data-stu-id="5333c-125">os</span></span>|<span data-ttu-id="5333c-126">Строка</span><span class="sxs-lookup"><span data-stu-id="5333c-126">String</span></span>|<span data-ttu-id="5333c-127">Хост операционной системы.</span><span class="sxs-lookup"><span data-stu-id="5333c-127">Host Operating System.</span></span> <span data-ttu-id="5333c-128">(Например, Windows10, MacOS, РХЕЛ и т. д.).</span><span class="sxs-lookup"><span data-stu-id="5333c-128">(For example, Windows10, MacOS, RHEL, etc.).</span></span>|
|<span data-ttu-id="5333c-129">приватеипаддресс</span><span class="sxs-lookup"><span data-stu-id="5333c-129">privateIpAddress</span></span>|<span data-ttu-id="5333c-130">Строка</span><span class="sxs-lookup"><span data-stu-id="5333c-130">String</span></span>|<span data-ttu-id="5333c-131">Частный (без маршрутизации) IPv4-или IPv6-адрес (см. [RFC 1918](https://tools.ietf.org/html/rfc1918)) на момент оповещения.</span><span class="sxs-lookup"><span data-stu-id="5333c-131">Private (not routable) IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at the time of the alert.</span></span>|
|<span data-ttu-id="5333c-132">публиЦипаддресс</span><span class="sxs-lookup"><span data-stu-id="5333c-132">publicIpAddress</span></span>|<span data-ttu-id="5333c-133">Строка</span><span class="sxs-lookup"><span data-stu-id="5333c-133">String</span></span>|<span data-ttu-id="5333c-134">IPv4-или IPv6-адрес общедоступной маршрутизации (см. [RFC 1918](https://tools.ietf.org/html/rfc1918)) во время оповещения.</span><span class="sxs-lookup"><span data-stu-id="5333c-134">Publicly routable IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at time of the alert.</span></span>|
|<span data-ttu-id="5333c-135">riskScore</span><span class="sxs-lookup"><span data-stu-id="5333c-135">riskScore</span></span>|<span data-ttu-id="5333c-136">Строка</span><span class="sxs-lookup"><span data-stu-id="5333c-136">String</span></span>|<span data-ttu-id="5333c-137">Полученный поставщиком и вычисляемый показатель риска для узла.</span><span class="sxs-lookup"><span data-stu-id="5333c-137">Provider-generated/calculated risk score of the host.</span></span>  <span data-ttu-id="5333c-138">Рекомендуемый диапазон значений 0-1, указывающий на процентное соотношение.</span><span class="sxs-lookup"><span data-stu-id="5333c-138">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5333c-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5333c-139">JSON representation</span></span>

<span data-ttu-id="5333c-140">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5333c-140">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.hostSecurityState"
}-->

```json
{
  "fqdn": "String",
  "isAzureAadJoined": true,
  "isAzureAadRegistered": true,
  "isHybridAzureDomainJoined": true,
  "netBiosName": "String",
  "os": "String",
  "privateIpAddress": "String",
  "publicIpAddress": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "hostSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
