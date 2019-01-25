---
title: Тип ресурса networkConnection
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
ms.openlocfilehash: ce7de8d5a0f63c4d924e8092e4e9e05f984ec335
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515358"
---
# <a name="networkconnection-resource-type"></a><span data-ttu-id="2089b-104">Тип ресурса networkConnection</span><span class="sxs-lookup"><span data-stu-id="2089b-104">networkConnection resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2089b-105">Содержит информацию о состояниях о сетевое подключение, связанные с оповещение.</span><span class="sxs-lookup"><span data-stu-id="2089b-105">Contains stateful information about the network connection related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="2089b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="2089b-106">Properties</span></span>

| <span data-ttu-id="2089b-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="2089b-107">Property</span></span>   | <span data-ttu-id="2089b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="2089b-108">Type</span></span>|<span data-ttu-id="2089b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2089b-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2089b-110">applicationName</span><span class="sxs-lookup"><span data-stu-id="2089b-110">applicationName</span></span>|<span data-ttu-id="2089b-111">String</span><span class="sxs-lookup"><span data-stu-id="2089b-111">String</span></span>|<span data-ttu-id="2089b-112">Имя приложения, управление сетевое подключение (например, Facebook, SMTP, и т.д.).</span><span class="sxs-lookup"><span data-stu-id="2089b-112">Name of the application managing the network connection (for example, Facebook, SMTP, etc.).</span></span>|
|<span data-ttu-id="2089b-113">destinationAddress</span><span class="sxs-lookup"><span data-stu-id="2089b-113">destinationAddress</span></span>|<span data-ttu-id="2089b-114">String</span><span class="sxs-lookup"><span data-stu-id="2089b-114">String</span></span>|<span data-ttu-id="2089b-115">Конечный IP-адрес (сетевое подключение).</span><span class="sxs-lookup"><span data-stu-id="2089b-115">Destination IP address (of the network connection).</span></span>|
|<span data-ttu-id="2089b-116">destinationDomain</span><span class="sxs-lookup"><span data-stu-id="2089b-116">destinationDomain</span></span>|<span data-ttu-id="2089b-117">String</span><span class="sxs-lookup"><span data-stu-id="2089b-117">String</span></span>|<span data-ttu-id="2089b-118">Часть домена конечный URL-адрес назначения.</span><span class="sxs-lookup"><span data-stu-id="2089b-118">Destination domain portion of the destination URL.</span></span> <span data-ttu-id="2089b-119">(например «www.contoso.com»).</span><span class="sxs-lookup"><span data-stu-id="2089b-119">(for example 'www.contoso.com').</span></span>|
|<span data-ttu-id="2089b-120">destinationPort</span><span class="sxs-lookup"><span data-stu-id="2089b-120">destinationPort</span></span>|<span data-ttu-id="2089b-121">String</span><span class="sxs-lookup"><span data-stu-id="2089b-121">String</span></span>|<span data-ttu-id="2089b-122">Порт назначения (сетевое подключение).</span><span class="sxs-lookup"><span data-stu-id="2089b-122">Destination port (of the network connection).</span></span>|
|<span data-ttu-id="2089b-123">destinationUrl</span><span class="sxs-lookup"><span data-stu-id="2089b-123">destinationUrl</span></span>|<span data-ttu-id="2089b-124">String</span><span class="sxs-lookup"><span data-stu-id="2089b-124">String</span></span>|<span data-ttu-id="2089b-125">Строка подключения URL-адрес или URI - исключение параметров в сети.</span><span class="sxs-lookup"><span data-stu-id="2089b-125">Network connection URL/URI string - excluding parameters.</span></span> <span data-ttu-id="2089b-126">(например, «www.contoso.com/products/default.html»)</span><span class="sxs-lookup"><span data-stu-id="2089b-126">(for example 'www.contoso.com/products/default.html')</span></span>|
|<span data-ttu-id="2089b-127">Direction</span><span class="sxs-lookup"><span data-stu-id="2089b-127">direction</span></span>|<span data-ttu-id="2089b-128">connectionDirection</span><span class="sxs-lookup"><span data-stu-id="2089b-128">connectionDirection</span></span>|<span data-ttu-id="2089b-129">Направление подключения к сети.</span><span class="sxs-lookup"><span data-stu-id="2089b-129">Network connection direction.</span></span> <span data-ttu-id="2089b-130">Возможные значения: `unknown`, `inbound`, `outbound`.</span><span class="sxs-lookup"><span data-stu-id="2089b-130">Possible values are: `unknown`, `inbound`, `outbound`.</span></span>|
|<span data-ttu-id="2089b-131">domainRegisteredDateTime</span><span class="sxs-lookup"><span data-stu-id="2089b-131">domainRegisteredDateTime</span></span>|<span data-ttu-id="2089b-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2089b-132">DateTimeOffset</span></span>|<span data-ttu-id="2089b-133">Дата регистрации целевом домене.</span><span class="sxs-lookup"><span data-stu-id="2089b-133">Date when the destination domain was registered.</span></span> <span data-ttu-id="2089b-134">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="2089b-134">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2089b-135">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="2089b-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="2089b-136">localDnsName</span><span class="sxs-lookup"><span data-stu-id="2089b-136">localDnsName</span></span>|<span data-ttu-id="2089b-137">String</span><span class="sxs-lookup"><span data-stu-id="2089b-137">String</span></span>|<span data-ttu-id="2089b-138">Локальное разрешение имен DNS как оно отображается в локальном кэше DNS узла (например, в случае подделано файл «hosts»).</span><span class="sxs-lookup"><span data-stu-id="2089b-138">The local DNS name resolution as it appears in the host's local DNS cache (for example, in case the 'hosts' file was tampered with).</span></span>|
|<span data-ttu-id="2089b-139">natDestinationAddress</span><span class="sxs-lookup"><span data-stu-id="2089b-139">natDestinationAddress</span></span>|<span data-ttu-id="2089b-140">String</span><span class="sxs-lookup"><span data-stu-id="2089b-140">String</span></span>|<span data-ttu-id="2089b-141">Преобразование адресов конечный IP-адрес в сети.</span><span class="sxs-lookup"><span data-stu-id="2089b-141">Network Address Translation destination IP address.</span></span>|
|<span data-ttu-id="2089b-142">natDestinationPort</span><span class="sxs-lookup"><span data-stu-id="2089b-142">natDestinationPort</span></span>|<span data-ttu-id="2089b-143">String</span><span class="sxs-lookup"><span data-stu-id="2089b-143">String</span></span>|<span data-ttu-id="2089b-144">Конечный порт преобразование адресов в сети.</span><span class="sxs-lookup"><span data-stu-id="2089b-144">Network Address Translation destination port.</span></span>|
|<span data-ttu-id="2089b-145">natSourceAddress</span><span class="sxs-lookup"><span data-stu-id="2089b-145">natSourceAddress</span></span>|<span data-ttu-id="2089b-146">String</span><span class="sxs-lookup"><span data-stu-id="2089b-146">String</span></span>|<span data-ttu-id="2089b-147">Преобразование адресов исходный IP-адрес в сети.</span><span class="sxs-lookup"><span data-stu-id="2089b-147">Network Address Translation source IP address.</span></span>|
|<span data-ttu-id="2089b-148">natSourcePort</span><span class="sxs-lookup"><span data-stu-id="2089b-148">natSourcePort</span></span>|<span data-ttu-id="2089b-149">String</span><span class="sxs-lookup"><span data-stu-id="2089b-149">String</span></span>|<span data-ttu-id="2089b-150">Порт источника, преобразование адресов сети.</span><span class="sxs-lookup"><span data-stu-id="2089b-150">Network Address Translation source port.</span></span>|
|<span data-ttu-id="2089b-151">protocol</span><span class="sxs-lookup"><span data-stu-id="2089b-151">protocol</span></span>|[<span data-ttu-id="2089b-152">securityNetworkProtocol</span><span class="sxs-lookup"><span data-stu-id="2089b-152">securityNetworkProtocol</span></span>](securitynetworkprotocolenumtype.md)|<span data-ttu-id="2089b-153">Сетевой протокол.</span><span class="sxs-lookup"><span data-stu-id="2089b-153">Network protocol.</span></span> <span data-ttu-id="2089b-154">Возможные значения: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd` , `raw`, `ipx`, `spx`, `spxII`.</span><span class="sxs-lookup"><span data-stu-id="2089b-154">Possible values are: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd`, `raw`, `ipx`, `spx`, `spxII`.</span></span>|
|<span data-ttu-id="2089b-155">riskScore</span><span class="sxs-lookup"><span data-stu-id="2089b-155">riskScore</span></span>|<span data-ttu-id="2089b-156">String</span><span class="sxs-lookup"><span data-stu-id="2089b-156">String</span></span>|<span data-ttu-id="2089b-157">Поставщик создан/вычисляется риск показатель для подключения к сети.</span><span class="sxs-lookup"><span data-stu-id="2089b-157">Provider generated/calculated risk score of the network connection.</span></span> <span data-ttu-id="2089b-158">Рекомендуемое значение диапазона 0-1, который соответствует в процентах.</span><span class="sxs-lookup"><span data-stu-id="2089b-158">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="2089b-159">sourceAddress</span><span class="sxs-lookup"><span data-stu-id="2089b-159">sourceAddress</span></span>|<span data-ttu-id="2089b-160">String</span><span class="sxs-lookup"><span data-stu-id="2089b-160">String</span></span>|<span data-ttu-id="2089b-161">(То есть источник) IP-адрес источника (сетевое подключение).</span><span class="sxs-lookup"><span data-stu-id="2089b-161">Source (i.e. origin) IP address (of the network connection).</span></span>|
|<span data-ttu-id="2089b-162">sourcePort</span><span class="sxs-lookup"><span data-stu-id="2089b-162">sourcePort</span></span>|<span data-ttu-id="2089b-163">String</span><span class="sxs-lookup"><span data-stu-id="2089b-163">String</span></span>|<span data-ttu-id="2089b-164">Исходный (то есть источник) IP-адрес порт (сетевое подключение).</span><span class="sxs-lookup"><span data-stu-id="2089b-164">Source (i.e. origin) IP port (of the network connection).</span></span>|
|<span data-ttu-id="2089b-165">status</span><span class="sxs-lookup"><span data-stu-id="2089b-165">status</span></span>|<span data-ttu-id="2089b-166">connectionStatus</span><span class="sxs-lookup"><span data-stu-id="2089b-166">connectionStatus</span></span>|<span data-ttu-id="2089b-167">Состояние подключения к сети.</span><span class="sxs-lookup"><span data-stu-id="2089b-167">Network connection status.</span></span> <span data-ttu-id="2089b-168">Возможные значения: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="2089b-168">Possible values are: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span></span>|
|<span data-ttu-id="2089b-169">urlParameters</span><span class="sxs-lookup"><span data-stu-id="2089b-169">urlParameters</span></span>|<span data-ttu-id="2089b-170">String</span><span class="sxs-lookup"><span data-stu-id="2089b-170">String</span></span>|<span data-ttu-id="2089b-171">Параметры (суффикс) URL-адрес назначения.</span><span class="sxs-lookup"><span data-stu-id="2089b-171">Parameters (suffix) of the destination URL.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2089b-172">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2089b-172">JSON representation</span></span>

<span data-ttu-id="2089b-173">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2089b-173">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "networkConnection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/networkconnection.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
