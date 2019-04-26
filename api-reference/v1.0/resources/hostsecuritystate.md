---
title: Тип ресурса Хостсекуритистате
description: Содержит сведения о состоянии узла (включая устройства, компьютеры и т. д.).
localization_priority: Normal
ms.openlocfilehash: 0646547b7f3e31dcf283c1ce423a52b4ae16f013
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570787"
---
# <a name="hostsecuritystate-resource-type"></a><span data-ttu-id="a179d-103">Тип ресурса Хостсекуритистате</span><span class="sxs-lookup"><span data-stu-id="a179d-103">hostSecurityState resource type</span></span>

<span data-ttu-id="a179d-104">Содержит сведения о состоянии узла (включая устройства, компьютеры и т. д.).</span><span class="sxs-lookup"><span data-stu-id="a179d-104">Contains stateful information about the host (including devices, computers, and so on).</span></span>

## <a name="properties"></a><span data-ttu-id="a179d-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="a179d-105">Properties</span></span>

| <span data-ttu-id="a179d-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="a179d-106">Property</span></span>   | <span data-ttu-id="a179d-107">Тип</span><span class="sxs-lookup"><span data-stu-id="a179d-107">Type</span></span>|<span data-ttu-id="a179d-108">Описание</span><span class="sxs-lookup"><span data-stu-id="a179d-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a179d-109">полным</span><span class="sxs-lookup"><span data-stu-id="a179d-109">fqdn</span></span>|<span data-ttu-id="a179d-110">String</span><span class="sxs-lookup"><span data-stu-id="a179d-110">String</span></span>|<span data-ttu-id="a179d-111">ПОЛНОЕ доменное имя узла (полное доменное имя) ( `machine.company.com`например,).</span><span class="sxs-lookup"><span data-stu-id="a179d-111">Host FQDN (Fully Qualified Domain Name) (for example, `machine.company.com`).</span></span>|
|<span data-ttu-id="a179d-112">Исазуреааджоинед</span><span class="sxs-lookup"><span data-stu-id="a179d-112">isAzureAadJoined</span></span>|<span data-ttu-id="a179d-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="a179d-113">Boolean</span></span>|<span data-ttu-id="a179d-114">True, если узел подключен к доменным службам Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a179d-114">True if the host is domain joined to Azure Active Directory Domain Services.</span></span>|
|<span data-ttu-id="a179d-115">Исазуреаадрегистеред</span><span class="sxs-lookup"><span data-stu-id="a179d-115">isAzureAadRegistered</span></span>|<span data-ttu-id="a179d-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="a179d-116">Boolean</span></span>|<span data-ttu-id="a179d-117">True, если узел зарегистрирован с регистрацией устройств Azure Active Directory (BYOD Devices — то есть, не полностью управляется предприятием).</span><span class="sxs-lookup"><span data-stu-id="a179d-117">True if the host registered with Azure Active Directory Device Registration (BYOD devices - that is, not fully managed by enterprise).</span></span>|
|<span data-ttu-id="a179d-118">Ишибридазуредомаинжоинед</span><span class="sxs-lookup"><span data-stu-id="a179d-118">isHybridAzureDomainJoined</span></span>|<span data-ttu-id="a179d-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="a179d-119">Boolean</span></span>|<span data-ttu-id="a179d-120">True, если узел является доменом, присоединенным к локальному домену Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a179d-120">True if the host is domain joined to an on-premises Active Directory domain.</span></span>|
|<span data-ttu-id="a179d-121">Нетбиоснаме</span><span class="sxs-lookup"><span data-stu-id="a179d-121">netBiosName</span></span>|<span data-ttu-id="a179d-122">String</span><span class="sxs-lookup"><span data-stu-id="a179d-122">String</span></span>|<span data-ttu-id="a179d-123">Имя локального узла без DNS-имени домена.</span><span class="sxs-lookup"><span data-stu-id="a179d-123">The local host name, without the DNS domain name.</span></span>|
|<span data-ttu-id="a179d-124">совместим</span><span class="sxs-lookup"><span data-stu-id="a179d-124">os</span></span>|<span data-ttu-id="a179d-125">String</span><span class="sxs-lookup"><span data-stu-id="a179d-125">String</span></span>|<span data-ttu-id="a179d-126">Хост операционной системы.</span><span class="sxs-lookup"><span data-stu-id="a179d-126">Host Operating System.</span></span> <span data-ttu-id="a179d-127">(Например, Windows10, MacOS, РХЕЛ и т. д.).</span><span class="sxs-lookup"><span data-stu-id="a179d-127">(For example, Windows10, MacOS, RHEL, etc.).</span></span>|
|<span data-ttu-id="a179d-128">Приватеипаддресс</span><span class="sxs-lookup"><span data-stu-id="a179d-128">privateIpAddress</span></span>|<span data-ttu-id="a179d-129">String</span><span class="sxs-lookup"><span data-stu-id="a179d-129">String</span></span>|<span data-ttu-id="a179d-130">Частный (без маршрутизации) IPv4-или IPv6-адрес (см. [RFC 1918](https://tools.ietf.org/html/rfc1918)) на момент оповещения.</span><span class="sxs-lookup"><span data-stu-id="a179d-130">Private (not routable) IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at the time of the alert.</span></span>|
|<span data-ttu-id="a179d-131">ПублиЦипаддресс</span><span class="sxs-lookup"><span data-stu-id="a179d-131">publicIpAddress</span></span>|<span data-ttu-id="a179d-132">String</span><span class="sxs-lookup"><span data-stu-id="a179d-132">String</span></span>|<span data-ttu-id="a179d-133">IPv4-или IPv6-адрес общеДоступной маршрутизации (см. [RFC 1918](https://tools.ietf.org/html/rfc1918)) во время оповещения.</span><span class="sxs-lookup"><span data-stu-id="a179d-133">Publicly routable IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at time of the alert.</span></span>|
|<span data-ttu-id="a179d-134">riskScore</span><span class="sxs-lookup"><span data-stu-id="a179d-134">riskScore</span></span>|<span data-ttu-id="a179d-135">String</span><span class="sxs-lookup"><span data-stu-id="a179d-135">String</span></span>|<span data-ttu-id="a179d-136">Полученный поставщиком и вычисляемый показатель риска для узла.</span><span class="sxs-lookup"><span data-stu-id="a179d-136">Provider-generated/calculated risk score of the host.</span></span>  <span data-ttu-id="a179d-137">Рекомендуемый диапазон значений 0-1, указывающий на процентное соотношение.</span><span class="sxs-lookup"><span data-stu-id="a179d-137">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a179d-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a179d-138">JSON representation</span></span>

<span data-ttu-id="a179d-139">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a179d-139">The following is a JSON representation of the resource.</span></span>

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
