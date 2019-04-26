---
title: Тип ресурса Хостсекуритистате
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
ms.openlocfilehash: 670a052fa3d63da0b78ba620dbc6530a8ab122dc
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340312"
---
# <a name="hostsecuritystate-resource-type"></a><span data-ttu-id="6a804-104">Тип ресурса Хостсекуритистате</span><span class="sxs-lookup"><span data-stu-id="6a804-104">hostSecurityState resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a804-105">Содержит сведения о состоянии узла (включая устройства, компьютеры и т. д.).</span><span class="sxs-lookup"><span data-stu-id="6a804-105">Contains stateful information about the host (including devices, computers, and so on).</span></span>

## <a name="properties"></a><span data-ttu-id="6a804-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="6a804-106">Properties</span></span>

| <span data-ttu-id="6a804-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="6a804-107">Property</span></span>   | <span data-ttu-id="6a804-108">Тип</span><span class="sxs-lookup"><span data-stu-id="6a804-108">Type</span></span>|<span data-ttu-id="6a804-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6a804-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6a804-110">полным</span><span class="sxs-lookup"><span data-stu-id="6a804-110">fqdn</span></span>|<span data-ttu-id="6a804-111">String</span><span class="sxs-lookup"><span data-stu-id="6a804-111">String</span></span>|<span data-ttu-id="6a804-112">ПОЛНОЕ доменное имя узла (полное доменное имя) (например, machine.company.com).</span><span class="sxs-lookup"><span data-stu-id="6a804-112">Host FQDN (Fully Qualified Domain Name) (for example, machine.company.com).</span></span>|
|<span data-ttu-id="6a804-113">Исазуреааджоинед</span><span class="sxs-lookup"><span data-stu-id="6a804-113">isAzureAadJoined</span></span>|<span data-ttu-id="6a804-114">Логический</span><span class="sxs-lookup"><span data-stu-id="6a804-114">Boolean</span></span>|<span data-ttu-id="6a804-115">True, если узел подключен к доменным службам Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6a804-115">True if the host is domain joined to Azure Active Directory Domain Services.</span></span>|
|<span data-ttu-id="6a804-116">Исазуреаадрегистеред</span><span class="sxs-lookup"><span data-stu-id="6a804-116">isAzureAadRegistered</span></span>|<span data-ttu-id="6a804-117">Логический</span><span class="sxs-lookup"><span data-stu-id="6a804-117">Boolean</span></span>|<span data-ttu-id="6a804-118">True, если узел зарегистрирован с регистрацией устройств Azure Active Directory (BYOD Devices — то есть, не полностью управляется предприятием).</span><span class="sxs-lookup"><span data-stu-id="6a804-118">True if the host registered with Azure Active Directory Device Registration (BYOD devices - that is, not fully managed by enterprise).</span></span>|
|<span data-ttu-id="6a804-119">Ишибридазуредомаинжоинед</span><span class="sxs-lookup"><span data-stu-id="6a804-119">isHybridAzureDomainJoined</span></span>|<span data-ttu-id="6a804-120">Логический</span><span class="sxs-lookup"><span data-stu-id="6a804-120">Boolean</span></span>|<span data-ttu-id="6a804-121">True, если узел является доменом, присоединенным к локальному домену Active Directory.</span><span class="sxs-lookup"><span data-stu-id="6a804-121">True if the host is domain joined to an on-premises Active Directory domain.</span></span>|
|<span data-ttu-id="6a804-122">Нетбиоснаме</span><span class="sxs-lookup"><span data-stu-id="6a804-122">netBiosName</span></span>|<span data-ttu-id="6a804-123">String</span><span class="sxs-lookup"><span data-stu-id="6a804-123">String</span></span>|<span data-ttu-id="6a804-124">Имя локального узла без DNS-имени домена.</span><span class="sxs-lookup"><span data-stu-id="6a804-124">The local host name, without the DNS domain name.</span></span>|
|<span data-ttu-id="6a804-125">совместим</span><span class="sxs-lookup"><span data-stu-id="6a804-125">os</span></span>|<span data-ttu-id="6a804-126">String</span><span class="sxs-lookup"><span data-stu-id="6a804-126">String</span></span>|<span data-ttu-id="6a804-127">Хост операционной системы.</span><span class="sxs-lookup"><span data-stu-id="6a804-127">Host Operating System.</span></span> <span data-ttu-id="6a804-128">(Например, Windows10, MacOS, РХЕЛ и т. д.).</span><span class="sxs-lookup"><span data-stu-id="6a804-128">(For example, Windows10, MacOS, RHEL, etc.).</span></span>|
|<span data-ttu-id="6a804-129">Приватеипаддресс</span><span class="sxs-lookup"><span data-stu-id="6a804-129">privateIpAddress</span></span>|<span data-ttu-id="6a804-130">String</span><span class="sxs-lookup"><span data-stu-id="6a804-130">String</span></span>|<span data-ttu-id="6a804-131">Частный (без маршрутизации) IPv4-или IPv6-адрес (см. [RFC 1918](https://tools.ietf.org/html/rfc1918)) на момент оповещения.</span><span class="sxs-lookup"><span data-stu-id="6a804-131">Private (not routable) IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at the time of the alert.</span></span>|
|<span data-ttu-id="6a804-132">ПублиЦипаддресс</span><span class="sxs-lookup"><span data-stu-id="6a804-132">publicIpAddress</span></span>|<span data-ttu-id="6a804-133">String</span><span class="sxs-lookup"><span data-stu-id="6a804-133">String</span></span>|<span data-ttu-id="6a804-134">IPv4-или IPv6-адрес общеДоступной маршрутизации (см. [RFC 1918](https://tools.ietf.org/html/rfc1918)) во время оповещения.</span><span class="sxs-lookup"><span data-stu-id="6a804-134">Publicly routable IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at time of the alert.</span></span>|
|<span data-ttu-id="6a804-135">riskScore</span><span class="sxs-lookup"><span data-stu-id="6a804-135">riskScore</span></span>|<span data-ttu-id="6a804-136">String</span><span class="sxs-lookup"><span data-stu-id="6a804-136">String</span></span>|<span data-ttu-id="6a804-137">Полученный поставщиком и вычисляемый показатель риска для узла.</span><span class="sxs-lookup"><span data-stu-id="6a804-137">Provider-generated/calculated risk score of the host.</span></span>  <span data-ttu-id="6a804-138">Рекомендуемый диапазон значений 0-1, указывающий на процентное соотношение.</span><span class="sxs-lookup"><span data-stu-id="6a804-138">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6a804-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6a804-139">JSON representation</span></span>

<span data-ttu-id="6a804-140">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6a804-140">The following is a JSON representation of the resource.</span></span>

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
