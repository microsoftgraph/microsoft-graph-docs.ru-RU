---
title: Тип ресурса networkConnection
description: Содержит информацию о состояниях о сетевое подключение, связанные с оповещение.
localization_priority: Normal
ms.openlocfilehash: 78ddcfd19d68b8dcd64c74a5beed6d1430f0ca38
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826511"
---
# <a name="networkconnection-resource-type"></a><span data-ttu-id="44542-103">Тип ресурса networkConnection</span><span class="sxs-lookup"><span data-stu-id="44542-103">networkConnection resource type</span></span>

<span data-ttu-id="44542-104">Содержит информацию о состояниях о сетевое подключение, связанные с оповещение.</span><span class="sxs-lookup"><span data-stu-id="44542-104">Contains stateful information about the network connection related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="44542-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="44542-105">Properties</span></span>

| <span data-ttu-id="44542-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="44542-106">Property</span></span>   | <span data-ttu-id="44542-107">Тип</span><span class="sxs-lookup"><span data-stu-id="44542-107">Type</span></span>|<span data-ttu-id="44542-108">Описание</span><span class="sxs-lookup"><span data-stu-id="44542-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="44542-109">applicationName</span><span class="sxs-lookup"><span data-stu-id="44542-109">applicationName</span></span>|<span data-ttu-id="44542-110">String</span><span class="sxs-lookup"><span data-stu-id="44542-110">String</span></span>|<span data-ttu-id="44542-111">Имя приложения, управление сетевое подключение (например, Facebook, SMTP, и т.д.).</span><span class="sxs-lookup"><span data-stu-id="44542-111">Name of the application managing the network connection (for example, Facebook, SMTP, etc.).</span></span>|
|<span data-ttu-id="44542-112">destinationAddress</span><span class="sxs-lookup"><span data-stu-id="44542-112">destinationAddress</span></span>|<span data-ttu-id="44542-113">Строка</span><span class="sxs-lookup"><span data-stu-id="44542-113">String</span></span>|<span data-ttu-id="44542-114">Конечный IP-адрес (сетевое подключение).</span><span class="sxs-lookup"><span data-stu-id="44542-114">Destination IP address (of the network connection).</span></span>|
|<span data-ttu-id="44542-115">destinationDomain</span><span class="sxs-lookup"><span data-stu-id="44542-115">destinationDomain</span></span>|<span data-ttu-id="44542-116">Строка</span><span class="sxs-lookup"><span data-stu-id="44542-116">String</span></span>|<span data-ttu-id="44542-117">Часть домена конечный URL-адрес назначения.</span><span class="sxs-lookup"><span data-stu-id="44542-117">Destination domain portion of the destination URL.</span></span> <span data-ttu-id="44542-118">(например «www.contoso.com»).</span><span class="sxs-lookup"><span data-stu-id="44542-118">(for example 'www.contoso.com').</span></span>|
|<span data-ttu-id="44542-119">destinationPort</span><span class="sxs-lookup"><span data-stu-id="44542-119">destinationPort</span></span>|<span data-ttu-id="44542-120">Строка</span><span class="sxs-lookup"><span data-stu-id="44542-120">String</span></span>|<span data-ttu-id="44542-121">Порт назначения (сетевое подключение).</span><span class="sxs-lookup"><span data-stu-id="44542-121">Destination port (of the network connection).</span></span>|
|<span data-ttu-id="44542-122">destinationUrl</span><span class="sxs-lookup"><span data-stu-id="44542-122">destinationUrl</span></span>|<span data-ttu-id="44542-123">Строка</span><span class="sxs-lookup"><span data-stu-id="44542-123">String</span></span>|<span data-ttu-id="44542-124">Строка подключения URL-адрес или URI - исключение параметров в сети.</span><span class="sxs-lookup"><span data-stu-id="44542-124">Network connection URL/URI string - excluding parameters.</span></span> <span data-ttu-id="44542-125">(например, «www.contoso.com/products/default.html»)</span><span class="sxs-lookup"><span data-stu-id="44542-125">(for example 'www.contoso.com/products/default.html')</span></span>|
|<span data-ttu-id="44542-126">Направление</span><span class="sxs-lookup"><span data-stu-id="44542-126">direction</span></span>|<span data-ttu-id="44542-127">connectionDirection</span><span class="sxs-lookup"><span data-stu-id="44542-127">connectionDirection</span></span>|<span data-ttu-id="44542-128">Направление подключения к сети.</span><span class="sxs-lookup"><span data-stu-id="44542-128">Network connection direction.</span></span> <span data-ttu-id="44542-129">Возможные значения: `unknown`, `inbound`, `outbound`.</span><span class="sxs-lookup"><span data-stu-id="44542-129">Possible values are: `unknown`, `inbound`, `outbound`.</span></span>|
|<span data-ttu-id="44542-130">domainRegisteredDateTime</span><span class="sxs-lookup"><span data-stu-id="44542-130">domainRegisteredDateTime</span></span>|<span data-ttu-id="44542-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44542-131">DateTimeOffset</span></span>|<span data-ttu-id="44542-132">Дата регистрации целевом домене.</span><span class="sxs-lookup"><span data-stu-id="44542-132">Date when the destination domain was registered.</span></span> <span data-ttu-id="44542-133">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="44542-133">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="44542-134">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="44542-134">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="44542-135">localDnsName</span><span class="sxs-lookup"><span data-stu-id="44542-135">localDnsName</span></span>|<span data-ttu-id="44542-136">Строка</span><span class="sxs-lookup"><span data-stu-id="44542-136">String</span></span>|<span data-ttu-id="44542-137">Локальное разрешение имен DNS как оно отображается в локальном кэше DNS узла (например, в случае подделано файл «hosts»).</span><span class="sxs-lookup"><span data-stu-id="44542-137">The local DNS name resolution as it appears in the host's local DNS cache (for example, in case the 'hosts' file was tampered with).</span></span>|
|<span data-ttu-id="44542-138">natDestinationAddress</span><span class="sxs-lookup"><span data-stu-id="44542-138">natDestinationAddress</span></span>|<span data-ttu-id="44542-139">Строка</span><span class="sxs-lookup"><span data-stu-id="44542-139">String</span></span>|<span data-ttu-id="44542-140">Преобразование адресов конечный IP-адрес в сети.</span><span class="sxs-lookup"><span data-stu-id="44542-140">Network Address Translation destination IP address.</span></span>|
|<span data-ttu-id="44542-141">natDestinationPort</span><span class="sxs-lookup"><span data-stu-id="44542-141">natDestinationPort</span></span>|<span data-ttu-id="44542-142">Строка</span><span class="sxs-lookup"><span data-stu-id="44542-142">String</span></span>|<span data-ttu-id="44542-143">Конечный порт преобразование адресов в сети.</span><span class="sxs-lookup"><span data-stu-id="44542-143">Network Address Translation destination port.</span></span>|
|<span data-ttu-id="44542-144">natSourceAddress</span><span class="sxs-lookup"><span data-stu-id="44542-144">natSourceAddress</span></span>|<span data-ttu-id="44542-145">Строка</span><span class="sxs-lookup"><span data-stu-id="44542-145">String</span></span>|<span data-ttu-id="44542-146">Преобразование адресов исходный IP-адрес в сети.</span><span class="sxs-lookup"><span data-stu-id="44542-146">Network Address Translation source IP address.</span></span>|
|<span data-ttu-id="44542-147">natSourcePort</span><span class="sxs-lookup"><span data-stu-id="44542-147">natSourcePort</span></span>|<span data-ttu-id="44542-148">Строка</span><span class="sxs-lookup"><span data-stu-id="44542-148">String</span></span>|<span data-ttu-id="44542-149">Порт источника, преобразование адресов сети.</span><span class="sxs-lookup"><span data-stu-id="44542-149">Network Address Translation source port.</span></span>|
|<span data-ttu-id="44542-150">protocol</span><span class="sxs-lookup"><span data-stu-id="44542-150">protocol</span></span>|[<span data-ttu-id="44542-151">securityNetworkProtocol</span><span class="sxs-lookup"><span data-stu-id="44542-151">securityNetworkProtocol</span></span>](securitynetworkprotocol.md)|<span data-ttu-id="44542-152">Сетевой протокол.</span><span class="sxs-lookup"><span data-stu-id="44542-152">Network protocol.</span></span> <span data-ttu-id="44542-153">Возможные значения: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd` , `raw`, `ipx`, `spx`, `spxII`.</span><span class="sxs-lookup"><span data-stu-id="44542-153">Possible values are: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd`, `raw`, `ipx`, `spx`, `spxII`.</span></span>|
|<span data-ttu-id="44542-154">riskScore</span><span class="sxs-lookup"><span data-stu-id="44542-154">riskScore</span></span>|<span data-ttu-id="44542-155">Строка</span><span class="sxs-lookup"><span data-stu-id="44542-155">String</span></span>|<span data-ttu-id="44542-156">Поставщик создан/вычисляется риск показатель для подключения к сети.</span><span class="sxs-lookup"><span data-stu-id="44542-156">Provider generated/calculated risk score of the network connection.</span></span> <span data-ttu-id="44542-157">Рекомендуемое значение диапазона 0-1, который соответствует в процентах.</span><span class="sxs-lookup"><span data-stu-id="44542-157">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="44542-158">sourceAddress</span><span class="sxs-lookup"><span data-stu-id="44542-158">sourceAddress</span></span>|<span data-ttu-id="44542-159">Строка</span><span class="sxs-lookup"><span data-stu-id="44542-159">String</span></span>|<span data-ttu-id="44542-160">(То есть источник) IP-адрес источника (сетевое подключение).</span><span class="sxs-lookup"><span data-stu-id="44542-160">Source (i.e. origin) IP address (of the network connection).</span></span>|
|<span data-ttu-id="44542-161">sourcePort</span><span class="sxs-lookup"><span data-stu-id="44542-161">sourcePort</span></span>|<span data-ttu-id="44542-162">Строка</span><span class="sxs-lookup"><span data-stu-id="44542-162">String</span></span>|<span data-ttu-id="44542-163">Исходный (то есть источник) IP-адрес порт (сетевое подключение).</span><span class="sxs-lookup"><span data-stu-id="44542-163">Source (i.e. origin) IP port (of the network connection).</span></span>|
|<span data-ttu-id="44542-164">status</span><span class="sxs-lookup"><span data-stu-id="44542-164">status</span></span>|<span data-ttu-id="44542-165">connectionStatus</span><span class="sxs-lookup"><span data-stu-id="44542-165">connectionStatus</span></span>|<span data-ttu-id="44542-166">Состояние подключения к сети.</span><span class="sxs-lookup"><span data-stu-id="44542-166">Network connection status.</span></span> <span data-ttu-id="44542-167">Возможные значения: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="44542-167">Possible values are: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span></span>|
|<span data-ttu-id="44542-168">urlParameters</span><span class="sxs-lookup"><span data-stu-id="44542-168">urlParameters</span></span>|<span data-ttu-id="44542-169">Строка</span><span class="sxs-lookup"><span data-stu-id="44542-169">String</span></span>|<span data-ttu-id="44542-170">Параметры (суффикс) URL-адрес назначения.</span><span class="sxs-lookup"><span data-stu-id="44542-170">Parameters (suffix) of the destination URL.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="44542-171">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="44542-171">JSON representation</span></span>

<span data-ttu-id="44542-172">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="44542-172">The following is a JSON representation of the resource.</span></span>

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
