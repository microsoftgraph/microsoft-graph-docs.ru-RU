---
title: тип ресурса networkConnection
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 2221f38c4ba8f8e71030d540985fb93f415bfa19
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722113"
---
# <a name="networkconnection-resource-type"></a><span data-ttu-id="5fffc-104">тип ресурса networkConnection</span><span class="sxs-lookup"><span data-stu-id="5fffc-104">networkConnection resource type</span></span>

<span data-ttu-id="5fffc-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5fffc-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5fffc-106">Содержит сведения о сетевом подключении, связанном с оповещением.</span><span class="sxs-lookup"><span data-stu-id="5fffc-106">Contains stateful information about the network connection related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="5fffc-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5fffc-107">Properties</span></span>

| <span data-ttu-id="5fffc-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="5fffc-108">Property</span></span>   | <span data-ttu-id="5fffc-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5fffc-109">Type</span></span>|<span data-ttu-id="5fffc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5fffc-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5fffc-111">applicationName</span><span class="sxs-lookup"><span data-stu-id="5fffc-111">applicationName</span></span>|<span data-ttu-id="5fffc-112">String</span><span class="sxs-lookup"><span data-stu-id="5fffc-112">String</span></span>|<span data-ttu-id="5fffc-113">Имя приложения, управляющего сетевым подключением (например, Facebook, SMTP и т.д.).</span><span class="sxs-lookup"><span data-stu-id="5fffc-113">Name of the application managing the network connection (for example, Facebook, SMTP, etc.).</span></span>|
|<span data-ttu-id="5fffc-114">destinationAddress</span><span class="sxs-lookup"><span data-stu-id="5fffc-114">destinationAddress</span></span>|<span data-ttu-id="5fffc-115">String</span><span class="sxs-lookup"><span data-stu-id="5fffc-115">String</span></span>|<span data-ttu-id="5fffc-116">IP-адрес назначения (сетевого подключения).</span><span class="sxs-lookup"><span data-stu-id="5fffc-116">Destination IP address (of the network connection).</span></span>|
|<span data-ttu-id="5fffc-117">destinationDomain</span><span class="sxs-lookup"><span data-stu-id="5fffc-117">destinationDomain</span></span>|<span data-ttu-id="5fffc-118">String</span><span class="sxs-lookup"><span data-stu-id="5fffc-118">String</span></span>|<span data-ttu-id="5fffc-119">Часть домена назначения URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="5fffc-119">Destination domain portion of the destination URL.</span></span> <span data-ttu-id="5fffc-120">(например, "www.contoso.com").</span><span class="sxs-lookup"><span data-stu-id="5fffc-120">(for example 'www.contoso.com').</span></span>|
|<span data-ttu-id="5fffc-121">destinationLocation</span><span class="sxs-lookup"><span data-stu-id="5fffc-121">destinationLocation</span></span>|<span data-ttu-id="5fffc-122">String</span><span class="sxs-lookup"><span data-stu-id="5fffc-122">String</span></span>|<span data-ttu-id="5fffc-123">Расположение (сопоставление IP-адресов), связанное с назначением сетевого подключения.</span><span class="sxs-lookup"><span data-stu-id="5fffc-123">Location (by IP address mapping) associated with the destination of a network connection.</span></span>|
|<span data-ttu-id="5fffc-124">destinationPort</span><span class="sxs-lookup"><span data-stu-id="5fffc-124">destinationPort</span></span>|<span data-ttu-id="5fffc-125">String</span><span class="sxs-lookup"><span data-stu-id="5fffc-125">String</span></span>|<span data-ttu-id="5fffc-126">Порт назначения (сетевого подключения).</span><span class="sxs-lookup"><span data-stu-id="5fffc-126">Destination port (of the network connection).</span></span>|
|<span data-ttu-id="5fffc-127">destinationUrl</span><span class="sxs-lookup"><span data-stu-id="5fffc-127">destinationUrl</span></span>|<span data-ttu-id="5fffc-128">String</span><span class="sxs-lookup"><span data-stu-id="5fffc-128">String</span></span>|<span data-ttu-id="5fffc-129">Строка URL-адрес/строка URI сетевого подключения без учета параметров.</span><span class="sxs-lookup"><span data-stu-id="5fffc-129">Network connection URL/URI string - excluding parameters.</span></span> <span data-ttu-id="5fffc-130">(например, www.contoso.com/products/default.html')</span><span class="sxs-lookup"><span data-stu-id="5fffc-130">(for example 'www.contoso.com/products/default.html')</span></span>|
|<span data-ttu-id="5fffc-131">direction</span><span class="sxs-lookup"><span data-stu-id="5fffc-131">direction</span></span>|<span data-ttu-id="5fffc-132">connectionDirection</span><span class="sxs-lookup"><span data-stu-id="5fffc-132">connectionDirection</span></span>|<span data-ttu-id="5fffc-133">Направление сетевого подключения.</span><span class="sxs-lookup"><span data-stu-id="5fffc-133">Network connection direction.</span></span> <span data-ttu-id="5fffc-134">Возможные значения: `unknown`, `inbound`, `outbound`.</span><span class="sxs-lookup"><span data-stu-id="5fffc-134">Possible values are: `unknown`, `inbound`, `outbound`.</span></span>|
|<span data-ttu-id="5fffc-135">domainRegisteredDateTime</span><span class="sxs-lookup"><span data-stu-id="5fffc-135">domainRegisteredDateTime</span></span>|<span data-ttu-id="5fffc-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5fffc-136">DateTimeOffset</span></span>|<span data-ttu-id="5fffc-137">Дата регистрации домена назначения.</span><span class="sxs-lookup"><span data-stu-id="5fffc-137">Date when the destination domain was registered.</span></span> <span data-ttu-id="5fffc-138">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="5fffc-138">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5fffc-139">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="5fffc-139">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="5fffc-140">localDnsName</span><span class="sxs-lookup"><span data-stu-id="5fffc-140">localDnsName</span></span>|<span data-ttu-id="5fffc-141">String</span><span class="sxs-lookup"><span data-stu-id="5fffc-141">String</span></span>|<span data-ttu-id="5fffc-142">Локальное разрешение имен DNS, как оно отображается в локальном DNS-кэше хоста (например, в случае, если файл "хост" был подделан).</span><span class="sxs-lookup"><span data-stu-id="5fffc-142">The local DNS name resolution as it appears in the host's local DNS cache (for example, in case the 'hosts' file was tampered with).</span></span>|
|<span data-ttu-id="5fffc-143">natDestinationAddress</span><span class="sxs-lookup"><span data-stu-id="5fffc-143">natDestinationAddress</span></span>|<span data-ttu-id="5fffc-144">String</span><span class="sxs-lookup"><span data-stu-id="5fffc-144">String</span></span>|<span data-ttu-id="5fffc-145">IP-адрес назначения перевода сетевого адреса.</span><span class="sxs-lookup"><span data-stu-id="5fffc-145">Network Address Translation destination IP address.</span></span>|
|<span data-ttu-id="5fffc-146">natDestinationPort</span><span class="sxs-lookup"><span data-stu-id="5fffc-146">natDestinationPort</span></span>|<span data-ttu-id="5fffc-147">String</span><span class="sxs-lookup"><span data-stu-id="5fffc-147">String</span></span>|<span data-ttu-id="5fffc-148">Порт назначения перевода сетевых адресов.</span><span class="sxs-lookup"><span data-stu-id="5fffc-148">Network Address Translation destination port.</span></span>|
|<span data-ttu-id="5fffc-149">natSourceAddress</span><span class="sxs-lookup"><span data-stu-id="5fffc-149">natSourceAddress</span></span>|<span data-ttu-id="5fffc-150">String</span><span class="sxs-lookup"><span data-stu-id="5fffc-150">String</span></span>|<span data-ttu-id="5fffc-151">IP-адрес источника перевода сетевого адреса.</span><span class="sxs-lookup"><span data-stu-id="5fffc-151">Network Address Translation source IP address.</span></span>|
|<span data-ttu-id="5fffc-152">natSourcePort</span><span class="sxs-lookup"><span data-stu-id="5fffc-152">natSourcePort</span></span>|<span data-ttu-id="5fffc-153">String</span><span class="sxs-lookup"><span data-stu-id="5fffc-153">String</span></span>|<span data-ttu-id="5fffc-154">Порт источника перевода сетевых адресов.</span><span class="sxs-lookup"><span data-stu-id="5fffc-154">Network Address Translation source port.</span></span>|
|<span data-ttu-id="5fffc-155">протокол</span><span class="sxs-lookup"><span data-stu-id="5fffc-155">protocol</span></span>|<span data-ttu-id="5fffc-156">securityNetworkProtocol</span><span class="sxs-lookup"><span data-stu-id="5fffc-156">securityNetworkProtocol</span></span>|<span data-ttu-id="5fffc-157">Сетевой протокол.</span><span class="sxs-lookup"><span data-stu-id="5fffc-157">Network protocol.</span></span> <span data-ttu-id="5fffc-158">Возможные значения: `unknown` `ip` , , `icmp` `igmp` `ggp` `ipv4` `tcp` `pup` `udp` `idp` `ipv6` `ipv6RoutingHeader` , `ipv6FragmentHeader` `ipSecEncapsulatingSecurityPayload` `ipSecAuthenticationHeader` `icmpV6` `ipv6NoNextHeader` `ipv6DestinationOptions` `nd` `raw` `ipx` `spx` `spxII` .</span><span class="sxs-lookup"><span data-stu-id="5fffc-158">Possible values are: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd`, `raw`, `ipx`, `spx`, `spxII`.</span></span>|
|<span data-ttu-id="5fffc-159">riskScore</span><span class="sxs-lookup"><span data-stu-id="5fffc-159">riskScore</span></span>|<span data-ttu-id="5fffc-160">String</span><span class="sxs-lookup"><span data-stu-id="5fffc-160">String</span></span>|<span data-ttu-id="5fffc-161">Оценка риска сетевого подключения поставщика сгенерирована и рассчитана.</span><span class="sxs-lookup"><span data-stu-id="5fffc-161">Provider generated/calculated risk score of the network connection.</span></span> <span data-ttu-id="5fffc-162">Рекомендуемый диапазон значений 0-1, который приравнивается к проценту.</span><span class="sxs-lookup"><span data-stu-id="5fffc-162">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="5fffc-163">sourceAddress</span><span class="sxs-lookup"><span data-stu-id="5fffc-163">sourceAddress</span></span>|<span data-ttu-id="5fffc-164">String</span><span class="sxs-lookup"><span data-stu-id="5fffc-164">String</span></span>|<span data-ttu-id="5fffc-165">IP-адрес источника (то есть происхождения) (сетевого подключения).</span><span class="sxs-lookup"><span data-stu-id="5fffc-165">Source (i.e. origin) IP address (of the network connection).</span></span>|
|<span data-ttu-id="5fffc-166">sourceLocation</span><span class="sxs-lookup"><span data-stu-id="5fffc-166">sourceLocation</span></span>|<span data-ttu-id="5fffc-167">String</span><span class="sxs-lookup"><span data-stu-id="5fffc-167">String</span></span>|<span data-ttu-id="5fffc-168">Расположение (по сопоставлению IP-адресов), связанное с источником сетевого подключения.</span><span class="sxs-lookup"><span data-stu-id="5fffc-168">Location (by IP address mapping) associated with the source of a network connection.</span></span>|
|<span data-ttu-id="5fffc-169">sourcePort</span><span class="sxs-lookup"><span data-stu-id="5fffc-169">sourcePort</span></span>|<span data-ttu-id="5fffc-170">String</span><span class="sxs-lookup"><span data-stu-id="5fffc-170">String</span></span>|<span data-ttu-id="5fffc-171">Ip-порт source (то есть происхождение) (сетевого подключения).</span><span class="sxs-lookup"><span data-stu-id="5fffc-171">Source (i.e. origin) IP port (of the network connection).</span></span>|
|<span data-ttu-id="5fffc-172">status</span><span class="sxs-lookup"><span data-stu-id="5fffc-172">status</span></span>|<span data-ttu-id="5fffc-173">connectionStatus</span><span class="sxs-lookup"><span data-stu-id="5fffc-173">connectionStatus</span></span>|<span data-ttu-id="5fffc-174">Состояние сетевого подключения.</span><span class="sxs-lookup"><span data-stu-id="5fffc-174">Network connection status.</span></span> <span data-ttu-id="5fffc-175">Возможные значения: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="5fffc-175">Possible values are: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span></span>|
|<span data-ttu-id="5fffc-176">urlParameters</span><span class="sxs-lookup"><span data-stu-id="5fffc-176">urlParameters</span></span>|<span data-ttu-id="5fffc-177">String</span><span class="sxs-lookup"><span data-stu-id="5fffc-177">String</span></span>|<span data-ttu-id="5fffc-178">Параметры (суффикс) URL-адреса назначения.</span><span class="sxs-lookup"><span data-stu-id="5fffc-178">Parameters (suffix) of the destination URL.</span></span>|

### <a name="securitynetworkprotocol-values"></a><span data-ttu-id="5fffc-179">значения securityNetworkProtocol</span><span class="sxs-lookup"><span data-stu-id="5fffc-179">securityNetworkProtocol values</span></span>

|<span data-ttu-id="5fffc-180">Элемент</span><span class="sxs-lookup"><span data-stu-id="5fffc-180">Member</span></span>|<span data-ttu-id="5fffc-181">Значение</span><span class="sxs-lookup"><span data-stu-id="5fffc-181">Value</span></span>|<span data-ttu-id="5fffc-182">Описание</span><span class="sxs-lookup"><span data-stu-id="5fffc-182">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5fffc-183">unknown</span><span class="sxs-lookup"><span data-stu-id="5fffc-183">unknown</span></span>|<span data-ttu-id="5fffc-184">-1</span><span class="sxs-lookup"><span data-stu-id="5fffc-184">-1</span></span>|<span data-ttu-id="5fffc-185">Неизвестный протокол.</span><span class="sxs-lookup"><span data-stu-id="5fffc-185">Unknown protocol.</span></span>|
|<span data-ttu-id="5fffc-186">IP</span><span class="sxs-lookup"><span data-stu-id="5fffc-186">ip</span></span>|<span data-ttu-id="5fffc-187">0</span><span class="sxs-lookup"><span data-stu-id="5fffc-187">0</span></span>|<span data-ttu-id="5fffc-188">Протокол Интернета.</span><span class="sxs-lookup"><span data-stu-id="5fffc-188">Internet Protocol.</span></span>|
|<span data-ttu-id="5fffc-189">icmp</span><span class="sxs-lookup"><span data-stu-id="5fffc-189">icmp</span></span>|<span data-ttu-id="5fffc-190">1</span><span class="sxs-lookup"><span data-stu-id="5fffc-190">1</span></span>| <span data-ttu-id="5fffc-191">Протокол сообщений управления Интернетом.</span><span class="sxs-lookup"><span data-stu-id="5fffc-191">Internet Control Message Protocol.</span></span>|
|<span data-ttu-id="5fffc-192">igmp</span><span class="sxs-lookup"><span data-stu-id="5fffc-192">igmp</span></span>|<span data-ttu-id="5fffc-193">2 </span><span class="sxs-lookup"><span data-stu-id="5fffc-193">2</span></span>| <span data-ttu-id="5fffc-194">Протокол управления интернет-группой.</span><span class="sxs-lookup"><span data-stu-id="5fffc-194">Internet Group Management Protocol.</span></span>|
|<span data-ttu-id="5fffc-195">ggp</span><span class="sxs-lookup"><span data-stu-id="5fffc-195">ggp</span></span>|<span data-ttu-id="5fffc-196">3 </span><span class="sxs-lookup"><span data-stu-id="5fffc-196">3</span></span>| <span data-ttu-id="5fffc-197">Протокол Gateway to Gateway.</span><span class="sxs-lookup"><span data-stu-id="5fffc-197">Gateway To Gateway Protocol.</span></span>|
|<span data-ttu-id="5fffc-198">ipv4</span><span class="sxs-lookup"><span data-stu-id="5fffc-198">ipv4</span></span>|<span data-ttu-id="5fffc-199">4 </span><span class="sxs-lookup"><span data-stu-id="5fffc-199">4</span></span>| <span data-ttu-id="5fffc-200">Версия 4 протокола Интернета.</span><span class="sxs-lookup"><span data-stu-id="5fffc-200">Internet Protocol version 4.</span></span>|
|<span data-ttu-id="5fffc-201">tcp</span><span class="sxs-lookup"><span data-stu-id="5fffc-201">tcp</span></span>|<span data-ttu-id="5fffc-202">6 </span><span class="sxs-lookup"><span data-stu-id="5fffc-202">6</span></span>| <span data-ttu-id="5fffc-203">Протокол управления передачей.</span><span class="sxs-lookup"><span data-stu-id="5fffc-203">Transmission Control Protocol.</span></span>|
|<span data-ttu-id="5fffc-204">pup</span><span class="sxs-lookup"><span data-stu-id="5fffc-204">pup</span></span>|<span data-ttu-id="5fffc-205">12 </span><span class="sxs-lookup"><span data-stu-id="5fffc-205">12</span></span>| <span data-ttu-id="5fffc-206">Универсальный протокол пакетов PARC.</span><span class="sxs-lookup"><span data-stu-id="5fffc-206">PARC Universal Packet Protocol.</span></span>|
|<span data-ttu-id="5fffc-207">udp</span><span class="sxs-lookup"><span data-stu-id="5fffc-207">udp</span></span>|<span data-ttu-id="5fffc-208">17 </span><span class="sxs-lookup"><span data-stu-id="5fffc-208">17</span></span>| <span data-ttu-id="5fffc-209">Протокол пользовательской datagram.</span><span class="sxs-lookup"><span data-stu-id="5fffc-209">User Datagram Protocol.</span></span>|
|<span data-ttu-id="5fffc-210">idp</span><span class="sxs-lookup"><span data-stu-id="5fffc-210">idp</span></span>|<span data-ttu-id="5fffc-211">22</span><span class="sxs-lookup"><span data-stu-id="5fffc-211">22</span></span>| <span data-ttu-id="5fffc-212">Протокол Internet Datagram.</span><span class="sxs-lookup"><span data-stu-id="5fffc-212">Internet Datagram Protocol.</span></span>|
|<span data-ttu-id="5fffc-213">ipv6</span><span class="sxs-lookup"><span data-stu-id="5fffc-213">ipv6</span></span>|<span data-ttu-id="5fffc-214">41</span><span class="sxs-lookup"><span data-stu-id="5fffc-214">41</span></span>| <span data-ttu-id="5fffc-215">Версия 6 протокола Интернета (ipv6).</span><span class="sxs-lookup"><span data-stu-id="5fffc-215">Internet Protocol version 6 (ipv6).</span></span>|
|<span data-ttu-id="5fffc-216">ipv6RoutingHeader</span><span class="sxs-lookup"><span data-stu-id="5fffc-216">ipv6RoutingHeader</span></span>|<span data-ttu-id="5fffc-217">43</span><span class="sxs-lookup"><span data-stu-id="5fffc-217">43</span></span>| <span data-ttu-id="5fffc-218">загодер маршрутивки ipv6.</span><span class="sxs-lookup"><span data-stu-id="5fffc-218">ipv6 Routing header.</span></span>|
|<span data-ttu-id="5fffc-219">ipv6FragmentHeader</span><span class="sxs-lookup"><span data-stu-id="5fffc-219">ipv6FragmentHeader</span></span>|<span data-ttu-id="5fffc-220">44</span><span class="sxs-lookup"><span data-stu-id="5fffc-220">44</span></span>| <span data-ttu-id="5fffc-221">Заглавная часть ipv6.</span><span class="sxs-lookup"><span data-stu-id="5fffc-221">ipv6 Fragment header.</span></span>|
|<span data-ttu-id="5fffc-222">ipSecEncapsulatingSecurityPayload</span><span class="sxs-lookup"><span data-stu-id="5fffc-222">ipSecEncapsulatingSecurityPayload</span></span>|<span data-ttu-id="5fffc-223">50</span><span class="sxs-lookup"><span data-stu-id="5fffc-223">50</span></span>| <span data-ttu-id="5fffc-224">ipv6 Encapsulating Security Payload header.</span><span class="sxs-lookup"><span data-stu-id="5fffc-224">ipv6 Encapsulating Security Payload header.</span></span>|
|<span data-ttu-id="5fffc-225">ipSecAuthenticationHeader</span><span class="sxs-lookup"><span data-stu-id="5fffc-225">ipSecAuthenticationHeader</span></span>|<span data-ttu-id="5fffc-226">51</span><span class="sxs-lookup"><span data-stu-id="5fffc-226">51</span></span>| <span data-ttu-id="5fffc-227">загона проверки подлинности ipv6.</span><span class="sxs-lookup"><span data-stu-id="5fffc-227">ipv6 Authentication header.</span></span>|
|<span data-ttu-id="5fffc-228">icmpV6</span><span class="sxs-lookup"><span data-stu-id="5fffc-228">icmpV6</span></span>|<span data-ttu-id="5fffc-229">58</span><span class="sxs-lookup"><span data-stu-id="5fffc-229">58</span></span>| <span data-ttu-id="5fffc-230">Протокол сообщения управления Интернетом для ipv6.</span><span class="sxs-lookup"><span data-stu-id="5fffc-230">Internet Control Message Protocol for ipv6.</span></span>|
|<span data-ttu-id="5fffc-231">ipv6NoNextHeader</span><span class="sxs-lookup"><span data-stu-id="5fffc-231">ipv6NoNextHeader</span></span>|<span data-ttu-id="5fffc-232">59</span><span class="sxs-lookup"><span data-stu-id="5fffc-232">59</span></span>| <span data-ttu-id="5fffc-233">ipv6 Нет следующего загона.</span><span class="sxs-lookup"><span data-stu-id="5fffc-233">ipv6 No next header.</span></span>|
|<span data-ttu-id="5fffc-234">ipv6DestinationOptions</span><span class="sxs-lookup"><span data-stu-id="5fffc-234">ipv6DestinationOptions</span></span>|<span data-ttu-id="5fffc-235">60</span><span class="sxs-lookup"><span data-stu-id="5fffc-235">60</span></span>| <span data-ttu-id="5fffc-236">заглавная головка вариантов назначения ipv6.</span><span class="sxs-lookup"><span data-stu-id="5fffc-236">ipv6 Destination Options header.</span></span>|
|<span data-ttu-id="5fffc-237">nd</span><span class="sxs-lookup"><span data-stu-id="5fffc-237">nd</span></span>|<span data-ttu-id="5fffc-238">77</span><span class="sxs-lookup"><span data-stu-id="5fffc-238">77</span></span>| <span data-ttu-id="5fffc-239">Протокол чистого диска (неофициальный).</span><span class="sxs-lookup"><span data-stu-id="5fffc-239">Net Disk Protocol (unofficial).</span></span>|
|<span data-ttu-id="5fffc-240">raw</span><span class="sxs-lookup"><span data-stu-id="5fffc-240">raw</span></span>|<span data-ttu-id="5fffc-241">255</span><span class="sxs-lookup"><span data-stu-id="5fffc-241">255</span></span>| <span data-ttu-id="5fffc-242">Необработанные протоколы пакетов IP.</span><span class="sxs-lookup"><span data-stu-id="5fffc-242">Raw IP packet protocol.</span></span>|
|<span data-ttu-id="5fffc-243">ipx</span><span class="sxs-lookup"><span data-stu-id="5fffc-243">ipx</span></span>|<span data-ttu-id="5fffc-244">1000</span><span class="sxs-lookup"><span data-stu-id="5fffc-244">1000</span></span>| <span data-ttu-id="5fffc-245">Протокол обмена пакетами в Интернете.</span><span class="sxs-lookup"><span data-stu-id="5fffc-245">Internet Packet Exchange Protocol.</span></span>|
|<span data-ttu-id="5fffc-246">spx</span><span class="sxs-lookup"><span data-stu-id="5fffc-246">spx</span></span>|<span data-ttu-id="5fffc-247">1256</span><span class="sxs-lookup"><span data-stu-id="5fffc-247">1256</span></span>| <span data-ttu-id="5fffc-248">Секвенный протокол Exchange пакетов.</span><span class="sxs-lookup"><span data-stu-id="5fffc-248">Sequenced Packet Exchange protocol.</span></span>|
|<span data-ttu-id="5fffc-249">spxII</span><span class="sxs-lookup"><span data-stu-id="5fffc-249">spxII</span></span>|<span data-ttu-id="5fffc-250">1257</span><span class="sxs-lookup"><span data-stu-id="5fffc-250">1257</span></span>| <span data-ttu-id="5fffc-251">Секвенсорный протокол Exchange пакетов версии 2.</span><span class="sxs-lookup"><span data-stu-id="5fffc-251">Sequenced Packet Exchange version 2 protocol.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5fffc-252">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5fffc-252">JSON representation</span></span>

<span data-ttu-id="5fffc-253">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5fffc-253">The following is a JSON representation of the resource.</span></span>

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


