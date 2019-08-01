---
title: Тип ресурса Хостсекуритистате
description: Содержит сведения о состоянии узла (включая устройства, компьютеры и т. д.).
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: dabe7d0aa026cb1b514e95fbc953dcb1974f8925
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029276"
---
# <a name="hostsecuritystate-resource-type"></a><span data-ttu-id="ec84b-103">Тип ресурса Хостсекуритистате</span><span class="sxs-lookup"><span data-stu-id="ec84b-103">hostSecurityState resource type</span></span>

<span data-ttu-id="ec84b-104">Содержит сведения о состоянии узла (включая устройства, компьютеры и т. д.).</span><span class="sxs-lookup"><span data-stu-id="ec84b-104">Contains stateful information about the host (including devices, computers, and so on).</span></span>

## <a name="properties"></a><span data-ttu-id="ec84b-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="ec84b-105">Properties</span></span>

| <span data-ttu-id="ec84b-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="ec84b-106">Property</span></span>   | <span data-ttu-id="ec84b-107">Тип</span><span class="sxs-lookup"><span data-stu-id="ec84b-107">Type</span></span>|<span data-ttu-id="ec84b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="ec84b-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ec84b-109">полным</span><span class="sxs-lookup"><span data-stu-id="ec84b-109">fqdn</span></span>|<span data-ttu-id="ec84b-110">String</span><span class="sxs-lookup"><span data-stu-id="ec84b-110">String</span></span>|<span data-ttu-id="ec84b-111">ПОЛНОЕ доменное имя узла (полное доменное имя) ( `machine.company.com`например,).</span><span class="sxs-lookup"><span data-stu-id="ec84b-111">Host FQDN (Fully Qualified Domain Name) (for example, `machine.company.com`).</span></span>|
|<span data-ttu-id="ec84b-112">Исазуреааджоинед</span><span class="sxs-lookup"><span data-stu-id="ec84b-112">isAzureAadJoined</span></span>|<span data-ttu-id="ec84b-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec84b-113">Boolean</span></span>|<span data-ttu-id="ec84b-114">True, если узел подключен к доменным службам Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ec84b-114">True if the host is domain joined to Azure Active Directory Domain Services.</span></span>|
|<span data-ttu-id="ec84b-115">Исазуреаадрегистеред</span><span class="sxs-lookup"><span data-stu-id="ec84b-115">isAzureAadRegistered</span></span>|<span data-ttu-id="ec84b-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec84b-116">Boolean</span></span>|<span data-ttu-id="ec84b-117">True, если узел зарегистрирован с регистрацией устройств Azure Active Directory (BYOD Devices — то есть, не полностью управляется предприятием).</span><span class="sxs-lookup"><span data-stu-id="ec84b-117">True if the host registered with Azure Active Directory Device Registration (BYOD devices - that is, not fully managed by enterprise).</span></span>|
|<span data-ttu-id="ec84b-118">Ишибридазуредомаинжоинед</span><span class="sxs-lookup"><span data-stu-id="ec84b-118">isHybridAzureDomainJoined</span></span>|<span data-ttu-id="ec84b-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="ec84b-119">Boolean</span></span>|<span data-ttu-id="ec84b-120">True, если узел является доменом, присоединенным к локальному домену Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ec84b-120">True if the host is domain joined to an on-premises Active Directory domain.</span></span>|
|<span data-ttu-id="ec84b-121">Нетбиоснаме</span><span class="sxs-lookup"><span data-stu-id="ec84b-121">netBiosName</span></span>|<span data-ttu-id="ec84b-122">String</span><span class="sxs-lookup"><span data-stu-id="ec84b-122">String</span></span>|<span data-ttu-id="ec84b-123">Имя локального узла без DNS-имени домена.</span><span class="sxs-lookup"><span data-stu-id="ec84b-123">The local host name, without the DNS domain name.</span></span>|
|<span data-ttu-id="ec84b-124">совместим</span><span class="sxs-lookup"><span data-stu-id="ec84b-124">os</span></span>|<span data-ttu-id="ec84b-125">String</span><span class="sxs-lookup"><span data-stu-id="ec84b-125">String</span></span>|<span data-ttu-id="ec84b-126">Хост операционной системы.</span><span class="sxs-lookup"><span data-stu-id="ec84b-126">Host Operating System.</span></span> <span data-ttu-id="ec84b-127">(Например, Windows10, MacOS, РХЕЛ и т. д.).</span><span class="sxs-lookup"><span data-stu-id="ec84b-127">(For example, Windows10, MacOS, RHEL, etc.).</span></span>|
|<span data-ttu-id="ec84b-128">Приватеипаддресс</span><span class="sxs-lookup"><span data-stu-id="ec84b-128">privateIpAddress</span></span>|<span data-ttu-id="ec84b-129">String</span><span class="sxs-lookup"><span data-stu-id="ec84b-129">String</span></span>|<span data-ttu-id="ec84b-130">Частный (без маршрутизации) IPv4-или IPv6-адрес (см. [RFC 1918](https://tools.ietf.org/html/rfc1918)) на момент оповещения.</span><span class="sxs-lookup"><span data-stu-id="ec84b-130">Private (not routable) IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at the time of the alert.</span></span>|
|<span data-ttu-id="ec84b-131">ПублиЦипаддресс</span><span class="sxs-lookup"><span data-stu-id="ec84b-131">publicIpAddress</span></span>|<span data-ttu-id="ec84b-132">String</span><span class="sxs-lookup"><span data-stu-id="ec84b-132">String</span></span>|<span data-ttu-id="ec84b-133">IPv4-или IPv6-адрес общедоступной маршрутизации (см. [RFC 1918](https://tools.ietf.org/html/rfc1918)) во время оповещения.</span><span class="sxs-lookup"><span data-stu-id="ec84b-133">Publicly routable IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at time of the alert.</span></span>|
|<span data-ttu-id="ec84b-134">riskScore</span><span class="sxs-lookup"><span data-stu-id="ec84b-134">riskScore</span></span>|<span data-ttu-id="ec84b-135">String</span><span class="sxs-lookup"><span data-stu-id="ec84b-135">String</span></span>|<span data-ttu-id="ec84b-136">Полученный поставщиком и вычисляемый показатель риска для узла.</span><span class="sxs-lookup"><span data-stu-id="ec84b-136">Provider-generated/calculated risk score of the host.</span></span>  <span data-ttu-id="ec84b-137">Рекомендуемый диапазон значений 0-1, указывающий на процентное соотношение.</span><span class="sxs-lookup"><span data-stu-id="ec84b-137">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ec84b-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ec84b-138">JSON representation</span></span>

<span data-ttu-id="ec84b-139">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ec84b-139">The following is a JSON representation of the resource.</span></span>

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
