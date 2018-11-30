---
title: Тип ресурса hostSecurityState
description: Содержит с сохранением состояния сведения об узле (включая устройства, компьютеры и т. п.).
ms.openlocfilehash: 3649553ae0f96222a09825e8819dfd0d199f8454
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027197"
---
# <a name="hostsecuritystate-resource-type"></a><span data-ttu-id="d641a-103">Тип ресурса hostSecurityState</span><span class="sxs-lookup"><span data-stu-id="d641a-103">hostSecurityState resource type</span></span>

<span data-ttu-id="d641a-104">Содержит с сохранением состояния сведения об узле (включая устройства, компьютеры и т. п.).</span><span class="sxs-lookup"><span data-stu-id="d641a-104">Contains stateful information about the host (including devices, computers, and so on).</span></span>

## <a name="properties"></a><span data-ttu-id="d641a-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="d641a-105">Properties</span></span>

| <span data-ttu-id="d641a-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="d641a-106">Property</span></span>   | <span data-ttu-id="d641a-107">Тип</span><span class="sxs-lookup"><span data-stu-id="d641a-107">Type</span></span>|<span data-ttu-id="d641a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="d641a-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d641a-109">полное доменное имя</span><span class="sxs-lookup"><span data-stu-id="d641a-109">fqdn</span></span>|<span data-ttu-id="d641a-110">String</span><span class="sxs-lookup"><span data-stu-id="d641a-110">String</span></span>|<span data-ttu-id="d641a-111">Полное доменное имя (полное доменное имя) размещения (например, `machine.company.com`).</span><span class="sxs-lookup"><span data-stu-id="d641a-111">Host FQDN (Fully Qualified Domain Name) (for example, `machine.company.com`).</span></span>|
|<span data-ttu-id="d641a-112">isAzureAadJoined</span><span class="sxs-lookup"><span data-stu-id="d641a-112">isAzureAadJoined</span></span>|<span data-ttu-id="d641a-113">Логический</span><span class="sxs-lookup"><span data-stu-id="d641a-113">Boolean</span></span>|<span data-ttu-id="d641a-114">Значение true, если узел является домен, в состав доменных служб Active Directory Azure.</span><span class="sxs-lookup"><span data-stu-id="d641a-114">True if the host is domain joined to Azure Active Directory Domain Services.</span></span>|
|<span data-ttu-id="d641a-115">isAzureAadRegistered</span><span class="sxs-lookup"><span data-stu-id="d641a-115">isAzureAadRegistered</span></span>|<span data-ttu-id="d641a-116">Логический</span><span class="sxs-lookup"><span data-stu-id="d641a-116">Boolean</span></span>|<span data-ttu-id="d641a-117">Значение true, если узел зарегистрирован устройства регистрации Azure Active Directory (BYOD устройства - то есть, не полностью управляются предприятия).</span><span class="sxs-lookup"><span data-stu-id="d641a-117">True if the host registered with Azure Active Directory Device Registration (BYOD devices - that is, not fully managed by enterprise).</span></span>|
|<span data-ttu-id="d641a-118">isHybridAzureDomainJoined</span><span class="sxs-lookup"><span data-stu-id="d641a-118">isHybridAzureDomainJoined</span></span>|<span data-ttu-id="d641a-119">Логический</span><span class="sxs-lookup"><span data-stu-id="d641a-119">Boolean</span></span>|<span data-ttu-id="d641a-120">Значение true, если узел присоединен к домену на локальный домен Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d641a-120">True if the host is domain joined to an on-premises Active Directory domain.</span></span>|
|<span data-ttu-id="d641a-121">netBiosName</span><span class="sxs-lookup"><span data-stu-id="d641a-121">netBiosName</span></span>|<span data-ttu-id="d641a-122">String</span><span class="sxs-lookup"><span data-stu-id="d641a-122">String</span></span>|<span data-ttu-id="d641a-123">Имя локального узла без DNS-имени домена.</span><span class="sxs-lookup"><span data-stu-id="d641a-123">The local host name, without the DNS domain name.</span></span>|
|<span data-ttu-id="d641a-124">операционная система</span><span class="sxs-lookup"><span data-stu-id="d641a-124">os</span></span>|<span data-ttu-id="d641a-125">String</span><span class="sxs-lookup"><span data-stu-id="d641a-125">String</span></span>|<span data-ttu-id="d641a-126">Операционной системы.</span><span class="sxs-lookup"><span data-stu-id="d641a-126">Host Operating System.</span></span> <span data-ttu-id="d641a-127">(Например, Windows10, MacOS, RHEL, и т.д.).</span><span class="sxs-lookup"><span data-stu-id="d641a-127">(For example, Windows10, MacOS, RHEL, etc.).</span></span>|
|<span data-ttu-id="d641a-128">privateIpAddress</span><span class="sxs-lookup"><span data-stu-id="d641a-128">privateIpAddress</span></span>|<span data-ttu-id="d641a-129">String</span><span class="sxs-lookup"><span data-stu-id="d641a-129">String</span></span>|<span data-ttu-id="d641a-130">Частный (не маршрутизируемые) адрес IPv4 или IPv6 [(см)](https://tools.ietf.org/html/rfc1918)во время оповещения.</span><span class="sxs-lookup"><span data-stu-id="d641a-130">Private (not routable) IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at the time of the alert.</span></span>|
|<span data-ttu-id="d641a-131">publicIpAddress</span><span class="sxs-lookup"><span data-stu-id="d641a-131">publicIpAddress</span></span>|<span data-ttu-id="d641a-132">String</span><span class="sxs-lookup"><span data-stu-id="d641a-132">String</span></span>|<span data-ttu-id="d641a-133">Открыто маршрутизируемыми IPv4 или IPv6-адрес [(см)](https://tools.ietf.org/html/rfc1918)во время оповещения.</span><span class="sxs-lookup"><span data-stu-id="d641a-133">Publicly routable IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at time of the alert.</span></span>|
|<span data-ttu-id="d641a-134">riskScore</span><span class="sxs-lookup"><span data-stu-id="d641a-134">riskScore</span></span>|<span data-ttu-id="d641a-135">String</span><span class="sxs-lookup"><span data-stu-id="d641a-135">String</span></span>|<span data-ttu-id="d641a-136">Оценка риска поставщика создается/вычисляемые узла.</span><span class="sxs-lookup"><span data-stu-id="d641a-136">Provider-generated/calculated risk score of the host.</span></span>  <span data-ttu-id="d641a-137">Рекомендуемое значение диапазона 0-1, который соответствует в процентах.</span><span class="sxs-lookup"><span data-stu-id="d641a-137">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d641a-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d641a-138">JSON representation</span></span>

<span data-ttu-id="d641a-139">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d641a-139">The following is a JSON representation of the resource.</span></span>

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
