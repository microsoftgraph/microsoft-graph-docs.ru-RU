---
title: Тип ресурса networkConnection
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: c111082fe0b9a2f2090de3fe3abb71a96fd4a80d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026588"
---
# <a name="networkconnection-resource-type"></a><span data-ttu-id="ffe4f-104">Тип ресурса networkConnection</span><span class="sxs-lookup"><span data-stu-id="ffe4f-104">networkConnection resource type</span></span>

<span data-ttu-id="ffe4f-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ffe4f-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ffe4f-106">Содержит сведения о состоянии сетевого подключения, связанного с оповещением.</span><span class="sxs-lookup"><span data-stu-id="ffe4f-106">Contains stateful information about the network connection related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="ffe4f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ffe4f-107">Properties</span></span>

| <span data-ttu-id="ffe4f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ffe4f-108">Property</span></span>   | <span data-ttu-id="ffe4f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ffe4f-109">Type</span></span>|<span data-ttu-id="ffe4f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ffe4f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ffe4f-111">applicationName</span><span class="sxs-lookup"><span data-stu-id="ffe4f-111">applicationName</span></span>|<span data-ttu-id="ffe4f-112">String</span><span class="sxs-lookup"><span data-stu-id="ffe4f-112">String</span></span>|<span data-ttu-id="ffe4f-113">Имя приложения, управляющего сетевым подключением (например, Facebook, SMTP и т. д.).</span><span class="sxs-lookup"><span data-stu-id="ffe4f-113">Name of the application managing the network connection (for example, Facebook, SMTP, etc.).</span></span>|
|<span data-ttu-id="ffe4f-114">дестинатионаддресс</span><span class="sxs-lookup"><span data-stu-id="ffe4f-114">destinationAddress</span></span>|<span data-ttu-id="ffe4f-115">String</span><span class="sxs-lookup"><span data-stu-id="ffe4f-115">String</span></span>|<span data-ttu-id="ffe4f-116">Конечный IP-адрес (сетевого подключения).</span><span class="sxs-lookup"><span data-stu-id="ffe4f-116">Destination IP address (of the network connection).</span></span>|
|<span data-ttu-id="ffe4f-117">дестинатиондомаин</span><span class="sxs-lookup"><span data-stu-id="ffe4f-117">destinationDomain</span></span>|<span data-ttu-id="ffe4f-118">String</span><span class="sxs-lookup"><span data-stu-id="ffe4f-118">String</span></span>|<span data-ttu-id="ffe4f-119">Часть конечного домена, в которой находится конечный URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="ffe4f-119">Destination domain portion of the destination URL.</span></span> <span data-ttu-id="ffe4f-120">(например, "www.contoso.com").</span><span class="sxs-lookup"><span data-stu-id="ffe4f-120">(for example 'www.contoso.com').</span></span>|
|<span data-ttu-id="ffe4f-121">дестинатионлокатион</span><span class="sxs-lookup"><span data-stu-id="ffe4f-121">destinationLocation</span></span>|<span data-ttu-id="ffe4f-122">String</span><span class="sxs-lookup"><span data-stu-id="ffe4f-122">String</span></span>|<span data-ttu-id="ffe4f-123">Расположение (по сопоставлению IP-адресов), связанное с назначением сетевого подключения.</span><span class="sxs-lookup"><span data-stu-id="ffe4f-123">Location (by IP address mapping) associated with the destination of a network connection.</span></span>|
|<span data-ttu-id="ffe4f-124">дестинатионпорт</span><span class="sxs-lookup"><span data-stu-id="ffe4f-124">destinationPort</span></span>|<span data-ttu-id="ffe4f-125">String</span><span class="sxs-lookup"><span data-stu-id="ffe4f-125">String</span></span>|<span data-ttu-id="ffe4f-126">Порт назначения (для сетевого подключения).</span><span class="sxs-lookup"><span data-stu-id="ffe4f-126">Destination port (of the network connection).</span></span>|
|<span data-ttu-id="ffe4f-127">дестинатионурл</span><span class="sxs-lookup"><span data-stu-id="ffe4f-127">destinationUrl</span></span>|<span data-ttu-id="ffe4f-128">String</span><span class="sxs-lookup"><span data-stu-id="ffe4f-128">String</span></span>|<span data-ttu-id="ffe4f-129">URL-адрес сетевого подключения/URI-строка — без параметров.</span><span class="sxs-lookup"><span data-stu-id="ffe4f-129">Network connection URL/URI string - excluding parameters.</span></span> <span data-ttu-id="ffe4f-130">(например, "www.contoso.com/products/default.html")</span><span class="sxs-lookup"><span data-stu-id="ffe4f-130">(for example 'www.contoso.com/products/default.html')</span></span>|
|<span data-ttu-id="ffe4f-131">direction</span><span class="sxs-lookup"><span data-stu-id="ffe4f-131">direction</span></span>|<span data-ttu-id="ffe4f-132">connectionDirection</span><span class="sxs-lookup"><span data-stu-id="ffe4f-132">connectionDirection</span></span>|<span data-ttu-id="ffe4f-133">Направление сетевого подключения.</span><span class="sxs-lookup"><span data-stu-id="ffe4f-133">Network connection direction.</span></span> <span data-ttu-id="ffe4f-134">Возможные значения: `unknown`, `inbound`, `outbound`.</span><span class="sxs-lookup"><span data-stu-id="ffe4f-134">Possible values are: `unknown`, `inbound`, `outbound`.</span></span>|
|<span data-ttu-id="ffe4f-135">домаинрегистереддатетиме</span><span class="sxs-lookup"><span data-stu-id="ffe4f-135">domainRegisteredDateTime</span></span>|<span data-ttu-id="ffe4f-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ffe4f-136">DateTimeOffset</span></span>|<span data-ttu-id="ffe4f-137">Дата регистрации конечного домена.</span><span class="sxs-lookup"><span data-stu-id="ffe4f-137">Date when the destination domain was registered.</span></span> <span data-ttu-id="ffe4f-138">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="ffe4f-138">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ffe4f-139">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="ffe4f-139">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="ffe4f-140">локалднснаме</span><span class="sxs-lookup"><span data-stu-id="ffe4f-140">localDnsName</span></span>|<span data-ttu-id="ffe4f-141">String</span><span class="sxs-lookup"><span data-stu-id="ffe4f-141">String</span></span>|<span data-ttu-id="ffe4f-142">Локальное разрешение DNS-имен, отображаемое в локальном кэше DNS узла (например, на случай, если файл hosts был подделан).</span><span class="sxs-lookup"><span data-stu-id="ffe4f-142">The local DNS name resolution as it appears in the host's local DNS cache (for example, in case the 'hosts' file was tampered with).</span></span>|
|<span data-ttu-id="ffe4f-143">натдестинатионаддресс</span><span class="sxs-lookup"><span data-stu-id="ffe4f-143">natDestinationAddress</span></span>|<span data-ttu-id="ffe4f-144">String</span><span class="sxs-lookup"><span data-stu-id="ffe4f-144">String</span></span>|<span data-ttu-id="ffe4f-145">IP-адрес назначения преобразования сетевых адресов.</span><span class="sxs-lookup"><span data-stu-id="ffe4f-145">Network Address Translation destination IP address.</span></span>|
|<span data-ttu-id="ffe4f-146">натдестинатионпорт</span><span class="sxs-lookup"><span data-stu-id="ffe4f-146">natDestinationPort</span></span>|<span data-ttu-id="ffe4f-147">String</span><span class="sxs-lookup"><span data-stu-id="ffe4f-147">String</span></span>|<span data-ttu-id="ffe4f-148">Порт назначения преобразования сетевых адресов.</span><span class="sxs-lookup"><span data-stu-id="ffe4f-148">Network Address Translation destination port.</span></span>|
|<span data-ttu-id="ffe4f-149">натсаурцеаддресс</span><span class="sxs-lookup"><span data-stu-id="ffe4f-149">natSourceAddress</span></span>|<span data-ttu-id="ffe4f-150">String</span><span class="sxs-lookup"><span data-stu-id="ffe4f-150">String</span></span>|<span data-ttu-id="ffe4f-151">IP-адрес источника преобразования сетевых адресов.</span><span class="sxs-lookup"><span data-stu-id="ffe4f-151">Network Address Translation source IP address.</span></span>|
|<span data-ttu-id="ffe4f-152">натсаурцепорт</span><span class="sxs-lookup"><span data-stu-id="ffe4f-152">natSourcePort</span></span>|<span data-ttu-id="ffe4f-153">String</span><span class="sxs-lookup"><span data-stu-id="ffe4f-153">String</span></span>|<span data-ttu-id="ffe4f-154">Порт источника преобразования сетевых адресов.</span><span class="sxs-lookup"><span data-stu-id="ffe4f-154">Network Address Translation source port.</span></span>|
|<span data-ttu-id="ffe4f-155">Protocol</span><span class="sxs-lookup"><span data-stu-id="ffe4f-155">protocol</span></span>|<span data-ttu-id="ffe4f-156">securityNetworkProtocol</span><span class="sxs-lookup"><span data-stu-id="ffe4f-156">securityNetworkProtocol</span></span>|<span data-ttu-id="ffe4f-157">Сетевой протокол.</span><span class="sxs-lookup"><span data-stu-id="ffe4f-157">Network protocol.</span></span> <span data-ttu-id="ffe4f-158">Возможные значения:,,,,,,,,,,, `unknown` `ip` `icmp` `igmp` `ggp` `ipv4` `tcp` `pup` `udp` `idp` `ipv6` `ipv6RoutingHeader` `ipv6FragmentHeader` , `ipSecEncapsulatingSecurityPayload` , `ipSecAuthenticationHeader` , `icmpV6` `ipv6NoNextHeader` `ipv6DestinationOptions` `nd` `raw` `ipx` `spx` `spxII` ,,,,,,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="ffe4f-158">Possible values are: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd`, `raw`, `ipx`, `spx`, `spxII`.</span></span>|
|<span data-ttu-id="ffe4f-159">riskScore</span><span class="sxs-lookup"><span data-stu-id="ffe4f-159">riskScore</span></span>|<span data-ttu-id="ffe4f-160">String</span><span class="sxs-lookup"><span data-stu-id="ffe4f-160">String</span></span>|<span data-ttu-id="ffe4f-161">Созданный поставщиком/вычисляемый показатель риска для сетевого подключения.</span><span class="sxs-lookup"><span data-stu-id="ffe4f-161">Provider generated/calculated risk score of the network connection.</span></span> <span data-ttu-id="ffe4f-162">Рекомендуемый диапазон значений 0-1, указывающий на процентное соотношение.</span><span class="sxs-lookup"><span data-stu-id="ffe4f-162">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="ffe4f-163">саурцеаддресс</span><span class="sxs-lookup"><span data-stu-id="ffe4f-163">sourceAddress</span></span>|<span data-ttu-id="ffe4f-164">String</span><span class="sxs-lookup"><span data-stu-id="ffe4f-164">String</span></span>|<span data-ttu-id="ffe4f-165">Источник (то есть источник) IP-адрес сетевого подключения.</span><span class="sxs-lookup"><span data-stu-id="ffe4f-165">Source (i.e. origin) IP address (of the network connection).</span></span>|
|<span data-ttu-id="ffe4f-166">sourceLocation</span><span class="sxs-lookup"><span data-stu-id="ffe4f-166">sourceLocation</span></span>|<span data-ttu-id="ffe4f-167">String</span><span class="sxs-lookup"><span data-stu-id="ffe4f-167">String</span></span>|<span data-ttu-id="ffe4f-168">Расположение (по сопоставлению IP-адресов), связанное с источником сетевого подключения.</span><span class="sxs-lookup"><span data-stu-id="ffe4f-168">Location (by IP address mapping) associated with the source of a network connection.</span></span>|
|<span data-ttu-id="ffe4f-169">саурцепорт</span><span class="sxs-lookup"><span data-stu-id="ffe4f-169">sourcePort</span></span>|<span data-ttu-id="ffe4f-170">String</span><span class="sxs-lookup"><span data-stu-id="ffe4f-170">String</span></span>|<span data-ttu-id="ffe4f-171">Исходный (то есть источник) IP-порт (сетевого подключения).</span><span class="sxs-lookup"><span data-stu-id="ffe4f-171">Source (i.e. origin) IP port (of the network connection).</span></span>|
|<span data-ttu-id="ffe4f-172">status</span><span class="sxs-lookup"><span data-stu-id="ffe4f-172">status</span></span>|<span data-ttu-id="ffe4f-173">connectionStatus</span><span class="sxs-lookup"><span data-stu-id="ffe4f-173">connectionStatus</span></span>|<span data-ttu-id="ffe4f-174">Состояние сетевого подключения.</span><span class="sxs-lookup"><span data-stu-id="ffe4f-174">Network connection status.</span></span> <span data-ttu-id="ffe4f-175">Возможные значения: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="ffe4f-175">Possible values are: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span></span>|
|<span data-ttu-id="ffe4f-176">урлпараметерс</span><span class="sxs-lookup"><span data-stu-id="ffe4f-176">urlParameters</span></span>|<span data-ttu-id="ffe4f-177">String</span><span class="sxs-lookup"><span data-stu-id="ffe4f-177">String</span></span>|<span data-ttu-id="ffe4f-178">Параметры (суффикс) конечного URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="ffe4f-178">Parameters (suffix) of the destination URL.</span></span>|

### <a name="securitynetworkprotocol-values"></a><span data-ttu-id="ffe4f-179">значения Секуритинетворкпротокол</span><span class="sxs-lookup"><span data-stu-id="ffe4f-179">securityNetworkProtocol values</span></span>

|<span data-ttu-id="ffe4f-180">Элемент</span><span class="sxs-lookup"><span data-stu-id="ffe4f-180">Member</span></span>|<span data-ttu-id="ffe4f-181">Значение</span><span class="sxs-lookup"><span data-stu-id="ffe4f-181">Value</span></span>|<span data-ttu-id="ffe4f-182">Описание</span><span class="sxs-lookup"><span data-stu-id="ffe4f-182">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ffe4f-183">unknown</span><span class="sxs-lookup"><span data-stu-id="ffe4f-183">unknown</span></span>|<span data-ttu-id="ffe4f-184">–1</span><span class="sxs-lookup"><span data-stu-id="ffe4f-184">-1</span></span>|<span data-ttu-id="ffe4f-185">Неизвестный протокол.</span><span class="sxs-lookup"><span data-stu-id="ffe4f-185">Unknown protocol.</span></span>|
|<span data-ttu-id="ffe4f-186">см</span><span class="sxs-lookup"><span data-stu-id="ffe4f-186">ip</span></span>|<span data-ttu-id="ffe4f-187">нуль</span><span class="sxs-lookup"><span data-stu-id="ffe4f-187">0</span></span>|<span data-ttu-id="ffe4f-188">Протокол IP.</span><span class="sxs-lookup"><span data-stu-id="ffe4f-188">Internet Protocol.</span></span>|
|<span data-ttu-id="ffe4f-189">полученных</span><span class="sxs-lookup"><span data-stu-id="ffe4f-189">icmp</span></span>|<span data-ttu-id="ffe4f-190">1 </span><span class="sxs-lookup"><span data-stu-id="ffe4f-190">1</span></span>| <span data-ttu-id="ffe4f-191">Протокол управления сообщениями в Интернете.</span><span class="sxs-lookup"><span data-stu-id="ffe4f-191">Internet Control Message Protocol.</span></span>|
|<span data-ttu-id="ffe4f-192">режимы</span><span class="sxs-lookup"><span data-stu-id="ffe4f-192">igmp</span></span>|<span data-ttu-id="ffe4f-193">2 </span><span class="sxs-lookup"><span data-stu-id="ffe4f-193">2</span></span>| <span data-ttu-id="ffe4f-194">Протокол управления группами Интернет.</span><span class="sxs-lookup"><span data-stu-id="ffe4f-194">Internet Group Management Protocol.</span></span>|
|<span data-ttu-id="ffe4f-195">ггп</span><span class="sxs-lookup"><span data-stu-id="ffe4f-195">ggp</span></span>|<span data-ttu-id="ffe4f-196">4</span><span class="sxs-lookup"><span data-stu-id="ffe4f-196">3</span></span>| <span data-ttu-id="ffe4f-197">Протокол шлюза для шлюза.</span><span class="sxs-lookup"><span data-stu-id="ffe4f-197">Gateway To Gateway Protocol.</span></span>|
|<span data-ttu-id="ffe4f-198">IPv4</span><span class="sxs-lookup"><span data-stu-id="ffe4f-198">ipv4</span></span>|<span data-ttu-id="ffe4f-199">4 </span><span class="sxs-lookup"><span data-stu-id="ffe4f-199">4</span></span>| <span data-ttu-id="ffe4f-200">Протокол Интернета версии 4.</span><span class="sxs-lookup"><span data-stu-id="ffe4f-200">Internet Protocol version 4.</span></span>|
|<span data-ttu-id="ffe4f-201">tcp</span><span class="sxs-lookup"><span data-stu-id="ffe4f-201">tcp</span></span>|<span data-ttu-id="ffe4f-202">6 </span><span class="sxs-lookup"><span data-stu-id="ffe4f-202">6</span></span>| <span data-ttu-id="ffe4f-203">Протокол управления передачей.</span><span class="sxs-lookup"><span data-stu-id="ffe4f-203">Transmission Control Protocol.</span></span>|
|<span data-ttu-id="ffe4f-204">пуп</span><span class="sxs-lookup"><span data-stu-id="ffe4f-204">pup</span></span>|<span data-ttu-id="ffe4f-205">12 </span><span class="sxs-lookup"><span data-stu-id="ffe4f-205">12</span></span>| <span data-ttu-id="ffe4f-206">Протокол универсальных пакетов парк.</span><span class="sxs-lookup"><span data-stu-id="ffe4f-206">PARC Universal Packet Protocol.</span></span>|
|<span data-ttu-id="ffe4f-207">протокола</span><span class="sxs-lookup"><span data-stu-id="ffe4f-207">udp</span></span>|<span data-ttu-id="ffe4f-208">17 </span><span class="sxs-lookup"><span data-stu-id="ffe4f-208">17</span></span>| <span data-ttu-id="ffe4f-209">Протокол датаграммы пользователя.</span><span class="sxs-lookup"><span data-stu-id="ffe4f-209">User Datagram Protocol.</span></span>|
|<span data-ttu-id="ffe4f-210">IDP</span><span class="sxs-lookup"><span data-stu-id="ffe4f-210">idp</span></span>|<span data-ttu-id="ffe4f-211">22</span><span class="sxs-lookup"><span data-stu-id="ffe4f-211">22</span></span>| <span data-ttu-id="ffe4f-212">Протокол датаграмм через Интернет.</span><span class="sxs-lookup"><span data-stu-id="ffe4f-212">Internet Datagram Protocol.</span></span>|
|<span data-ttu-id="ffe4f-213">поддерживающ</span><span class="sxs-lookup"><span data-stu-id="ffe4f-213">ipv6</span></span>|<span data-ttu-id="ffe4f-214">41</span><span class="sxs-lookup"><span data-stu-id="ffe4f-214">41</span></span>| <span data-ttu-id="ffe4f-215">Протокол IP версии 6 (IPv6).</span><span class="sxs-lookup"><span data-stu-id="ffe4f-215">Internet Protocol version 6 (ipv6).</span></span>|
|<span data-ttu-id="ffe4f-216">ipv6RoutingHeader</span><span class="sxs-lookup"><span data-stu-id="ffe4f-216">ipv6RoutingHeader</span></span>|<span data-ttu-id="ffe4f-217">43</span><span class="sxs-lookup"><span data-stu-id="ffe4f-217">43</span></span>| <span data-ttu-id="ffe4f-218">заголовок маршрутизации IPv6.</span><span class="sxs-lookup"><span data-stu-id="ffe4f-218">ipv6 Routing header.</span></span>|
|<span data-ttu-id="ffe4f-219">ipv6FragmentHeader</span><span class="sxs-lookup"><span data-stu-id="ffe4f-219">ipv6FragmentHeader</span></span>|<span data-ttu-id="ffe4f-220">44</span><span class="sxs-lookup"><span data-stu-id="ffe4f-220">44</span></span>| <span data-ttu-id="ffe4f-221">заголовок фрагмента IPv6.</span><span class="sxs-lookup"><span data-stu-id="ffe4f-221">ipv6 Fragment header.</span></span>|
|<span data-ttu-id="ffe4f-222">ипсеценкапсулатингсекуритипайлоад</span><span class="sxs-lookup"><span data-stu-id="ffe4f-222">ipSecEncapsulatingSecurityPayload</span></span>|<span data-ttu-id="ffe4f-223">50</span><span class="sxs-lookup"><span data-stu-id="ffe4f-223">50</span></span>| <span data-ttu-id="ffe4f-224">заголовок полезных данных безопасности, включающий IPv6.</span><span class="sxs-lookup"><span data-stu-id="ffe4f-224">ipv6 Encapsulating Security Payload header.</span></span>|
|<span data-ttu-id="ffe4f-225">ипсекаусентикатионхеадер</span><span class="sxs-lookup"><span data-stu-id="ffe4f-225">ipSecAuthenticationHeader</span></span>|<span data-ttu-id="ffe4f-226">51</span><span class="sxs-lookup"><span data-stu-id="ffe4f-226">51</span></span>| <span data-ttu-id="ffe4f-227">заголовок проверки подлинности IPv6.</span><span class="sxs-lookup"><span data-stu-id="ffe4f-227">ipv6 Authentication header.</span></span>|
|<span data-ttu-id="ffe4f-228">icmpV6</span><span class="sxs-lookup"><span data-stu-id="ffe4f-228">icmpV6</span></span>|<span data-ttu-id="ffe4f-229">58</span><span class="sxs-lookup"><span data-stu-id="ffe4f-229">58</span></span>| <span data-ttu-id="ffe4f-230">Протокол управления сообщениями в Интернете для IPv6.</span><span class="sxs-lookup"><span data-stu-id="ffe4f-230">Internet Control Message Protocol for ipv6.</span></span>|
|<span data-ttu-id="ffe4f-231">ipv6NoNextHeader</span><span class="sxs-lookup"><span data-stu-id="ffe4f-231">ipv6NoNextHeader</span></span>|<span data-ttu-id="ffe4f-232">59</span><span class="sxs-lookup"><span data-stu-id="ffe4f-232">59</span></span>| <span data-ttu-id="ffe4f-233">IPv6: следующий заголовок отсутствует.</span><span class="sxs-lookup"><span data-stu-id="ffe4f-233">ipv6 No next header.</span></span>|
|<span data-ttu-id="ffe4f-234">ipv6DestinationOptions</span><span class="sxs-lookup"><span data-stu-id="ffe4f-234">ipv6DestinationOptions</span></span>|<span data-ttu-id="ffe4f-235">60</span><span class="sxs-lookup"><span data-stu-id="ffe4f-235">60</span></span>| <span data-ttu-id="ffe4f-236">заголовок параметров назначения IPv6.</span><span class="sxs-lookup"><span data-stu-id="ffe4f-236">ipv6 Destination Options header.</span></span>|
|<span data-ttu-id="ffe4f-237">этаже</span><span class="sxs-lookup"><span data-stu-id="ffe4f-237">nd</span></span>|<span data-ttu-id="ffe4f-238">77</span><span class="sxs-lookup"><span data-stu-id="ffe4f-238">77</span></span>| <span data-ttu-id="ffe4f-239">Протокол сетевого диска (неофициальный).</span><span class="sxs-lookup"><span data-stu-id="ffe4f-239">Net Disk Protocol (unofficial).</span></span>|
|<span data-ttu-id="ffe4f-240">RAW</span><span class="sxs-lookup"><span data-stu-id="ffe4f-240">raw</span></span>|<span data-ttu-id="ffe4f-241">255</span><span class="sxs-lookup"><span data-stu-id="ffe4f-241">255</span></span>| <span data-ttu-id="ffe4f-242">Протокол IP-пакетов RAW.</span><span class="sxs-lookup"><span data-stu-id="ffe4f-242">Raw IP packet protocol.</span></span>|
|<span data-ttu-id="ffe4f-243">x</span><span class="sxs-lookup"><span data-stu-id="ffe4f-243">ipx</span></span>|<span data-ttu-id="ffe4f-244">1000</span><span class="sxs-lookup"><span data-stu-id="ffe4f-244">1000</span></span>| <span data-ttu-id="ffe4f-245">Протокол обмена пакетами в Интернете.</span><span class="sxs-lookup"><span data-stu-id="ffe4f-245">Internet Packet Exchange Protocol.</span></span>|
|<span data-ttu-id="ffe4f-246">возмож</span><span class="sxs-lookup"><span data-stu-id="ffe4f-246">spx</span></span>|<span data-ttu-id="ffe4f-247">1256</span><span class="sxs-lookup"><span data-stu-id="ffe4f-247">1256</span></span>| <span data-ttu-id="ffe4f-248">Последовательный протокол обмена пакетами.</span><span class="sxs-lookup"><span data-stu-id="ffe4f-248">Sequenced Packet Exchange protocol.</span></span>|
|<span data-ttu-id="ffe4f-249">спксии</span><span class="sxs-lookup"><span data-stu-id="ffe4f-249">spxII</span></span>|<span data-ttu-id="ffe4f-250">1257</span><span class="sxs-lookup"><span data-stu-id="ffe4f-250">1257</span></span>| <span data-ttu-id="ffe4f-251">Последовательный протокол обмена пакетами версии 2.</span><span class="sxs-lookup"><span data-stu-id="ffe4f-251">Sequenced Packet Exchange version 2 protocol.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ffe4f-252">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ffe4f-252">JSON representation</span></span>

<span data-ttu-id="ffe4f-253">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ffe4f-253">The following is a JSON representation of the resource.</span></span>

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
  "destinationLocation": "String",
  "destinationPort": "String",
  "destinationUrl": "String",
  "direction": "String",
  "domainRegisteredDateTime": "String (timestamp)",
  "localDnsName": "String",
  "natDestinationAddress": "String",
  "natDestinationPort": "String",
  "natSourceAddress": "String",
  "natSourcePort": "String",
  "protocol": "string",
  "riskScore": "String",
  "sourceAddress": "String",
  "sourceLocation": "String",
  "sourcePort": "String",
  "status": "String",
  "urlParameters": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "networkConnection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


