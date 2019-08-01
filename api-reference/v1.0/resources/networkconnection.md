---
title: Тип ресурса networkConnection
description: Содержит сведения о состоянии сетевого подключения, связанного с оповещением.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 25750b5484558c53ab03d3001bc2b8bafa307524
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035996"
---
# <a name="networkconnection-resource-type"></a><span data-ttu-id="9660f-103">Тип ресурса networkConnection</span><span class="sxs-lookup"><span data-stu-id="9660f-103">networkConnection resource type</span></span>

<span data-ttu-id="9660f-104">Содержит сведения о состоянии сетевого подключения, связанного с оповещением.</span><span class="sxs-lookup"><span data-stu-id="9660f-104">Contains stateful information about the network connection related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="9660f-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="9660f-105">Properties</span></span>

| <span data-ttu-id="9660f-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="9660f-106">Property</span></span>   | <span data-ttu-id="9660f-107">Тип</span><span class="sxs-lookup"><span data-stu-id="9660f-107">Type</span></span>|<span data-ttu-id="9660f-108">Описание</span><span class="sxs-lookup"><span data-stu-id="9660f-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9660f-109">applicationName</span><span class="sxs-lookup"><span data-stu-id="9660f-109">applicationName</span></span>|<span data-ttu-id="9660f-110">String</span><span class="sxs-lookup"><span data-stu-id="9660f-110">String</span></span>|<span data-ttu-id="9660f-111">Имя приложения, управляющего сетевым подключением (например, Facebook, SMTP и т. д.).</span><span class="sxs-lookup"><span data-stu-id="9660f-111">Name of the application managing the network connection (for example, Facebook, SMTP, etc.).</span></span>|
|<span data-ttu-id="9660f-112">Дестинатионаддресс</span><span class="sxs-lookup"><span data-stu-id="9660f-112">destinationAddress</span></span>|<span data-ttu-id="9660f-113">String</span><span class="sxs-lookup"><span data-stu-id="9660f-113">String</span></span>|<span data-ttu-id="9660f-114">Конечный IP-адрес (сетевого подключения).</span><span class="sxs-lookup"><span data-stu-id="9660f-114">Destination IP address (of the network connection).</span></span>|
|<span data-ttu-id="9660f-115">Дестинатиондомаин</span><span class="sxs-lookup"><span data-stu-id="9660f-115">destinationDomain</span></span>|<span data-ttu-id="9660f-116">String</span><span class="sxs-lookup"><span data-stu-id="9660f-116">String</span></span>|<span data-ttu-id="9660f-117">Часть конечного домена, в которой находится конечный URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="9660f-117">Destination domain portion of the destination URL.</span></span> <span data-ttu-id="9660f-118">(например, "www.contoso.com").</span><span class="sxs-lookup"><span data-stu-id="9660f-118">(for example 'www.contoso.com').</span></span>|
|<span data-ttu-id="9660f-119">Дестинатионпорт</span><span class="sxs-lookup"><span data-stu-id="9660f-119">destinationPort</span></span>|<span data-ttu-id="9660f-120">String</span><span class="sxs-lookup"><span data-stu-id="9660f-120">String</span></span>|<span data-ttu-id="9660f-121">Порт назначения (для сетевого подключения).</span><span class="sxs-lookup"><span data-stu-id="9660f-121">Destination port (of the network connection).</span></span>|
|<span data-ttu-id="9660f-122">Дестинатионурл</span><span class="sxs-lookup"><span data-stu-id="9660f-122">destinationUrl</span></span>|<span data-ttu-id="9660f-123">String</span><span class="sxs-lookup"><span data-stu-id="9660f-123">String</span></span>|<span data-ttu-id="9660f-124">URL-адрес сетевого подключения/URI-строка — без параметров.</span><span class="sxs-lookup"><span data-stu-id="9660f-124">Network connection URL/URI string - excluding parameters.</span></span> <span data-ttu-id="9660f-125">(например, "www.contoso.com/products/default.html")</span><span class="sxs-lookup"><span data-stu-id="9660f-125">(for example 'www.contoso.com/products/default.html')</span></span>|
|<span data-ttu-id="9660f-126">direction</span><span class="sxs-lookup"><span data-stu-id="9660f-126">direction</span></span>|<span data-ttu-id="9660f-127">connectionDirection</span><span class="sxs-lookup"><span data-stu-id="9660f-127">connectionDirection</span></span>|<span data-ttu-id="9660f-128">Направление сетевого подключения.</span><span class="sxs-lookup"><span data-stu-id="9660f-128">Network connection direction.</span></span> <span data-ttu-id="9660f-129">Возможные значения: `unknown`, `inbound`, `outbound`.</span><span class="sxs-lookup"><span data-stu-id="9660f-129">Possible values are: `unknown`, `inbound`, `outbound`.</span></span>|
|<span data-ttu-id="9660f-130">Домаинрегистереддатетиме</span><span class="sxs-lookup"><span data-stu-id="9660f-130">domainRegisteredDateTime</span></span>|<span data-ttu-id="9660f-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9660f-131">DateTimeOffset</span></span>|<span data-ttu-id="9660f-132">Дата регистрации конечного домена.</span><span class="sxs-lookup"><span data-stu-id="9660f-132">Date when the destination domain was registered.</span></span> <span data-ttu-id="9660f-133">Тип Timestamp представляет сведения о дате и времени с использованием формата ISO 8601, причем всегда используется время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="9660f-133">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9660f-134">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="9660f-134">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9660f-135">Локалднснаме</span><span class="sxs-lookup"><span data-stu-id="9660f-135">localDnsName</span></span>|<span data-ttu-id="9660f-136">String</span><span class="sxs-lookup"><span data-stu-id="9660f-136">String</span></span>|<span data-ttu-id="9660f-137">Локальное разрешение DNS-имен, отображаемое в локальном кэше DNS узла (например, на случай, если файл hosts был подделан).</span><span class="sxs-lookup"><span data-stu-id="9660f-137">The local DNS name resolution as it appears in the host's local DNS cache (for example, in case the 'hosts' file was tampered with).</span></span>|
|<span data-ttu-id="9660f-138">Натдестинатионаддресс</span><span class="sxs-lookup"><span data-stu-id="9660f-138">natDestinationAddress</span></span>|<span data-ttu-id="9660f-139">String</span><span class="sxs-lookup"><span data-stu-id="9660f-139">String</span></span>|<span data-ttu-id="9660f-140">IP-адрес назначения преобразования сетевых адресов.</span><span class="sxs-lookup"><span data-stu-id="9660f-140">Network Address Translation destination IP address.</span></span>|
|<span data-ttu-id="9660f-141">Натдестинатионпорт</span><span class="sxs-lookup"><span data-stu-id="9660f-141">natDestinationPort</span></span>|<span data-ttu-id="9660f-142">String</span><span class="sxs-lookup"><span data-stu-id="9660f-142">String</span></span>|<span data-ttu-id="9660f-143">Порт назначения преобразования сетевых адресов.</span><span class="sxs-lookup"><span data-stu-id="9660f-143">Network Address Translation destination port.</span></span>|
|<span data-ttu-id="9660f-144">Натсаурцеаддресс</span><span class="sxs-lookup"><span data-stu-id="9660f-144">natSourceAddress</span></span>|<span data-ttu-id="9660f-145">String</span><span class="sxs-lookup"><span data-stu-id="9660f-145">String</span></span>|<span data-ttu-id="9660f-146">IP-адрес источника преобразования сетевых адресов.</span><span class="sxs-lookup"><span data-stu-id="9660f-146">Network Address Translation source IP address.</span></span>|
|<span data-ttu-id="9660f-147">Натсаурцепорт</span><span class="sxs-lookup"><span data-stu-id="9660f-147">natSourcePort</span></span>|<span data-ttu-id="9660f-148">String</span><span class="sxs-lookup"><span data-stu-id="9660f-148">String</span></span>|<span data-ttu-id="9660f-149">Порт источника преобразования сетевых адресов.</span><span class="sxs-lookup"><span data-stu-id="9660f-149">Network Address Translation source port.</span></span>|
|<span data-ttu-id="9660f-150">Protocol</span><span class="sxs-lookup"><span data-stu-id="9660f-150">protocol</span></span>|[<span data-ttu-id="9660f-151">securityNetworkProtocol</span><span class="sxs-lookup"><span data-stu-id="9660f-151">securityNetworkProtocol</span></span>](securitynetworkprotocol.md)|<span data-ttu-id="9660f-152">Сетевой протокол.</span><span class="sxs-lookup"><span data-stu-id="9660f-152">Network protocol.</span></span> <span data-ttu-id="9660f-153">Возможные значения: `unknown`, `ip`, `icmp`, `igmp` `ggp` `ipv4` `tcp` `ipSecEncapsulatingSecurityPayload` `ipSecAuthenticationHeader` `icmpV6` `ipv6NoNextHeader` `ipv6DestinationOptions` `nd` `ipv6RoutingHeader` `ipv6FragmentHeader`,,,,,,,,,,,,,,,,,,,,, `pup` `udp` `idp` `ipv6` , `raw`, `ipx`, `spx`, `spxII`.</span><span class="sxs-lookup"><span data-stu-id="9660f-153">Possible values are: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd`, `raw`, `ipx`, `spx`, `spxII`.</span></span>|
|<span data-ttu-id="9660f-154">riskScore</span><span class="sxs-lookup"><span data-stu-id="9660f-154">riskScore</span></span>|<span data-ttu-id="9660f-155">String</span><span class="sxs-lookup"><span data-stu-id="9660f-155">String</span></span>|<span data-ttu-id="9660f-156">Созданный поставщиком/вычисляемый показатель риска для сетевого подключения.</span><span class="sxs-lookup"><span data-stu-id="9660f-156">Provider generated/calculated risk score of the network connection.</span></span> <span data-ttu-id="9660f-157">Рекомендуемый диапазон значений 0-1, указывающий на процентное соотношение.</span><span class="sxs-lookup"><span data-stu-id="9660f-157">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="9660f-158">Саурцеаддресс</span><span class="sxs-lookup"><span data-stu-id="9660f-158">sourceAddress</span></span>|<span data-ttu-id="9660f-159">String</span><span class="sxs-lookup"><span data-stu-id="9660f-159">String</span></span>|<span data-ttu-id="9660f-160">Источник (то есть источник) IP-адрес сетевого подключения.</span><span class="sxs-lookup"><span data-stu-id="9660f-160">Source (i.e. origin) IP address (of the network connection).</span></span>|
|<span data-ttu-id="9660f-161">Саурцепорт</span><span class="sxs-lookup"><span data-stu-id="9660f-161">sourcePort</span></span>|<span data-ttu-id="9660f-162">String</span><span class="sxs-lookup"><span data-stu-id="9660f-162">String</span></span>|<span data-ttu-id="9660f-163">Исходный (то есть источник) IP-порт (сетевого подключения).</span><span class="sxs-lookup"><span data-stu-id="9660f-163">Source (i.e. origin) IP port (of the network connection).</span></span>|
|<span data-ttu-id="9660f-164">status</span><span class="sxs-lookup"><span data-stu-id="9660f-164">status</span></span>|<span data-ttu-id="9660f-165">connectionStatus</span><span class="sxs-lookup"><span data-stu-id="9660f-165">connectionStatus</span></span>|<span data-ttu-id="9660f-166">Состояние сетевого подключения.</span><span class="sxs-lookup"><span data-stu-id="9660f-166">Network connection status.</span></span> <span data-ttu-id="9660f-167">Возможные значения: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="9660f-167">Possible values are: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span></span>|
|<span data-ttu-id="9660f-168">Урлпараметерс</span><span class="sxs-lookup"><span data-stu-id="9660f-168">urlParameters</span></span>|<span data-ttu-id="9660f-169">String</span><span class="sxs-lookup"><span data-stu-id="9660f-169">String</span></span>|<span data-ttu-id="9660f-170">Параметры (суффикс) конечного URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="9660f-170">Parameters (suffix) of the destination URL.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9660f-171">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9660f-171">JSON representation</span></span>

<span data-ttu-id="9660f-172">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9660f-172">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.networkConnection"
}-->

```json
{
  "applicationName": "String",
  "destinationAddress": "String",
  "destinationDomain": "String",
  "destinationPort": "String",
  "destinationUrl": "String",
  "direction": "@odata.type: microsoft.graph.connectionDirection",
  "domainRegisteredDateTime": "String (timestamp)",
  "localDnsName": "String",
  "natDestinationAddress": "String",
  "natDestinationPort": "String",
  "natSourceAddress": "String",
  "natSourcePort": "String",
  "protocol": "@odata.type: microsoft.graph.securityNetworkProtocol",
  "riskScore": "String",
  "sourceAddress": "String",
  "sourcePort": "String",
  "status": "@odata.type: microsoft.graph.connectionStatus",
  "urlParameters": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "networkConnection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
