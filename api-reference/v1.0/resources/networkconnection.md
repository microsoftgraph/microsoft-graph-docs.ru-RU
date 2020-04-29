---
title: Тип ресурса networkConnection
description: Содержит сведения о состоянии сетевого подключения, связанного с оповещением.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 86986178bc7104118dfb4db83ae43f7780307fe6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447369"
---
# <a name="networkconnection-resource-type"></a><span data-ttu-id="0a98c-103">Тип ресурса networkConnection</span><span class="sxs-lookup"><span data-stu-id="0a98c-103">networkConnection resource type</span></span>

<span data-ttu-id="0a98c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a98c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0a98c-105">Содержит сведения о состоянии сетевого подключения, связанного с оповещением.</span><span class="sxs-lookup"><span data-stu-id="0a98c-105">Contains stateful information about the network connection related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="0a98c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="0a98c-106">Properties</span></span>

| <span data-ttu-id="0a98c-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="0a98c-107">Property</span></span>   | <span data-ttu-id="0a98c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="0a98c-108">Type</span></span>|<span data-ttu-id="0a98c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0a98c-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0a98c-110">applicationName</span><span class="sxs-lookup"><span data-stu-id="0a98c-110">applicationName</span></span>|<span data-ttu-id="0a98c-111">String</span><span class="sxs-lookup"><span data-stu-id="0a98c-111">String</span></span>|<span data-ttu-id="0a98c-112">Имя приложения, управляющего сетевым подключением (например, Facebook, SMTP и т. д.).</span><span class="sxs-lookup"><span data-stu-id="0a98c-112">Name of the application managing the network connection (for example, Facebook, SMTP, etc.).</span></span>|
|<span data-ttu-id="0a98c-113">дестинатионаддресс</span><span class="sxs-lookup"><span data-stu-id="0a98c-113">destinationAddress</span></span>|<span data-ttu-id="0a98c-114">String</span><span class="sxs-lookup"><span data-stu-id="0a98c-114">String</span></span>|<span data-ttu-id="0a98c-115">Конечный IP-адрес (сетевого подключения).</span><span class="sxs-lookup"><span data-stu-id="0a98c-115">Destination IP address (of the network connection).</span></span>|
|<span data-ttu-id="0a98c-116">дестинатиондомаин</span><span class="sxs-lookup"><span data-stu-id="0a98c-116">destinationDomain</span></span>|<span data-ttu-id="0a98c-117">String</span><span class="sxs-lookup"><span data-stu-id="0a98c-117">String</span></span>|<span data-ttu-id="0a98c-118">Часть конечного домена, в которой находится конечный URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="0a98c-118">Destination domain portion of the destination URL.</span></span> <span data-ttu-id="0a98c-119">(например, "www.contoso.com").</span><span class="sxs-lookup"><span data-stu-id="0a98c-119">(for example 'www.contoso.com').</span></span>|
|<span data-ttu-id="0a98c-120">дестинатионпорт</span><span class="sxs-lookup"><span data-stu-id="0a98c-120">destinationPort</span></span>|<span data-ttu-id="0a98c-121">String</span><span class="sxs-lookup"><span data-stu-id="0a98c-121">String</span></span>|<span data-ttu-id="0a98c-122">Порт назначения (для сетевого подключения).</span><span class="sxs-lookup"><span data-stu-id="0a98c-122">Destination port (of the network connection).</span></span>|
|<span data-ttu-id="0a98c-123">дестинатионурл</span><span class="sxs-lookup"><span data-stu-id="0a98c-123">destinationUrl</span></span>|<span data-ttu-id="0a98c-124">String</span><span class="sxs-lookup"><span data-stu-id="0a98c-124">String</span></span>|<span data-ttu-id="0a98c-125">URL-адрес сетевого подключения/URI-строка — без параметров.</span><span class="sxs-lookup"><span data-stu-id="0a98c-125">Network connection URL/URI string - excluding parameters.</span></span> <span data-ttu-id="0a98c-126">(например, "www.contoso.com/products/default.html")</span><span class="sxs-lookup"><span data-stu-id="0a98c-126">(for example 'www.contoso.com/products/default.html')</span></span>|
|<span data-ttu-id="0a98c-127">direction</span><span class="sxs-lookup"><span data-stu-id="0a98c-127">direction</span></span>|<span data-ttu-id="0a98c-128">connectionDirection</span><span class="sxs-lookup"><span data-stu-id="0a98c-128">connectionDirection</span></span>|<span data-ttu-id="0a98c-129">Направление сетевого подключения.</span><span class="sxs-lookup"><span data-stu-id="0a98c-129">Network connection direction.</span></span> <span data-ttu-id="0a98c-130">Возможные значения: `unknown`, `inbound`, `outbound`.</span><span class="sxs-lookup"><span data-stu-id="0a98c-130">Possible values are: `unknown`, `inbound`, `outbound`.</span></span>|
|<span data-ttu-id="0a98c-131">домаинрегистереддатетиме</span><span class="sxs-lookup"><span data-stu-id="0a98c-131">domainRegisteredDateTime</span></span>|<span data-ttu-id="0a98c-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a98c-132">DateTimeOffset</span></span>|<span data-ttu-id="0a98c-133">Дата регистрации конечного домена.</span><span class="sxs-lookup"><span data-stu-id="0a98c-133">Date when the destination domain was registered.</span></span> <span data-ttu-id="0a98c-134">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="0a98c-134">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0a98c-135">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="0a98c-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="0a98c-136">локалднснаме</span><span class="sxs-lookup"><span data-stu-id="0a98c-136">localDnsName</span></span>|<span data-ttu-id="0a98c-137">String</span><span class="sxs-lookup"><span data-stu-id="0a98c-137">String</span></span>|<span data-ttu-id="0a98c-138">Локальное разрешение DNS-имен, отображаемое в локальном кэше DNS узла (например, на случай, если файл hosts был подделан).</span><span class="sxs-lookup"><span data-stu-id="0a98c-138">The local DNS name resolution as it appears in the host's local DNS cache (for example, in case the 'hosts' file was tampered with).</span></span>|
|<span data-ttu-id="0a98c-139">натдестинатионаддресс</span><span class="sxs-lookup"><span data-stu-id="0a98c-139">natDestinationAddress</span></span>|<span data-ttu-id="0a98c-140">String</span><span class="sxs-lookup"><span data-stu-id="0a98c-140">String</span></span>|<span data-ttu-id="0a98c-141">IP-адрес назначения преобразования сетевых адресов.</span><span class="sxs-lookup"><span data-stu-id="0a98c-141">Network Address Translation destination IP address.</span></span>|
|<span data-ttu-id="0a98c-142">натдестинатионпорт</span><span class="sxs-lookup"><span data-stu-id="0a98c-142">natDestinationPort</span></span>|<span data-ttu-id="0a98c-143">String</span><span class="sxs-lookup"><span data-stu-id="0a98c-143">String</span></span>|<span data-ttu-id="0a98c-144">Порт назначения преобразования сетевых адресов.</span><span class="sxs-lookup"><span data-stu-id="0a98c-144">Network Address Translation destination port.</span></span>|
|<span data-ttu-id="0a98c-145">натсаурцеаддресс</span><span class="sxs-lookup"><span data-stu-id="0a98c-145">natSourceAddress</span></span>|<span data-ttu-id="0a98c-146">String</span><span class="sxs-lookup"><span data-stu-id="0a98c-146">String</span></span>|<span data-ttu-id="0a98c-147">IP-адрес источника преобразования сетевых адресов.</span><span class="sxs-lookup"><span data-stu-id="0a98c-147">Network Address Translation source IP address.</span></span>|
|<span data-ttu-id="0a98c-148">натсаурцепорт</span><span class="sxs-lookup"><span data-stu-id="0a98c-148">natSourcePort</span></span>|<span data-ttu-id="0a98c-149">String</span><span class="sxs-lookup"><span data-stu-id="0a98c-149">String</span></span>|<span data-ttu-id="0a98c-150">Порт источника преобразования сетевых адресов.</span><span class="sxs-lookup"><span data-stu-id="0a98c-150">Network Address Translation source port.</span></span>|
|<span data-ttu-id="0a98c-151">Protocol</span><span class="sxs-lookup"><span data-stu-id="0a98c-151">protocol</span></span>|[<span data-ttu-id="0a98c-152">securityNetworkProtocol</span><span class="sxs-lookup"><span data-stu-id="0a98c-152">securityNetworkProtocol</span></span>](securitynetworkprotocol.md)|<span data-ttu-id="0a98c-153">Сетевой протокол.</span><span class="sxs-lookup"><span data-stu-id="0a98c-153">Network protocol.</span></span> <span data-ttu-id="0a98c-154">Возможные `unknown`значения:, `ip`, `icmp`, `igmp` `ggp` `ipv4` `tcp` `ipSecEncapsulatingSecurityPayload` `ipSecAuthenticationHeader` `icmpV6` `ipv6NoNextHeader` `ipv6DestinationOptions` `nd` `raw` `ipx` `spx` `spxII`,,,,,,, `ipv6FragmentHeader`,,,,,,,,,,,,,,,,,,. `pup` `udp` `idp` `ipv6` `ipv6RoutingHeader`</span><span class="sxs-lookup"><span data-stu-id="0a98c-154">Possible values are: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd`, `raw`, `ipx`, `spx`, `spxII`.</span></span>|
|<span data-ttu-id="0a98c-155">riskScore</span><span class="sxs-lookup"><span data-stu-id="0a98c-155">riskScore</span></span>|<span data-ttu-id="0a98c-156">String</span><span class="sxs-lookup"><span data-stu-id="0a98c-156">String</span></span>|<span data-ttu-id="0a98c-157">Созданный поставщиком/вычисляемый показатель риска для сетевого подключения.</span><span class="sxs-lookup"><span data-stu-id="0a98c-157">Provider generated/calculated risk score of the network connection.</span></span> <span data-ttu-id="0a98c-158">Рекомендуемый диапазон значений 0-1, указывающий на процентное соотношение.</span><span class="sxs-lookup"><span data-stu-id="0a98c-158">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="0a98c-159">саурцеаддресс</span><span class="sxs-lookup"><span data-stu-id="0a98c-159">sourceAddress</span></span>|<span data-ttu-id="0a98c-160">String</span><span class="sxs-lookup"><span data-stu-id="0a98c-160">String</span></span>|<span data-ttu-id="0a98c-161">Источник (то есть источник) IP-адрес сетевого подключения.</span><span class="sxs-lookup"><span data-stu-id="0a98c-161">Source (i.e. origin) IP address (of the network connection).</span></span>|
|<span data-ttu-id="0a98c-162">саурцепорт</span><span class="sxs-lookup"><span data-stu-id="0a98c-162">sourcePort</span></span>|<span data-ttu-id="0a98c-163">String</span><span class="sxs-lookup"><span data-stu-id="0a98c-163">String</span></span>|<span data-ttu-id="0a98c-164">Исходный (то есть источник) IP-порт (сетевого подключения).</span><span class="sxs-lookup"><span data-stu-id="0a98c-164">Source (i.e. origin) IP port (of the network connection).</span></span>|
|<span data-ttu-id="0a98c-165">status</span><span class="sxs-lookup"><span data-stu-id="0a98c-165">status</span></span>|<span data-ttu-id="0a98c-166">connectionStatus</span><span class="sxs-lookup"><span data-stu-id="0a98c-166">connectionStatus</span></span>|<span data-ttu-id="0a98c-167">Состояние сетевого подключения.</span><span class="sxs-lookup"><span data-stu-id="0a98c-167">Network connection status.</span></span> <span data-ttu-id="0a98c-168">Возможные значения: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="0a98c-168">Possible values are: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span></span>|
|<span data-ttu-id="0a98c-169">урлпараметерс</span><span class="sxs-lookup"><span data-stu-id="0a98c-169">urlParameters</span></span>|<span data-ttu-id="0a98c-170">String</span><span class="sxs-lookup"><span data-stu-id="0a98c-170">String</span></span>|<span data-ttu-id="0a98c-171">Параметры (суффикс) конечного URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="0a98c-171">Parameters (suffix) of the destination URL.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0a98c-172">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0a98c-172">JSON representation</span></span>

<span data-ttu-id="0a98c-173">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0a98c-173">The following is a JSON representation of the resource.</span></span>

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
