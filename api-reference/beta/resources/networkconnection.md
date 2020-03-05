---
title: Тип ресурса networkConnection
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: c587d9d6e11354a136948bbbf37565e42e0bb678
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522584"
---
# <a name="networkconnection-resource-type"></a><span data-ttu-id="5c669-104">Тип ресурса networkConnection</span><span class="sxs-lookup"><span data-stu-id="5c669-104">networkConnection resource type</span></span>

<span data-ttu-id="5c669-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5c669-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c669-106">Содержит сведения о состоянии сетевого подключения, связанного с оповещением.</span><span class="sxs-lookup"><span data-stu-id="5c669-106">Contains stateful information about the network connection related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="5c669-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5c669-107">Properties</span></span>

| <span data-ttu-id="5c669-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="5c669-108">Property</span></span>   | <span data-ttu-id="5c669-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5c669-109">Type</span></span>|<span data-ttu-id="5c669-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5c669-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5c669-111">applicationName</span><span class="sxs-lookup"><span data-stu-id="5c669-111">applicationName</span></span>|<span data-ttu-id="5c669-112">String</span><span class="sxs-lookup"><span data-stu-id="5c669-112">String</span></span>|<span data-ttu-id="5c669-113">Имя приложения, управляющего сетевым подключением (например, Facebook, SMTP и т. д.).</span><span class="sxs-lookup"><span data-stu-id="5c669-113">Name of the application managing the network connection (for example, Facebook, SMTP, etc.).</span></span>|
|<span data-ttu-id="5c669-114">дестинатионаддресс</span><span class="sxs-lookup"><span data-stu-id="5c669-114">destinationAddress</span></span>|<span data-ttu-id="5c669-115">String</span><span class="sxs-lookup"><span data-stu-id="5c669-115">String</span></span>|<span data-ttu-id="5c669-116">Конечный IP-адрес (сетевого подключения).</span><span class="sxs-lookup"><span data-stu-id="5c669-116">Destination IP address (of the network connection).</span></span>|
|<span data-ttu-id="5c669-117">дестинатиондомаин</span><span class="sxs-lookup"><span data-stu-id="5c669-117">destinationDomain</span></span>|<span data-ttu-id="5c669-118">String</span><span class="sxs-lookup"><span data-stu-id="5c669-118">String</span></span>|<span data-ttu-id="5c669-119">Часть конечного домена, в которой находится конечный URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="5c669-119">Destination domain portion of the destination URL.</span></span> <span data-ttu-id="5c669-120">(например, "www.contoso.com").</span><span class="sxs-lookup"><span data-stu-id="5c669-120">(for example 'www.contoso.com').</span></span>|
|<span data-ttu-id="5c669-121">дестинатионпорт</span><span class="sxs-lookup"><span data-stu-id="5c669-121">destinationPort</span></span>|<span data-ttu-id="5c669-122">String</span><span class="sxs-lookup"><span data-stu-id="5c669-122">String</span></span>|<span data-ttu-id="5c669-123">Порт назначения (для сетевого подключения).</span><span class="sxs-lookup"><span data-stu-id="5c669-123">Destination port (of the network connection).</span></span>|
|<span data-ttu-id="5c669-124">дестинатионурл</span><span class="sxs-lookup"><span data-stu-id="5c669-124">destinationUrl</span></span>|<span data-ttu-id="5c669-125">String</span><span class="sxs-lookup"><span data-stu-id="5c669-125">String</span></span>|<span data-ttu-id="5c669-126">URL-адрес сетевого подключения/URI-строка — без параметров.</span><span class="sxs-lookup"><span data-stu-id="5c669-126">Network connection URL/URI string - excluding parameters.</span></span> <span data-ttu-id="5c669-127">(например, "www.contoso.com/products/default.html")</span><span class="sxs-lookup"><span data-stu-id="5c669-127">(for example 'www.contoso.com/products/default.html')</span></span>|
|<span data-ttu-id="5c669-128">direction</span><span class="sxs-lookup"><span data-stu-id="5c669-128">direction</span></span>|<span data-ttu-id="5c669-129">connectionDirection</span><span class="sxs-lookup"><span data-stu-id="5c669-129">connectionDirection</span></span>|<span data-ttu-id="5c669-130">Направление сетевого подключения.</span><span class="sxs-lookup"><span data-stu-id="5c669-130">Network connection direction.</span></span> <span data-ttu-id="5c669-131">Возможные значения: `unknown`, `inbound`, `outbound`.</span><span class="sxs-lookup"><span data-stu-id="5c669-131">Possible values are: `unknown`, `inbound`, `outbound`.</span></span>|
|<span data-ttu-id="5c669-132">домаинрегистереддатетиме</span><span class="sxs-lookup"><span data-stu-id="5c669-132">domainRegisteredDateTime</span></span>|<span data-ttu-id="5c669-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c669-133">DateTimeOffset</span></span>|<span data-ttu-id="5c669-134">Дата регистрации конечного домена.</span><span class="sxs-lookup"><span data-stu-id="5c669-134">Date when the destination domain was registered.</span></span> <span data-ttu-id="5c669-135">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="5c669-135">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5c669-136">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="5c669-136">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="5c669-137">локалднснаме</span><span class="sxs-lookup"><span data-stu-id="5c669-137">localDnsName</span></span>|<span data-ttu-id="5c669-138">String</span><span class="sxs-lookup"><span data-stu-id="5c669-138">String</span></span>|<span data-ttu-id="5c669-139">Локальное разрешение DNS-имен, отображаемое в локальном кэше DNS узла (например, на случай, если файл hosts был подделан).</span><span class="sxs-lookup"><span data-stu-id="5c669-139">The local DNS name resolution as it appears in the host's local DNS cache (for example, in case the 'hosts' file was tampered with).</span></span>|
|<span data-ttu-id="5c669-140">натдестинатионаддресс</span><span class="sxs-lookup"><span data-stu-id="5c669-140">natDestinationAddress</span></span>|<span data-ttu-id="5c669-141">String</span><span class="sxs-lookup"><span data-stu-id="5c669-141">String</span></span>|<span data-ttu-id="5c669-142">IP-адрес назначения преобразования сетевых адресов.</span><span class="sxs-lookup"><span data-stu-id="5c669-142">Network Address Translation destination IP address.</span></span>|
|<span data-ttu-id="5c669-143">натдестинатионпорт</span><span class="sxs-lookup"><span data-stu-id="5c669-143">natDestinationPort</span></span>|<span data-ttu-id="5c669-144">String</span><span class="sxs-lookup"><span data-stu-id="5c669-144">String</span></span>|<span data-ttu-id="5c669-145">Порт назначения преобразования сетевых адресов.</span><span class="sxs-lookup"><span data-stu-id="5c669-145">Network Address Translation destination port.</span></span>|
|<span data-ttu-id="5c669-146">натсаурцеаддресс</span><span class="sxs-lookup"><span data-stu-id="5c669-146">natSourceAddress</span></span>|<span data-ttu-id="5c669-147">String</span><span class="sxs-lookup"><span data-stu-id="5c669-147">String</span></span>|<span data-ttu-id="5c669-148">IP-адрес источника преобразования сетевых адресов.</span><span class="sxs-lookup"><span data-stu-id="5c669-148">Network Address Translation source IP address.</span></span>|
|<span data-ttu-id="5c669-149">натсаурцепорт</span><span class="sxs-lookup"><span data-stu-id="5c669-149">natSourcePort</span></span>|<span data-ttu-id="5c669-150">String</span><span class="sxs-lookup"><span data-stu-id="5c669-150">String</span></span>|<span data-ttu-id="5c669-151">Порт источника преобразования сетевых адресов.</span><span class="sxs-lookup"><span data-stu-id="5c669-151">Network Address Translation source port.</span></span>|
|<span data-ttu-id="5c669-152">Protocol</span><span class="sxs-lookup"><span data-stu-id="5c669-152">protocol</span></span>|<span data-ttu-id="5c669-153">securityNetworkProtocol</span><span class="sxs-lookup"><span data-stu-id="5c669-153">securityNetworkProtocol</span></span>|<span data-ttu-id="5c669-154">Сетевой протокол.</span><span class="sxs-lookup"><span data-stu-id="5c669-154">Network protocol.</span></span> <span data-ttu-id="5c669-155">Возможные `unknown`значения:, `ip`, `icmp`, `igmp` `ggp` `ipv4` `tcp` `ipSecEncapsulatingSecurityPayload` `ipSecAuthenticationHeader` `icmpV6` `ipv6NoNextHeader` `ipv6DestinationOptions` `nd` `raw` `ipx` `spx` `spxII`,,,,,,, `ipv6FragmentHeader`,,,,,,,,,,,,,,,,,,. `pup` `udp` `idp` `ipv6` `ipv6RoutingHeader`</span><span class="sxs-lookup"><span data-stu-id="5c669-155">Possible values are: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd`, `raw`, `ipx`, `spx`, `spxII`.</span></span>|
|<span data-ttu-id="5c669-156">riskScore</span><span class="sxs-lookup"><span data-stu-id="5c669-156">riskScore</span></span>|<span data-ttu-id="5c669-157">String</span><span class="sxs-lookup"><span data-stu-id="5c669-157">String</span></span>|<span data-ttu-id="5c669-158">Созданный поставщиком/вычисляемый показатель риска для сетевого подключения.</span><span class="sxs-lookup"><span data-stu-id="5c669-158">Provider generated/calculated risk score of the network connection.</span></span> <span data-ttu-id="5c669-159">Рекомендуемый диапазон значений 0-1, указывающий на процентное соотношение.</span><span class="sxs-lookup"><span data-stu-id="5c669-159">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="5c669-160">саурцеаддресс</span><span class="sxs-lookup"><span data-stu-id="5c669-160">sourceAddress</span></span>|<span data-ttu-id="5c669-161">String</span><span class="sxs-lookup"><span data-stu-id="5c669-161">String</span></span>|<span data-ttu-id="5c669-162">Источник (то есть источник) IP-адрес сетевого подключения.</span><span class="sxs-lookup"><span data-stu-id="5c669-162">Source (i.e. origin) IP address (of the network connection).</span></span>|
|<span data-ttu-id="5c669-163">саурцепорт</span><span class="sxs-lookup"><span data-stu-id="5c669-163">sourcePort</span></span>|<span data-ttu-id="5c669-164">String</span><span class="sxs-lookup"><span data-stu-id="5c669-164">String</span></span>|<span data-ttu-id="5c669-165">Исходный (то есть источник) IP-порт (сетевого подключения).</span><span class="sxs-lookup"><span data-stu-id="5c669-165">Source (i.e. origin) IP port (of the network connection).</span></span>|
|<span data-ttu-id="5c669-166">status</span><span class="sxs-lookup"><span data-stu-id="5c669-166">status</span></span>|<span data-ttu-id="5c669-167">connectionStatus</span><span class="sxs-lookup"><span data-stu-id="5c669-167">connectionStatus</span></span>|<span data-ttu-id="5c669-168">Состояние сетевого подключения.</span><span class="sxs-lookup"><span data-stu-id="5c669-168">Network connection status.</span></span> <span data-ttu-id="5c669-169">Возможные значения: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="5c669-169">Possible values are: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span></span>|
|<span data-ttu-id="5c669-170">урлпараметерс</span><span class="sxs-lookup"><span data-stu-id="5c669-170">urlParameters</span></span>|<span data-ttu-id="5c669-171">String</span><span class="sxs-lookup"><span data-stu-id="5c669-171">String</span></span>|<span data-ttu-id="5c669-172">Параметры (суффикс) конечного URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="5c669-172">Parameters (suffix) of the destination URL.</span></span>|

### <a name="securitynetworkprotocol-values"></a><span data-ttu-id="5c669-173">значения Секуритинетворкпротокол</span><span class="sxs-lookup"><span data-stu-id="5c669-173">securityNetworkProtocol values</span></span>

|<span data-ttu-id="5c669-174">Элемент</span><span class="sxs-lookup"><span data-stu-id="5c669-174">Member</span></span>|<span data-ttu-id="5c669-175">Значение</span><span class="sxs-lookup"><span data-stu-id="5c669-175">Value</span></span>|<span data-ttu-id="5c669-176">Описание</span><span class="sxs-lookup"><span data-stu-id="5c669-176">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c669-177">unknown</span><span class="sxs-lookup"><span data-stu-id="5c669-177">unknown</span></span>|<span data-ttu-id="5c669-178">-1</span><span class="sxs-lookup"><span data-stu-id="5c669-178">-1</span></span>|<span data-ttu-id="5c669-179">Неизвестный протокол.</span><span class="sxs-lookup"><span data-stu-id="5c669-179">Unknown protocol.</span></span>|
|<span data-ttu-id="5c669-180">см</span><span class="sxs-lookup"><span data-stu-id="5c669-180">ip</span></span>|<span data-ttu-id="5c669-181">нуль</span><span class="sxs-lookup"><span data-stu-id="5c669-181">0</span></span>|<span data-ttu-id="5c669-182">Протокол IP.</span><span class="sxs-lookup"><span data-stu-id="5c669-182">Internet Protocol.</span></span>|
|<span data-ttu-id="5c669-183">полученных</span><span class="sxs-lookup"><span data-stu-id="5c669-183">icmp</span></span>|<span data-ttu-id="5c669-184">1 </span><span class="sxs-lookup"><span data-stu-id="5c669-184">1</span></span>| <span data-ttu-id="5c669-185">Протокол управления сообщениями в Интернете.</span><span class="sxs-lookup"><span data-stu-id="5c669-185">Internet Control Message Protocol.</span></span>|
|<span data-ttu-id="5c669-186">режимы</span><span class="sxs-lookup"><span data-stu-id="5c669-186">igmp</span></span>|<span data-ttu-id="5c669-187">2 </span><span class="sxs-lookup"><span data-stu-id="5c669-187">2</span></span>| <span data-ttu-id="5c669-188">Протокол управления группами Интернет.</span><span class="sxs-lookup"><span data-stu-id="5c669-188">Internet Group Management Protocol.</span></span>|
|<span data-ttu-id="5c669-189">ггп</span><span class="sxs-lookup"><span data-stu-id="5c669-189">ggp</span></span>|<span data-ttu-id="5c669-190">3 </span><span class="sxs-lookup"><span data-stu-id="5c669-190">3</span></span>| <span data-ttu-id="5c669-191">Протокол шлюза для шлюза.</span><span class="sxs-lookup"><span data-stu-id="5c669-191">Gateway To Gateway Protocol.</span></span>|
|<span data-ttu-id="5c669-192">IPv4</span><span class="sxs-lookup"><span data-stu-id="5c669-192">ipv4</span></span>|<span data-ttu-id="5c669-193">4 </span><span class="sxs-lookup"><span data-stu-id="5c669-193">4</span></span>| <span data-ttu-id="5c669-194">Протокол Интернета версии 4.</span><span class="sxs-lookup"><span data-stu-id="5c669-194">Internet Protocol version 4.</span></span>|
|<span data-ttu-id="5c669-195">tcp</span><span class="sxs-lookup"><span data-stu-id="5c669-195">tcp</span></span>|<span data-ttu-id="5c669-196">6 </span><span class="sxs-lookup"><span data-stu-id="5c669-196">6</span></span>| <span data-ttu-id="5c669-197">Протокол управления передачей.</span><span class="sxs-lookup"><span data-stu-id="5c669-197">Transmission Control Protocol.</span></span>|
|<span data-ttu-id="5c669-198">пуп</span><span class="sxs-lookup"><span data-stu-id="5c669-198">pup</span></span>|<span data-ttu-id="5c669-199">12 </span><span class="sxs-lookup"><span data-stu-id="5c669-199">12</span></span>| <span data-ttu-id="5c669-200">Протокол универсальных пакетов парк.</span><span class="sxs-lookup"><span data-stu-id="5c669-200">PARC Universal Packet Protocol.</span></span>|
|<span data-ttu-id="5c669-201">протокола</span><span class="sxs-lookup"><span data-stu-id="5c669-201">udp</span></span>|<span data-ttu-id="5c669-202">17 </span><span class="sxs-lookup"><span data-stu-id="5c669-202">17</span></span>| <span data-ttu-id="5c669-203">Протокол датаграммы пользователя.</span><span class="sxs-lookup"><span data-stu-id="5c669-203">User Datagram Protocol.</span></span>|
|<span data-ttu-id="5c669-204">IDP</span><span class="sxs-lookup"><span data-stu-id="5c669-204">idp</span></span>|<span data-ttu-id="5c669-205">22</span><span class="sxs-lookup"><span data-stu-id="5c669-205">22</span></span>| <span data-ttu-id="5c669-206">Протокол датаграмм через Интернет.</span><span class="sxs-lookup"><span data-stu-id="5c669-206">Internet Datagram Protocol.</span></span>|
|<span data-ttu-id="5c669-207">поддерживающ</span><span class="sxs-lookup"><span data-stu-id="5c669-207">ipv6</span></span>|<span data-ttu-id="5c669-208">41</span><span class="sxs-lookup"><span data-stu-id="5c669-208">41</span></span>| <span data-ttu-id="5c669-209">Протокол IP версии 6 (IPv6).</span><span class="sxs-lookup"><span data-stu-id="5c669-209">Internet Protocol version 6 (ipv6).</span></span>|
|<span data-ttu-id="5c669-210">ipv6RoutingHeader</span><span class="sxs-lookup"><span data-stu-id="5c669-210">ipv6RoutingHeader</span></span>|<span data-ttu-id="5c669-211">43</span><span class="sxs-lookup"><span data-stu-id="5c669-211">43</span></span>| <span data-ttu-id="5c669-212">заголовок маршрутизации IPv6.</span><span class="sxs-lookup"><span data-stu-id="5c669-212">ipv6 Routing header.</span></span>|
|<span data-ttu-id="5c669-213">ipv6FragmentHeader</span><span class="sxs-lookup"><span data-stu-id="5c669-213">ipv6FragmentHeader</span></span>|<span data-ttu-id="5c669-214">44</span><span class="sxs-lookup"><span data-stu-id="5c669-214">44</span></span>| <span data-ttu-id="5c669-215">заголовок фрагмента IPv6.</span><span class="sxs-lookup"><span data-stu-id="5c669-215">ipv6 Fragment header.</span></span>|
|<span data-ttu-id="5c669-216">ипсеценкапсулатингсекуритипайлоад</span><span class="sxs-lookup"><span data-stu-id="5c669-216">ipSecEncapsulatingSecurityPayload</span></span>|<span data-ttu-id="5c669-217">50</span><span class="sxs-lookup"><span data-stu-id="5c669-217">50</span></span>| <span data-ttu-id="5c669-218">заголовок полезных данных безопасности, включающий IPv6.</span><span class="sxs-lookup"><span data-stu-id="5c669-218">ipv6 Encapsulating Security Payload header.</span></span>|
|<span data-ttu-id="5c669-219">ипсекаусентикатионхеадер</span><span class="sxs-lookup"><span data-stu-id="5c669-219">ipSecAuthenticationHeader</span></span>|<span data-ttu-id="5c669-220">51</span><span class="sxs-lookup"><span data-stu-id="5c669-220">51</span></span>| <span data-ttu-id="5c669-221">заголовок проверки подлинности IPv6.</span><span class="sxs-lookup"><span data-stu-id="5c669-221">ipv6 Authentication header.</span></span>|
|<span data-ttu-id="5c669-222">icmpV6</span><span class="sxs-lookup"><span data-stu-id="5c669-222">icmpV6</span></span>|<span data-ttu-id="5c669-223">58</span><span class="sxs-lookup"><span data-stu-id="5c669-223">58</span></span>| <span data-ttu-id="5c669-224">Протокол управления сообщениями в Интернете для IPv6.</span><span class="sxs-lookup"><span data-stu-id="5c669-224">Internet Control Message Protocol for ipv6.</span></span>|
|<span data-ttu-id="5c669-225">ipv6NoNextHeader</span><span class="sxs-lookup"><span data-stu-id="5c669-225">ipv6NoNextHeader</span></span>|<span data-ttu-id="5c669-226">59</span><span class="sxs-lookup"><span data-stu-id="5c669-226">59</span></span>| <span data-ttu-id="5c669-227">IPv6: следующий заголовок отсутствует.</span><span class="sxs-lookup"><span data-stu-id="5c669-227">ipv6 No next header.</span></span>|
|<span data-ttu-id="5c669-228">ipv6DestinationOptions</span><span class="sxs-lookup"><span data-stu-id="5c669-228">ipv6DestinationOptions</span></span>|<span data-ttu-id="5c669-229">60</span><span class="sxs-lookup"><span data-stu-id="5c669-229">60</span></span>| <span data-ttu-id="5c669-230">заголовок параметров назначения IPv6.</span><span class="sxs-lookup"><span data-stu-id="5c669-230">ipv6 Destination Options header.</span></span>|
|<span data-ttu-id="5c669-231">этаже</span><span class="sxs-lookup"><span data-stu-id="5c669-231">nd</span></span>|<span data-ttu-id="5c669-232">77</span><span class="sxs-lookup"><span data-stu-id="5c669-232">77</span></span>| <span data-ttu-id="5c669-233">Протокол сетевого диска (неофициальный).</span><span class="sxs-lookup"><span data-stu-id="5c669-233">Net Disk Protocol (unofficial).</span></span>|
|<span data-ttu-id="5c669-234">RAW</span><span class="sxs-lookup"><span data-stu-id="5c669-234">raw</span></span>|<span data-ttu-id="5c669-235">255</span><span class="sxs-lookup"><span data-stu-id="5c669-235">255</span></span>| <span data-ttu-id="5c669-236">Протокол IP-пакетов RAW.</span><span class="sxs-lookup"><span data-stu-id="5c669-236">Raw IP packet protocol.</span></span>|
|<span data-ttu-id="5c669-237">x</span><span class="sxs-lookup"><span data-stu-id="5c669-237">ipx</span></span>|<span data-ttu-id="5c669-238">1000</span><span class="sxs-lookup"><span data-stu-id="5c669-238">1000</span></span>| <span data-ttu-id="5c669-239">Протокол обмена пакетами в Интернете.</span><span class="sxs-lookup"><span data-stu-id="5c669-239">Internet Packet Exchange Protocol.</span></span>|
|<span data-ttu-id="5c669-240">возмож</span><span class="sxs-lookup"><span data-stu-id="5c669-240">spx</span></span>|<span data-ttu-id="5c669-241">1256</span><span class="sxs-lookup"><span data-stu-id="5c669-241">1256</span></span>| <span data-ttu-id="5c669-242">Последовательный протокол обмена пакетами.</span><span class="sxs-lookup"><span data-stu-id="5c669-242">Sequenced Packet Exchange protocol.</span></span>|
|<span data-ttu-id="5c669-243">спксии</span><span class="sxs-lookup"><span data-stu-id="5c669-243">spxII</span></span>|<span data-ttu-id="5c669-244">1257</span><span class="sxs-lookup"><span data-stu-id="5c669-244">1257</span></span>| <span data-ttu-id="5c669-245">Последовательный протокол обмена пакетами версии 2.</span><span class="sxs-lookup"><span data-stu-id="5c669-245">Sequenced Packet Exchange version 2 protocol.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5c669-246">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5c669-246">JSON representation</span></span>

<span data-ttu-id="5c669-247">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5c669-247">The following is a JSON representation of the resource.</span></span>

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
