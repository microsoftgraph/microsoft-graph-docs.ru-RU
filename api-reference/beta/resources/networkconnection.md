---
title: Тип ресурса networkConnection
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
ms.openlocfilehash: ce7de8d5a0f63c4d924e8092e4e9e05f984ec335
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570724"
---
# <a name="networkconnection-resource-type"></a><span data-ttu-id="0f646-104">Тип ресурса networkConnection</span><span class="sxs-lookup"><span data-stu-id="0f646-104">networkConnection resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f646-105">Содержит сведения о состоянии сетевого подключения, связанного с оповещением.</span><span class="sxs-lookup"><span data-stu-id="0f646-105">Contains stateful information about the network connection related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="0f646-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="0f646-106">Properties</span></span>

| <span data-ttu-id="0f646-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="0f646-107">Property</span></span>   | <span data-ttu-id="0f646-108">Тип</span><span class="sxs-lookup"><span data-stu-id="0f646-108">Type</span></span>|<span data-ttu-id="0f646-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0f646-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0f646-110">applicationName</span><span class="sxs-lookup"><span data-stu-id="0f646-110">applicationName</span></span>|<span data-ttu-id="0f646-111">String</span><span class="sxs-lookup"><span data-stu-id="0f646-111">String</span></span>|<span data-ttu-id="0f646-112">Имя приложения, управляющего сетевым подключением (например, Facebook, SMTP и т. д.).</span><span class="sxs-lookup"><span data-stu-id="0f646-112">Name of the application managing the network connection (for example, Facebook, SMTP, etc.).</span></span>|
|<span data-ttu-id="0f646-113">Дестинатионаддресс</span><span class="sxs-lookup"><span data-stu-id="0f646-113">destinationAddress</span></span>|<span data-ttu-id="0f646-114">String</span><span class="sxs-lookup"><span data-stu-id="0f646-114">String</span></span>|<span data-ttu-id="0f646-115">Конечный IP-адрес (сетевого подключения).</span><span class="sxs-lookup"><span data-stu-id="0f646-115">Destination IP address (of the network connection).</span></span>|
|<span data-ttu-id="0f646-116">Дестинатиондомаин</span><span class="sxs-lookup"><span data-stu-id="0f646-116">destinationDomain</span></span>|<span data-ttu-id="0f646-117">String</span><span class="sxs-lookup"><span data-stu-id="0f646-117">String</span></span>|<span data-ttu-id="0f646-118">Часть конечного домена, в которой находится конечный URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="0f646-118">Destination domain portion of the destination URL.</span></span> <span data-ttu-id="0f646-119">(например, "www.contoso.com").</span><span class="sxs-lookup"><span data-stu-id="0f646-119">(for example 'www.contoso.com').</span></span>|
|<span data-ttu-id="0f646-120">Дестинатионпорт</span><span class="sxs-lookup"><span data-stu-id="0f646-120">destinationPort</span></span>|<span data-ttu-id="0f646-121">String</span><span class="sxs-lookup"><span data-stu-id="0f646-121">String</span></span>|<span data-ttu-id="0f646-122">Порт назначения (для сетевого подключения).</span><span class="sxs-lookup"><span data-stu-id="0f646-122">Destination port (of the network connection).</span></span>|
|<span data-ttu-id="0f646-123">Дестинатионурл</span><span class="sxs-lookup"><span data-stu-id="0f646-123">destinationUrl</span></span>|<span data-ttu-id="0f646-124">String</span><span class="sxs-lookup"><span data-stu-id="0f646-124">String</span></span>|<span data-ttu-id="0f646-125">URL-адрес сетевого подключения/URI-строка — без параметров.</span><span class="sxs-lookup"><span data-stu-id="0f646-125">Network connection URL/URI string - excluding parameters.</span></span> <span data-ttu-id="0f646-126">(например, "www.contoso.com/products/Default.HTML")</span><span class="sxs-lookup"><span data-stu-id="0f646-126">(for example 'www.contoso.com/products/default.html')</span></span>|
|<span data-ttu-id="0f646-127">direction</span><span class="sxs-lookup"><span data-stu-id="0f646-127">direction</span></span>|<span data-ttu-id="0f646-128">connectionDirection</span><span class="sxs-lookup"><span data-stu-id="0f646-128">connectionDirection</span></span>|<span data-ttu-id="0f646-129">Направление сетевого подключения.</span><span class="sxs-lookup"><span data-stu-id="0f646-129">Network connection direction.</span></span> <span data-ttu-id="0f646-130">Возможные значения: `unknown`, `inbound`, `outbound`.</span><span class="sxs-lookup"><span data-stu-id="0f646-130">Possible values are: `unknown`, `inbound`, `outbound`.</span></span>|
|<span data-ttu-id="0f646-131">Домаинрегистереддатетиме</span><span class="sxs-lookup"><span data-stu-id="0f646-131">domainRegisteredDateTime</span></span>|<span data-ttu-id="0f646-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f646-132">DateTimeOffset</span></span>|<span data-ttu-id="0f646-133">Дата регистрации конечного домена.</span><span class="sxs-lookup"><span data-stu-id="0f646-133">Date when the destination domain was registered.</span></span> <span data-ttu-id="0f646-134">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="0f646-134">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0f646-135">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="0f646-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="0f646-136">Локалднснаме</span><span class="sxs-lookup"><span data-stu-id="0f646-136">localDnsName</span></span>|<span data-ttu-id="0f646-137">String</span><span class="sxs-lookup"><span data-stu-id="0f646-137">String</span></span>|<span data-ttu-id="0f646-138">Локальное разрешение DNS-имен, отображаемое в локальном кэше DNS узла (например, на случай, если файл hosts был подделан).</span><span class="sxs-lookup"><span data-stu-id="0f646-138">The local DNS name resolution as it appears in the host's local DNS cache (for example, in case the 'hosts' file was tampered with).</span></span>|
|<span data-ttu-id="0f646-139">Натдестинатионаддресс</span><span class="sxs-lookup"><span data-stu-id="0f646-139">natDestinationAddress</span></span>|<span data-ttu-id="0f646-140">String</span><span class="sxs-lookup"><span data-stu-id="0f646-140">String</span></span>|<span data-ttu-id="0f646-141">IP-адрес назначения преобразования сетевых адресов.</span><span class="sxs-lookup"><span data-stu-id="0f646-141">Network Address Translation destination IP address.</span></span>|
|<span data-ttu-id="0f646-142">Натдестинатионпорт</span><span class="sxs-lookup"><span data-stu-id="0f646-142">natDestinationPort</span></span>|<span data-ttu-id="0f646-143">String</span><span class="sxs-lookup"><span data-stu-id="0f646-143">String</span></span>|<span data-ttu-id="0f646-144">Порт назначения преобразования сетевых адресов.</span><span class="sxs-lookup"><span data-stu-id="0f646-144">Network Address Translation destination port.</span></span>|
|<span data-ttu-id="0f646-145">Натсаурцеаддресс</span><span class="sxs-lookup"><span data-stu-id="0f646-145">natSourceAddress</span></span>|<span data-ttu-id="0f646-146">String</span><span class="sxs-lookup"><span data-stu-id="0f646-146">String</span></span>|<span data-ttu-id="0f646-147">IP-адрес источника преобразования сетевых адресов.</span><span class="sxs-lookup"><span data-stu-id="0f646-147">Network Address Translation source IP address.</span></span>|
|<span data-ttu-id="0f646-148">Натсаурцепорт</span><span class="sxs-lookup"><span data-stu-id="0f646-148">natSourcePort</span></span>|<span data-ttu-id="0f646-149">String</span><span class="sxs-lookup"><span data-stu-id="0f646-149">String</span></span>|<span data-ttu-id="0f646-150">Порт источника преобразования сетевых адресов.</span><span class="sxs-lookup"><span data-stu-id="0f646-150">Network Address Translation source port.</span></span>|
|<span data-ttu-id="0f646-151">Protocol</span><span class="sxs-lookup"><span data-stu-id="0f646-151">protocol</span></span>|[<span data-ttu-id="0f646-152">securityNetworkProtocol</span><span class="sxs-lookup"><span data-stu-id="0f646-152">securityNetworkProtocol</span></span>](securitynetworkprotocolenumtype.md)|<span data-ttu-id="0f646-153">Сетевой протокол.</span><span class="sxs-lookup"><span data-stu-id="0f646-153">Network protocol.</span></span> <span data-ttu-id="0f646-154">Возможные значения: `unknown`, `ip`, `icmp`, `igmp` `ggp` `ipv4` `tcp` `ipSecEncapsulatingSecurityPayload` `ipSecAuthenticationHeader` `icmpV6` `ipv6NoNextHeader` `ipv6DestinationOptions` `nd` `ipv6RoutingHeader` `ipv6FragmentHeader`,,,,,,,,,,,,,,,,,,,,, `pup` `udp` `idp` `ipv6` , `raw`, `ipx`, `spx`, `spxII`.</span><span class="sxs-lookup"><span data-stu-id="0f646-154">Possible values are: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd`, `raw`, `ipx`, `spx`, `spxII`.</span></span>|
|<span data-ttu-id="0f646-155">riskScore</span><span class="sxs-lookup"><span data-stu-id="0f646-155">riskScore</span></span>|<span data-ttu-id="0f646-156">String</span><span class="sxs-lookup"><span data-stu-id="0f646-156">String</span></span>|<span data-ttu-id="0f646-157">Созданный поставщиком/вычисляемый показатель риска для сетевого подключения.</span><span class="sxs-lookup"><span data-stu-id="0f646-157">Provider generated/calculated risk score of the network connection.</span></span> <span data-ttu-id="0f646-158">Рекомендуемый диапазон значений 0-1, указывающий на процентное соотношение.</span><span class="sxs-lookup"><span data-stu-id="0f646-158">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="0f646-159">Саурцеаддресс</span><span class="sxs-lookup"><span data-stu-id="0f646-159">sourceAddress</span></span>|<span data-ttu-id="0f646-160">String</span><span class="sxs-lookup"><span data-stu-id="0f646-160">String</span></span>|<span data-ttu-id="0f646-161">Источник (то есть источник) IP-адрес сетевого подключения.</span><span class="sxs-lookup"><span data-stu-id="0f646-161">Source (i.e. origin) IP address (of the network connection).</span></span>|
|<span data-ttu-id="0f646-162">Саурцепорт</span><span class="sxs-lookup"><span data-stu-id="0f646-162">sourcePort</span></span>|<span data-ttu-id="0f646-163">String</span><span class="sxs-lookup"><span data-stu-id="0f646-163">String</span></span>|<span data-ttu-id="0f646-164">Исходный (то есть источник) IP-порт (сетевого подключения).</span><span class="sxs-lookup"><span data-stu-id="0f646-164">Source (i.e. origin) IP port (of the network connection).</span></span>|
|<span data-ttu-id="0f646-165">status</span><span class="sxs-lookup"><span data-stu-id="0f646-165">status</span></span>|<span data-ttu-id="0f646-166">connectionStatus</span><span class="sxs-lookup"><span data-stu-id="0f646-166">connectionStatus</span></span>|<span data-ttu-id="0f646-167">Состояние сетевого подключения.</span><span class="sxs-lookup"><span data-stu-id="0f646-167">Network connection status.</span></span> <span data-ttu-id="0f646-168">Возможные значения: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="0f646-168">Possible values are: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span></span>|
|<span data-ttu-id="0f646-169">Урлпараметерс</span><span class="sxs-lookup"><span data-stu-id="0f646-169">urlParameters</span></span>|<span data-ttu-id="0f646-170">String</span><span class="sxs-lookup"><span data-stu-id="0f646-170">String</span></span>|<span data-ttu-id="0f646-171">Параметры (суффикс) конечного URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="0f646-171">Parameters (suffix) of the destination URL.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0f646-172">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0f646-172">JSON representation</span></span>

<span data-ttu-id="0f646-173">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0f646-173">The following is a JSON representation of the resource.</span></span>

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
