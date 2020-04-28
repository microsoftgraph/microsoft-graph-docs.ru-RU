---
title: Тип ресурса Хостсекуритистате
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: ec4b6ba22aceaaaeb3c612f61eb522bfe14243c6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42496868"
---
# <a name="hostsecuritystate-resource-type"></a><span data-ttu-id="6e8ea-104">Тип ресурса Хостсекуритистате</span><span class="sxs-lookup"><span data-stu-id="6e8ea-104">hostSecurityState resource type</span></span>

<span data-ttu-id="6e8ea-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e8ea-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e8ea-106">Содержит сведения о состоянии узла (включая устройства, компьютеры и т. д.).</span><span class="sxs-lookup"><span data-stu-id="6e8ea-106">Contains stateful information about the host (including devices, computers, and so on).</span></span>

## <a name="properties"></a><span data-ttu-id="6e8ea-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6e8ea-107">Properties</span></span>

| <span data-ttu-id="6e8ea-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6e8ea-108">Property</span></span>   | <span data-ttu-id="6e8ea-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6e8ea-109">Type</span></span>|<span data-ttu-id="6e8ea-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6e8ea-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6e8ea-111">полным</span><span class="sxs-lookup"><span data-stu-id="6e8ea-111">fqdn</span></span>|<span data-ttu-id="6e8ea-112">String</span><span class="sxs-lookup"><span data-stu-id="6e8ea-112">String</span></span>|<span data-ttu-id="6e8ea-113">ПОЛНОЕ доменное имя узла (полное доменное имя) (например, machine.company.com).</span><span class="sxs-lookup"><span data-stu-id="6e8ea-113">Host FQDN (Fully Qualified Domain Name) (for example, machine.company.com).</span></span>|
|<span data-ttu-id="6e8ea-114">исазуреааджоинед</span><span class="sxs-lookup"><span data-stu-id="6e8ea-114">isAzureAadJoined</span></span>|<span data-ttu-id="6e8ea-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e8ea-115">Boolean</span></span>|<span data-ttu-id="6e8ea-116">True, если узел подключен к доменным службам Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6e8ea-116">True if the host is domain joined to Azure Active Directory Domain Services.</span></span>|
|<span data-ttu-id="6e8ea-117">исазуреаадрегистеред</span><span class="sxs-lookup"><span data-stu-id="6e8ea-117">isAzureAadRegistered</span></span>|<span data-ttu-id="6e8ea-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e8ea-118">Boolean</span></span>|<span data-ttu-id="6e8ea-119">True, если узел зарегистрирован с регистрацией устройств Azure Active Directory (BYOD Devices — то есть, не полностью управляется предприятием).</span><span class="sxs-lookup"><span data-stu-id="6e8ea-119">True if the host registered with Azure Active Directory Device Registration (BYOD devices - that is, not fully managed by enterprise).</span></span>|
|<span data-ttu-id="6e8ea-120">ишибридазуредомаинжоинед</span><span class="sxs-lookup"><span data-stu-id="6e8ea-120">isHybridAzureDomainJoined</span></span>|<span data-ttu-id="6e8ea-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e8ea-121">Boolean</span></span>|<span data-ttu-id="6e8ea-122">True, если узел является доменом, присоединенным к локальному домену Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6e8ea-122">True if the host is domain joined to an on-premises Active Directory domain.</span></span>|
|<span data-ttu-id="6e8ea-123">нетбиоснаме</span><span class="sxs-lookup"><span data-stu-id="6e8ea-123">netBiosName</span></span>|<span data-ttu-id="6e8ea-124">String</span><span class="sxs-lookup"><span data-stu-id="6e8ea-124">String</span></span>|<span data-ttu-id="6e8ea-125">Имя локального узла без DNS-имени домена.</span><span class="sxs-lookup"><span data-stu-id="6e8ea-125">The local host name, without the DNS domain name.</span></span>|
|<span data-ttu-id="6e8ea-126">совместим</span><span class="sxs-lookup"><span data-stu-id="6e8ea-126">os</span></span>|<span data-ttu-id="6e8ea-127">String</span><span class="sxs-lookup"><span data-stu-id="6e8ea-127">String</span></span>|<span data-ttu-id="6e8ea-128">Хост операционной системы.</span><span class="sxs-lookup"><span data-stu-id="6e8ea-128">Host Operating System.</span></span> <span data-ttu-id="6e8ea-129">(Например, Windows10, MacOS, РХЕЛ и т. д.).</span><span class="sxs-lookup"><span data-stu-id="6e8ea-129">(For example, Windows10, MacOS, RHEL, etc.).</span></span>|
|<span data-ttu-id="6e8ea-130">приватеипаддресс</span><span class="sxs-lookup"><span data-stu-id="6e8ea-130">privateIpAddress</span></span>|<span data-ttu-id="6e8ea-131">String</span><span class="sxs-lookup"><span data-stu-id="6e8ea-131">String</span></span>|<span data-ttu-id="6e8ea-132">Частный (без маршрутизации) IPv4-или IPv6-адрес (см. [RFC 1918](https://tools.ietf.org/html/rfc1918)) на момент оповещения.</span><span class="sxs-lookup"><span data-stu-id="6e8ea-132">Private (not routable) IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at the time of the alert.</span></span>|
|<span data-ttu-id="6e8ea-133">публиЦипаддресс</span><span class="sxs-lookup"><span data-stu-id="6e8ea-133">publicIpAddress</span></span>|<span data-ttu-id="6e8ea-134">String</span><span class="sxs-lookup"><span data-stu-id="6e8ea-134">String</span></span>|<span data-ttu-id="6e8ea-135">IPv4-или IPv6-адрес общедоступной маршрутизации (см. [RFC 1918](https://tools.ietf.org/html/rfc1918)) во время оповещения.</span><span class="sxs-lookup"><span data-stu-id="6e8ea-135">Publicly routable IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at time of the alert.</span></span>|
|<span data-ttu-id="6e8ea-136">riskScore</span><span class="sxs-lookup"><span data-stu-id="6e8ea-136">riskScore</span></span>|<span data-ttu-id="6e8ea-137">String</span><span class="sxs-lookup"><span data-stu-id="6e8ea-137">String</span></span>|<span data-ttu-id="6e8ea-138">Полученный поставщиком и вычисляемый показатель риска для узла.</span><span class="sxs-lookup"><span data-stu-id="6e8ea-138">Provider-generated/calculated risk score of the host.</span></span>  <span data-ttu-id="6e8ea-139">Рекомендуемый диапазон значений 0-1, указывающий на процентное соотношение.</span><span class="sxs-lookup"><span data-stu-id="6e8ea-139">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6e8ea-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6e8ea-140">JSON representation</span></span>

<span data-ttu-id="6e8ea-141">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6e8ea-141">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "hostSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
