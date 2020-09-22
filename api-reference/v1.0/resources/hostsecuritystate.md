---
title: Тип ресурса Хостсекуритистате
description: Содержит сведения о состоянии узла (включая устройства, компьютеры и т. д.).
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 2d8543512162398f38f9ddb74cf72f57171c58f8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48062885"
---
# <a name="hostsecuritystate-resource-type"></a><span data-ttu-id="321f6-103">Тип ресурса Хостсекуритистате</span><span class="sxs-lookup"><span data-stu-id="321f6-103">hostSecurityState resource type</span></span>

<span data-ttu-id="321f6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="321f6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="321f6-105">Содержит сведения о состоянии узла (включая устройства, компьютеры и т. д.).</span><span class="sxs-lookup"><span data-stu-id="321f6-105">Contains stateful information about the host (including devices, computers, and so on).</span></span>

## <a name="properties"></a><span data-ttu-id="321f6-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="321f6-106">Properties</span></span>

| <span data-ttu-id="321f6-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="321f6-107">Property</span></span>   | <span data-ttu-id="321f6-108">Тип</span><span class="sxs-lookup"><span data-stu-id="321f6-108">Type</span></span>|<span data-ttu-id="321f6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="321f6-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="321f6-110">полным</span><span class="sxs-lookup"><span data-stu-id="321f6-110">fqdn</span></span>|<span data-ttu-id="321f6-111">String</span><span class="sxs-lookup"><span data-stu-id="321f6-111">String</span></span>|<span data-ttu-id="321f6-112">ПОЛНОЕ доменное имя узла (полное доменное имя) (например, `machine.company.com` ).</span><span class="sxs-lookup"><span data-stu-id="321f6-112">Host FQDN (Fully Qualified Domain Name) (for example, `machine.company.com`).</span></span>|
|<span data-ttu-id="321f6-113">исазуреааджоинед</span><span class="sxs-lookup"><span data-stu-id="321f6-113">isAzureAadJoined</span></span>|<span data-ttu-id="321f6-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="321f6-114">Boolean</span></span>|<span data-ttu-id="321f6-115">True, если узел подключен к доменным службам Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="321f6-115">True if the host is domain joined to Azure Active Directory Domain Services.</span></span>|
|<span data-ttu-id="321f6-116">исазуреаадрегистеред</span><span class="sxs-lookup"><span data-stu-id="321f6-116">isAzureAadRegistered</span></span>|<span data-ttu-id="321f6-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="321f6-117">Boolean</span></span>|<span data-ttu-id="321f6-118">True, если узел зарегистрирован с регистрацией устройств Azure Active Directory (BYOD Devices — то есть, не полностью управляется предприятием).</span><span class="sxs-lookup"><span data-stu-id="321f6-118">True if the host registered with Azure Active Directory Device Registration (BYOD devices - that is, not fully managed by enterprise).</span></span>|
|<span data-ttu-id="321f6-119">ишибридазуредомаинжоинед</span><span class="sxs-lookup"><span data-stu-id="321f6-119">isHybridAzureDomainJoined</span></span>|<span data-ttu-id="321f6-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="321f6-120">Boolean</span></span>|<span data-ttu-id="321f6-121">True, если узел является доменом, присоединенным к локальному домену Active Directory.</span><span class="sxs-lookup"><span data-stu-id="321f6-121">True if the host is domain joined to an on-premises Active Directory domain.</span></span>|
|<span data-ttu-id="321f6-122">нетбиоснаме</span><span class="sxs-lookup"><span data-stu-id="321f6-122">netBiosName</span></span>|<span data-ttu-id="321f6-123">String</span><span class="sxs-lookup"><span data-stu-id="321f6-123">String</span></span>|<span data-ttu-id="321f6-124">Имя локального узла без DNS-имени домена.</span><span class="sxs-lookup"><span data-stu-id="321f6-124">The local host name, without the DNS domain name.</span></span>|
|<span data-ttu-id="321f6-125">совместим</span><span class="sxs-lookup"><span data-stu-id="321f6-125">os</span></span>|<span data-ttu-id="321f6-126">String</span><span class="sxs-lookup"><span data-stu-id="321f6-126">String</span></span>|<span data-ttu-id="321f6-127">Хост операционной системы.</span><span class="sxs-lookup"><span data-stu-id="321f6-127">Host Operating System.</span></span> <span data-ttu-id="321f6-128">(Например, Windows10, MacOS, РХЕЛ и т. д.).</span><span class="sxs-lookup"><span data-stu-id="321f6-128">(For example, Windows10, MacOS, RHEL, etc.).</span></span>|
|<span data-ttu-id="321f6-129">приватеипаддресс</span><span class="sxs-lookup"><span data-stu-id="321f6-129">privateIpAddress</span></span>|<span data-ttu-id="321f6-130">String</span><span class="sxs-lookup"><span data-stu-id="321f6-130">String</span></span>|<span data-ttu-id="321f6-131">Частный (без маршрутизации) IPv4-или IPv6-адрес (см. [RFC 1918](https://tools.ietf.org/html/rfc1918)) на момент оповещения.</span><span class="sxs-lookup"><span data-stu-id="321f6-131">Private (not routable) IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at the time of the alert.</span></span>|
|<span data-ttu-id="321f6-132">публиЦипаддресс</span><span class="sxs-lookup"><span data-stu-id="321f6-132">publicIpAddress</span></span>|<span data-ttu-id="321f6-133">String</span><span class="sxs-lookup"><span data-stu-id="321f6-133">String</span></span>|<span data-ttu-id="321f6-134">IPv4-или IPv6-адрес общедоступной маршрутизации (см. [RFC 1918](https://tools.ietf.org/html/rfc1918)) во время оповещения.</span><span class="sxs-lookup"><span data-stu-id="321f6-134">Publicly routable IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at time of the alert.</span></span>|
|<span data-ttu-id="321f6-135">riskScore</span><span class="sxs-lookup"><span data-stu-id="321f6-135">riskScore</span></span>|<span data-ttu-id="321f6-136">String</span><span class="sxs-lookup"><span data-stu-id="321f6-136">String</span></span>|<span data-ttu-id="321f6-137">Полученный поставщиком и вычисляемый показатель риска для узла.</span><span class="sxs-lookup"><span data-stu-id="321f6-137">Provider-generated/calculated risk score of the host.</span></span>  <span data-ttu-id="321f6-138">Рекомендуемый диапазон значений 0-1, указывающий на процентное соотношение.</span><span class="sxs-lookup"><span data-stu-id="321f6-138">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="321f6-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="321f6-139">JSON representation</span></span>

<span data-ttu-id="321f6-140">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="321f6-140">The following is a JSON representation of the resource.</span></span>

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

