---
title: Тип ресурса networkConnection
description: Содержит сведения о состоянии сетевого подключения, связанного с оповещением.
localization_priority: Normal
author: chinguyen1
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 72fcfcd3c6849e9c8e9f05b50671e1aa611dc129
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2020
ms.locfileid: "44682056"
---
# <a name="networkconnection-resource-type"></a><span data-ttu-id="56844-103">Тип ресурса networkConnection</span><span class="sxs-lookup"><span data-stu-id="56844-103">networkConnection resource type</span></span>

<span data-ttu-id="56844-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56844-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="56844-105">Содержит сведения о состоянии сетевого подключения, связанного с оповещением.</span><span class="sxs-lookup"><span data-stu-id="56844-105">Contains stateful information about the network connection related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="56844-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="56844-106">Properties</span></span>

| <span data-ttu-id="56844-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="56844-107">Property</span></span>   | <span data-ttu-id="56844-108">Тип</span><span class="sxs-lookup"><span data-stu-id="56844-108">Type</span></span>|<span data-ttu-id="56844-109">Описание</span><span class="sxs-lookup"><span data-stu-id="56844-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="56844-110">applicationName</span><span class="sxs-lookup"><span data-stu-id="56844-110">applicationName</span></span>|<span data-ttu-id="56844-111">String</span><span class="sxs-lookup"><span data-stu-id="56844-111">String</span></span>|<span data-ttu-id="56844-112">Имя приложения, управляющего сетевым подключением (например, Facebook или SMTP).</span><span class="sxs-lookup"><span data-stu-id="56844-112">Name of the application managing the network connection (for example, Facebook or SMTP).</span></span>|
|<span data-ttu-id="56844-113">дестинатионаддресс</span><span class="sxs-lookup"><span data-stu-id="56844-113">destinationAddress</span></span>|<span data-ttu-id="56844-114">String</span><span class="sxs-lookup"><span data-stu-id="56844-114">String</span></span>|<span data-ttu-id="56844-115">Конечный IP-адрес (сетевого подключения).</span><span class="sxs-lookup"><span data-stu-id="56844-115">Destination IP address (of the network connection).</span></span>|
|<span data-ttu-id="56844-116">дестинатионлокатион</span><span class="sxs-lookup"><span data-stu-id="56844-116">destinationLocation</span></span>|<span data-ttu-id="56844-117">String</span><span class="sxs-lookup"><span data-stu-id="56844-117">String</span></span>|<span data-ttu-id="56844-118">Расположение (по сопоставлению IP-адресов), связанное с назначением сетевого подключения.</span><span class="sxs-lookup"><span data-stu-id="56844-118">Location (by IP address mapping) associated with the destination of a network connection.</span></span>|
|<span data-ttu-id="56844-119">дестинатиондомаин</span><span class="sxs-lookup"><span data-stu-id="56844-119">destinationDomain</span></span>|<span data-ttu-id="56844-120">String</span><span class="sxs-lookup"><span data-stu-id="56844-120">String</span></span>|<span data-ttu-id="56844-121">Часть конечного домена, в которой находится конечный URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="56844-121">Destination domain portion of the destination URL.</span></span> <span data-ttu-id="56844-122">(например, "www.contoso.com").</span><span class="sxs-lookup"><span data-stu-id="56844-122">(for example 'www.contoso.com').</span></span>|
|<span data-ttu-id="56844-123">дестинатионпорт</span><span class="sxs-lookup"><span data-stu-id="56844-123">destinationPort</span></span>|<span data-ttu-id="56844-124">String</span><span class="sxs-lookup"><span data-stu-id="56844-124">String</span></span>|<span data-ttu-id="56844-125">Порт назначения (для сетевого подключения).</span><span class="sxs-lookup"><span data-stu-id="56844-125">Destination port (of the network connection).</span></span>|
|<span data-ttu-id="56844-126">дестинатионурл</span><span class="sxs-lookup"><span data-stu-id="56844-126">destinationUrl</span></span>|<span data-ttu-id="56844-127">String</span><span class="sxs-lookup"><span data-stu-id="56844-127">String</span></span>|<span data-ttu-id="56844-128">URL-адрес сетевого подключения/URI-строка — без параметров.</span><span class="sxs-lookup"><span data-stu-id="56844-128">Network connection URL/URI string - excluding parameters.</span></span> <span data-ttu-id="56844-129">(например, "www.contoso.com/products/default.html")</span><span class="sxs-lookup"><span data-stu-id="56844-129">(for example 'www.contoso.com/products/default.html')</span></span>|
|<span data-ttu-id="56844-130">direction</span><span class="sxs-lookup"><span data-stu-id="56844-130">direction</span></span>|<span data-ttu-id="56844-131">connectionDirection</span><span class="sxs-lookup"><span data-stu-id="56844-131">connectionDirection</span></span>|<span data-ttu-id="56844-132">Направление сетевого подключения.</span><span class="sxs-lookup"><span data-stu-id="56844-132">Network connection direction.</span></span> <span data-ttu-id="56844-133">Возможные значения: `unknown`, `inbound`, `outbound`.</span><span class="sxs-lookup"><span data-stu-id="56844-133">Possible values are: `unknown`, `inbound`, `outbound`.</span></span>|
|<span data-ttu-id="56844-134">домаинрегистереддатетиме</span><span class="sxs-lookup"><span data-stu-id="56844-134">domainRegisteredDateTime</span></span>|<span data-ttu-id="56844-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56844-135">DateTimeOffset</span></span>|<span data-ttu-id="56844-136">Дата регистрации конечного домена.</span><span class="sxs-lookup"><span data-stu-id="56844-136">Date when the destination domain was registered.</span></span> <span data-ttu-id="56844-137">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="56844-137">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="56844-138">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="56844-138">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="56844-139">локалднснаме</span><span class="sxs-lookup"><span data-stu-id="56844-139">localDnsName</span></span>|<span data-ttu-id="56844-140">String</span><span class="sxs-lookup"><span data-stu-id="56844-140">String</span></span>|<span data-ttu-id="56844-141">Локальное разрешение DNS-имен, отображаемое в локальном кэше DNS узла (например, на случай, если файл hosts был подделан).</span><span class="sxs-lookup"><span data-stu-id="56844-141">The local DNS name resolution as it appears in the host's local DNS cache (for example, in case the 'hosts' file was tampered with).</span></span>|
|<span data-ttu-id="56844-142">натдестинатионаддресс</span><span class="sxs-lookup"><span data-stu-id="56844-142">natDestinationAddress</span></span>|<span data-ttu-id="56844-143">String</span><span class="sxs-lookup"><span data-stu-id="56844-143">String</span></span>|<span data-ttu-id="56844-144">IP-адрес назначения преобразования сетевых адресов.</span><span class="sxs-lookup"><span data-stu-id="56844-144">Network Address Translation destination IP address.</span></span>|
|<span data-ttu-id="56844-145">натдестинатионпорт</span><span class="sxs-lookup"><span data-stu-id="56844-145">natDestinationPort</span></span>|<span data-ttu-id="56844-146">String</span><span class="sxs-lookup"><span data-stu-id="56844-146">String</span></span>|<span data-ttu-id="56844-147">Порт назначения преобразования сетевых адресов.</span><span class="sxs-lookup"><span data-stu-id="56844-147">Network Address Translation destination port.</span></span>|
|<span data-ttu-id="56844-148">натсаурцеаддресс</span><span class="sxs-lookup"><span data-stu-id="56844-148">natSourceAddress</span></span>|<span data-ttu-id="56844-149">String</span><span class="sxs-lookup"><span data-stu-id="56844-149">String</span></span>|<span data-ttu-id="56844-150">IP-адрес источника преобразования сетевых адресов.</span><span class="sxs-lookup"><span data-stu-id="56844-150">Network Address Translation source IP address.</span></span>|
|<span data-ttu-id="56844-151">натсаурцепорт</span><span class="sxs-lookup"><span data-stu-id="56844-151">natSourcePort</span></span>|<span data-ttu-id="56844-152">String</span><span class="sxs-lookup"><span data-stu-id="56844-152">String</span></span>|<span data-ttu-id="56844-153">Порт источника преобразования сетевых адресов.</span><span class="sxs-lookup"><span data-stu-id="56844-153">Network Address Translation source port.</span></span>|
|<span data-ttu-id="56844-154">Protocol</span><span class="sxs-lookup"><span data-stu-id="56844-154">protocol</span></span>|[<span data-ttu-id="56844-155">securityNetworkProtocol</span><span class="sxs-lookup"><span data-stu-id="56844-155">securityNetworkProtocol</span></span>](securitynetworkprotocol.md)|<span data-ttu-id="56844-156">Сетевой протокол.</span><span class="sxs-lookup"><span data-stu-id="56844-156">Network protocol.</span></span> <span data-ttu-id="56844-157">Возможные значения:,,,,,,,,,,, `unknown` `ip` `icmp` `igmp` `ggp` `ipv4` `tcp` `pup` `udp` `idp` `ipv6` `ipv6RoutingHeader` `ipv6FragmentHeader` , `ipSecEncapsulatingSecurityPayload` , `ipSecAuthenticationHeader` , `icmpV6` `ipv6NoNextHeader` `ipv6DestinationOptions` `nd` `raw` `ipx` `spx` `spxII` ,,,,,,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="56844-157">Possible values are: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd`, `raw`, `ipx`, `spx`, `spxII`.</span></span>|
|<span data-ttu-id="56844-158">riskScore</span><span class="sxs-lookup"><span data-stu-id="56844-158">riskScore</span></span>|<span data-ttu-id="56844-159">String</span><span class="sxs-lookup"><span data-stu-id="56844-159">String</span></span>|<span data-ttu-id="56844-160">Созданный поставщиком/вычисляемый показатель риска для сетевого подключения.</span><span class="sxs-lookup"><span data-stu-id="56844-160">Provider generated/calculated risk score of the network connection.</span></span> <span data-ttu-id="56844-161">Рекомендуемый диапазон значений 0-1, указывающий на процентное соотношение.</span><span class="sxs-lookup"><span data-stu-id="56844-161">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="56844-162">саурцеаддресс</span><span class="sxs-lookup"><span data-stu-id="56844-162">sourceAddress</span></span>|<span data-ttu-id="56844-163">String</span><span class="sxs-lookup"><span data-stu-id="56844-163">String</span></span>|<span data-ttu-id="56844-164">Источник (то есть источник) IP-адрес сетевого подключения.</span><span class="sxs-lookup"><span data-stu-id="56844-164">Source (i.e. origin) IP address (of the network connection).</span></span>|
|<span data-ttu-id="56844-165">sourceLocation</span><span class="sxs-lookup"><span data-stu-id="56844-165">sourceLocation</span></span>|<span data-ttu-id="56844-166">String</span><span class="sxs-lookup"><span data-stu-id="56844-166">String</span></span>|<span data-ttu-id="56844-167">Расположение (по сопоставлению IP-адресов), связанное с источником сетевого подключения.</span><span class="sxs-lookup"><span data-stu-id="56844-167">Location (by IP address mapping) associated with the source of a network connection.</span></span>|
|<span data-ttu-id="56844-168">саурцепорт</span><span class="sxs-lookup"><span data-stu-id="56844-168">sourcePort</span></span>|<span data-ttu-id="56844-169">String</span><span class="sxs-lookup"><span data-stu-id="56844-169">String</span></span>|<span data-ttu-id="56844-170">Исходный (то есть источник) IP-порт (сетевого подключения).</span><span class="sxs-lookup"><span data-stu-id="56844-170">Source (i.e. origin) IP port (of the network connection).</span></span>|
|<span data-ttu-id="56844-171">status</span><span class="sxs-lookup"><span data-stu-id="56844-171">status</span></span>|<span data-ttu-id="56844-172">connectionStatus</span><span class="sxs-lookup"><span data-stu-id="56844-172">connectionStatus</span></span>|<span data-ttu-id="56844-173">Состояние сетевого подключения.</span><span class="sxs-lookup"><span data-stu-id="56844-173">Network connection status.</span></span> <span data-ttu-id="56844-174">Возможные значения: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="56844-174">Possible values are: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span></span>|
|<span data-ttu-id="56844-175">урлпараметерс</span><span class="sxs-lookup"><span data-stu-id="56844-175">urlParameters</span></span>|<span data-ttu-id="56844-176">String</span><span class="sxs-lookup"><span data-stu-id="56844-176">String</span></span>|<span data-ttu-id="56844-177">Параметры (суффикс) конечного URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="56844-177">Parameters (suffix) of the destination URL.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="56844-178">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="56844-178">JSON representation</span></span>

<span data-ttu-id="56844-179">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="56844-179">The following is a JSON representation of the resource.</span></span>

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
  "destinationLocation": "String",
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
  "sourceLocation": "String",
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
