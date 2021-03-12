---
title: тип ресурса networkConnection
description: Содержит сведения о сетевом подключении, связанном с оповещением.
localization_priority: Normal
author: chinguyen1
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 5671726ead3da811c109a9a2afe01c49b665e513
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50719012"
---
# <a name="networkconnection-resource-type"></a><span data-ttu-id="9c367-103">тип ресурса networkConnection</span><span class="sxs-lookup"><span data-stu-id="9c367-103">networkConnection resource type</span></span>

<span data-ttu-id="9c367-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c367-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9c367-105">Содержит сведения о сетевом подключении, связанном с оповещением.</span><span class="sxs-lookup"><span data-stu-id="9c367-105">Contains stateful information about the network connection related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="9c367-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="9c367-106">Properties</span></span>

| <span data-ttu-id="9c367-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="9c367-107">Property</span></span>   | <span data-ttu-id="9c367-108">Тип</span><span class="sxs-lookup"><span data-stu-id="9c367-108">Type</span></span>|<span data-ttu-id="9c367-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9c367-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9c367-110">applicationName</span><span class="sxs-lookup"><span data-stu-id="9c367-110">applicationName</span></span>|<span data-ttu-id="9c367-111">String</span><span class="sxs-lookup"><span data-stu-id="9c367-111">String</span></span>|<span data-ttu-id="9c367-112">Имя приложения, управляющего сетевым подключением (например, Facebook или SMTP).</span><span class="sxs-lookup"><span data-stu-id="9c367-112">Name of the application managing the network connection (for example, Facebook or SMTP).</span></span>|
|<span data-ttu-id="9c367-113">destinationAddress</span><span class="sxs-lookup"><span data-stu-id="9c367-113">destinationAddress</span></span>|<span data-ttu-id="9c367-114">String</span><span class="sxs-lookup"><span data-stu-id="9c367-114">String</span></span>|<span data-ttu-id="9c367-115">IP-адрес назначения (сетевого подключения).</span><span class="sxs-lookup"><span data-stu-id="9c367-115">Destination IP address (of the network connection).</span></span>|
|<span data-ttu-id="9c367-116">destinationLocation</span><span class="sxs-lookup"><span data-stu-id="9c367-116">destinationLocation</span></span>|<span data-ttu-id="9c367-117">String</span><span class="sxs-lookup"><span data-stu-id="9c367-117">String</span></span>|<span data-ttu-id="9c367-118">Расположение (сопоставление IP-адресов), связанное с назначением сетевого подключения.</span><span class="sxs-lookup"><span data-stu-id="9c367-118">Location (by IP address mapping) associated with the destination of a network connection.</span></span>|
|<span data-ttu-id="9c367-119">destinationDomain</span><span class="sxs-lookup"><span data-stu-id="9c367-119">destinationDomain</span></span>|<span data-ttu-id="9c367-120">String</span><span class="sxs-lookup"><span data-stu-id="9c367-120">String</span></span>|<span data-ttu-id="9c367-121">Часть домена назначения URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="9c367-121">Destination domain portion of the destination URL.</span></span> <span data-ttu-id="9c367-122">(например, "www.contoso.com").</span><span class="sxs-lookup"><span data-stu-id="9c367-122">(for example 'www.contoso.com').</span></span>|
|<span data-ttu-id="9c367-123">destinationPort</span><span class="sxs-lookup"><span data-stu-id="9c367-123">destinationPort</span></span>|<span data-ttu-id="9c367-124">String</span><span class="sxs-lookup"><span data-stu-id="9c367-124">String</span></span>|<span data-ttu-id="9c367-125">Порт назначения (сетевого подключения).</span><span class="sxs-lookup"><span data-stu-id="9c367-125">Destination port (of the network connection).</span></span>|
|<span data-ttu-id="9c367-126">destinationUrl</span><span class="sxs-lookup"><span data-stu-id="9c367-126">destinationUrl</span></span>|<span data-ttu-id="9c367-127">String</span><span class="sxs-lookup"><span data-stu-id="9c367-127">String</span></span>|<span data-ttu-id="9c367-128">Строка URL-адрес/строка URI сетевого подключения без учета параметров.</span><span class="sxs-lookup"><span data-stu-id="9c367-128">Network connection URL/URI string - excluding parameters.</span></span> <span data-ttu-id="9c367-129">(например, www.contoso.com/products/default.html')</span><span class="sxs-lookup"><span data-stu-id="9c367-129">(for example 'www.contoso.com/products/default.html')</span></span>|
|<span data-ttu-id="9c367-130">direction</span><span class="sxs-lookup"><span data-stu-id="9c367-130">direction</span></span>|<span data-ttu-id="9c367-131">connectionDirection</span><span class="sxs-lookup"><span data-stu-id="9c367-131">connectionDirection</span></span>|<span data-ttu-id="9c367-132">Направление сетевого подключения.</span><span class="sxs-lookup"><span data-stu-id="9c367-132">Network connection direction.</span></span> <span data-ttu-id="9c367-133">Возможные значения: `unknown`, `inbound`, `outbound`.</span><span class="sxs-lookup"><span data-stu-id="9c367-133">Possible values are: `unknown`, `inbound`, `outbound`.</span></span>|
|<span data-ttu-id="9c367-134">domainRegisteredDateTime</span><span class="sxs-lookup"><span data-stu-id="9c367-134">domainRegisteredDateTime</span></span>|<span data-ttu-id="9c367-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c367-135">DateTimeOffset</span></span>|<span data-ttu-id="9c367-136">Дата регистрации домена назначения.</span><span class="sxs-lookup"><span data-stu-id="9c367-136">Date when the destination domain was registered.</span></span> <span data-ttu-id="9c367-137">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="9c367-137">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9c367-138">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="9c367-138">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="9c367-139">localDnsName</span><span class="sxs-lookup"><span data-stu-id="9c367-139">localDnsName</span></span>|<span data-ttu-id="9c367-140">String</span><span class="sxs-lookup"><span data-stu-id="9c367-140">String</span></span>|<span data-ttu-id="9c367-141">Локальное разрешение имен DNS, как оно отображается в локальном DNS-кэше хоста (например, в случае, если файл "хост" был подделан).</span><span class="sxs-lookup"><span data-stu-id="9c367-141">The local DNS name resolution as it appears in the host's local DNS cache (for example, in case the 'hosts' file was tampered with).</span></span>|
|<span data-ttu-id="9c367-142">natDestinationAddress</span><span class="sxs-lookup"><span data-stu-id="9c367-142">natDestinationAddress</span></span>|<span data-ttu-id="9c367-143">String</span><span class="sxs-lookup"><span data-stu-id="9c367-143">String</span></span>|<span data-ttu-id="9c367-144">IP-адрес назначения перевода сетевого адреса.</span><span class="sxs-lookup"><span data-stu-id="9c367-144">Network Address Translation destination IP address.</span></span>|
|<span data-ttu-id="9c367-145">natDestinationPort</span><span class="sxs-lookup"><span data-stu-id="9c367-145">natDestinationPort</span></span>|<span data-ttu-id="9c367-146">String</span><span class="sxs-lookup"><span data-stu-id="9c367-146">String</span></span>|<span data-ttu-id="9c367-147">Порт назначения перевода сетевых адресов.</span><span class="sxs-lookup"><span data-stu-id="9c367-147">Network Address Translation destination port.</span></span>|
|<span data-ttu-id="9c367-148">natSourceAddress</span><span class="sxs-lookup"><span data-stu-id="9c367-148">natSourceAddress</span></span>|<span data-ttu-id="9c367-149">String</span><span class="sxs-lookup"><span data-stu-id="9c367-149">String</span></span>|<span data-ttu-id="9c367-150">IP-адрес источника перевода сетевого адреса.</span><span class="sxs-lookup"><span data-stu-id="9c367-150">Network Address Translation source IP address.</span></span>|
|<span data-ttu-id="9c367-151">natSourcePort</span><span class="sxs-lookup"><span data-stu-id="9c367-151">natSourcePort</span></span>|<span data-ttu-id="9c367-152">String</span><span class="sxs-lookup"><span data-stu-id="9c367-152">String</span></span>|<span data-ttu-id="9c367-153">Порт источника перевода сетевых адресов.</span><span class="sxs-lookup"><span data-stu-id="9c367-153">Network Address Translation source port.</span></span>|
|<span data-ttu-id="9c367-154">протокол</span><span class="sxs-lookup"><span data-stu-id="9c367-154">protocol</span></span>|[<span data-ttu-id="9c367-155">securityNetworkProtocol</span><span class="sxs-lookup"><span data-stu-id="9c367-155">securityNetworkProtocol</span></span>](securitynetworkprotocol.md)|<span data-ttu-id="9c367-156">Сетевой протокол.</span><span class="sxs-lookup"><span data-stu-id="9c367-156">Network protocol.</span></span> <span data-ttu-id="9c367-157">Возможные значения: `unknown` `ip` , , `icmp` `igmp` `ggp` `ipv4` `tcp` `pup` `udp` `idp` `ipv6` `ipv6RoutingHeader` , `ipv6FragmentHeader` `ipSecEncapsulatingSecurityPayload` `ipSecAuthenticationHeader` `icmpV6` `ipv6NoNextHeader` `ipv6DestinationOptions` `nd` `raw` `ipx` `spx` `spxII` .</span><span class="sxs-lookup"><span data-stu-id="9c367-157">Possible values are: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd`, `raw`, `ipx`, `spx`, `spxII`.</span></span>|
|<span data-ttu-id="9c367-158">riskScore</span><span class="sxs-lookup"><span data-stu-id="9c367-158">riskScore</span></span>|<span data-ttu-id="9c367-159">String</span><span class="sxs-lookup"><span data-stu-id="9c367-159">String</span></span>|<span data-ttu-id="9c367-160">Оценка риска сетевого подключения поставщика сгенерирована и рассчитана.</span><span class="sxs-lookup"><span data-stu-id="9c367-160">Provider generated/calculated risk score of the network connection.</span></span> <span data-ttu-id="9c367-161">Рекомендуемый диапазон значений 0-1, который приравнивается к проценту.</span><span class="sxs-lookup"><span data-stu-id="9c367-161">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="9c367-162">sourceAddress</span><span class="sxs-lookup"><span data-stu-id="9c367-162">sourceAddress</span></span>|<span data-ttu-id="9c367-163">String</span><span class="sxs-lookup"><span data-stu-id="9c367-163">String</span></span>|<span data-ttu-id="9c367-164">IP-адрес источника (то есть происхождения) (сетевого подключения).</span><span class="sxs-lookup"><span data-stu-id="9c367-164">Source (i.e. origin) IP address (of the network connection).</span></span>|
|<span data-ttu-id="9c367-165">sourceLocation</span><span class="sxs-lookup"><span data-stu-id="9c367-165">sourceLocation</span></span>|<span data-ttu-id="9c367-166">String</span><span class="sxs-lookup"><span data-stu-id="9c367-166">String</span></span>|<span data-ttu-id="9c367-167">Расположение (по сопоставлению IP-адресов), связанное с источником сетевого подключения.</span><span class="sxs-lookup"><span data-stu-id="9c367-167">Location (by IP address mapping) associated with the source of a network connection.</span></span>|
|<span data-ttu-id="9c367-168">sourcePort</span><span class="sxs-lookup"><span data-stu-id="9c367-168">sourcePort</span></span>|<span data-ttu-id="9c367-169">String</span><span class="sxs-lookup"><span data-stu-id="9c367-169">String</span></span>|<span data-ttu-id="9c367-170">Ip-порт source (то есть происхождение) (сетевого подключения).</span><span class="sxs-lookup"><span data-stu-id="9c367-170">Source (i.e. origin) IP port (of the network connection).</span></span>|
|<span data-ttu-id="9c367-171">status</span><span class="sxs-lookup"><span data-stu-id="9c367-171">status</span></span>|<span data-ttu-id="9c367-172">connectionStatus</span><span class="sxs-lookup"><span data-stu-id="9c367-172">connectionStatus</span></span>|<span data-ttu-id="9c367-173">Состояние сетевого подключения.</span><span class="sxs-lookup"><span data-stu-id="9c367-173">Network connection status.</span></span> <span data-ttu-id="9c367-174">Возможные значения: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="9c367-174">Possible values are: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span></span>|
|<span data-ttu-id="9c367-175">urlParameters</span><span class="sxs-lookup"><span data-stu-id="9c367-175">urlParameters</span></span>|<span data-ttu-id="9c367-176">String</span><span class="sxs-lookup"><span data-stu-id="9c367-176">String</span></span>|<span data-ttu-id="9c367-177">Параметры (суффикс) URL-адреса назначения.</span><span class="sxs-lookup"><span data-stu-id="9c367-177">Parameters (suffix) of the destination URL.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9c367-178">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9c367-178">JSON representation</span></span>

<span data-ttu-id="9c367-179">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9c367-179">The following is a JSON representation of the resource.</span></span>

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

