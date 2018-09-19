# <a name="networkconnection-resource-type"></a><span data-ttu-id="ca1ed-101">Тип ресурса networkConnection</span><span class="sxs-lookup"><span data-stu-id="ca1ed-101">networkConnection resource type</span></span>

<span data-ttu-id="ca1ed-102">Содержит информацию о состоянии сетевого подключения, связанного с оповещением.</span><span class="sxs-lookup"><span data-stu-id="ca1ed-102">Contains stateful information about the network connection related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="ca1ed-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="ca1ed-103">Properties</span></span>

| <span data-ttu-id="ca1ed-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="ca1ed-104">Property</span></span>   | <span data-ttu-id="ca1ed-105">Тип</span><span class="sxs-lookup"><span data-stu-id="ca1ed-105">Type</span></span>|<span data-ttu-id="ca1ed-106">Описание</span><span class="sxs-lookup"><span data-stu-id="ca1ed-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ca1ed-107">applicationName</span><span class="sxs-lookup"><span data-stu-id="ca1ed-107">applicationName</span></span>|<span data-ttu-id="ca1ed-108">String</span><span class="sxs-lookup"><span data-stu-id="ca1ed-108">String</span></span>|<span data-ttu-id="ca1ed-109">Имя приложения, управляющее сетевым подключением (например, Facebook, SMTP, и т.д.).</span><span class="sxs-lookup"><span data-stu-id="ca1ed-109">Name of the application managing the network connection (for example, Facebook, SMTP, etc.).</span></span>|
|<span data-ttu-id="ca1ed-110">destinationAddress</span><span class="sxs-lookup"><span data-stu-id="ca1ed-110">destinationAddress</span></span>|<span data-ttu-id="ca1ed-111">String</span><span class="sxs-lookup"><span data-stu-id="ca1ed-111">String</span></span>|<span data-ttu-id="ca1ed-112">Конечный IP-адрес (сетевого подключения).</span><span class="sxs-lookup"><span data-stu-id="ca1ed-112">Destination IP address (of the network connection).</span></span>|
|<span data-ttu-id="ca1ed-113">destinationDomain</span><span class="sxs-lookup"><span data-stu-id="ca1ed-113">destinationDomain</span></span>|<span data-ttu-id="ca1ed-114">String</span><span class="sxs-lookup"><span data-stu-id="ca1ed-114">String</span></span>|<span data-ttu-id="ca1ed-115">Часть домена назначения URL-адреса назначения.</span><span class="sxs-lookup"><span data-stu-id="ca1ed-115">Destination domain portion of the destination URL.</span></span> <span data-ttu-id="ca1ed-116">(например, "www.contoso.com").</span><span class="sxs-lookup"><span data-stu-id="ca1ed-116">(for example 'www.contoso.com').</span></span>|
|<span data-ttu-id="ca1ed-117">destinationPort</span><span class="sxs-lookup"><span data-stu-id="ca1ed-117">destinationPort</span></span>|<span data-ttu-id="ca1ed-118">String</span><span class="sxs-lookup"><span data-stu-id="ca1ed-118">String</span></span>|<span data-ttu-id="ca1ed-119">Порт назначения (сетевого подключения).</span><span class="sxs-lookup"><span data-stu-id="ca1ed-119">Destination port (of the network connection).</span></span>|
|<span data-ttu-id="ca1ed-120">destinationUrl</span><span class="sxs-lookup"><span data-stu-id="ca1ed-120">destinationUrl</span></span>|<span data-ttu-id="ca1ed-121">String</span><span class="sxs-lookup"><span data-stu-id="ca1ed-121">String</span></span>|<span data-ttu-id="ca1ed-122">Строка URL/URI сетевого подключения - исключая параметры.</span><span class="sxs-lookup"><span data-stu-id="ca1ed-122">Network connection URL/URI string - excluding parameters.</span></span> <span data-ttu-id="ca1ed-123">(например, «www.contoso.com/products/default.html»)</span><span class="sxs-lookup"><span data-stu-id="ca1ed-123">(for example 'www.contoso.com/products/default.html')</span></span>|
|<span data-ttu-id="ca1ed-124">direction</span><span class="sxs-lookup"><span data-stu-id="ca1ed-124">direction</span></span>|<span data-ttu-id="ca1ed-125">connectionDirection</span><span class="sxs-lookup"><span data-stu-id="ca1ed-125">connectionDirection</span></span>|<span data-ttu-id="ca1ed-126">Направление сетевого подключения.</span><span class="sxs-lookup"><span data-stu-id="ca1ed-126">Network connection direction.</span></span> <span data-ttu-id="ca1ed-127">Возможные значения: `unknown`, `inbound`, `outbound`.</span><span class="sxs-lookup"><span data-stu-id="ca1ed-127">Possible values are: `unknown`, `inbound`, `outbound`.</span></span>|
|<span data-ttu-id="ca1ed-128">domainRegisteredDateTime</span><span class="sxs-lookup"><span data-stu-id="ca1ed-128">domainRegisteredDateTime</span></span>|<span data-ttu-id="ca1ed-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca1ed-129">DateTimeOffset</span></span>|<span data-ttu-id="ca1ed-130">Дата регистрации домена назначения.</span><span class="sxs-lookup"><span data-stu-id="ca1ed-130">Date when the destination domain was registered.</span></span> <span data-ttu-id="ca1ed-131">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется часовой пояс UTC).</span><span class="sxs-lookup"><span data-stu-id="ca1ed-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ca1ed-132">Например, полночь 1 января 2014 года в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="ca1ed-132">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="ca1ed-133">localDnsName</span><span class="sxs-lookup"><span data-stu-id="ca1ed-133">localDnsName</span></span>|<span data-ttu-id="ca1ed-134">String</span><span class="sxs-lookup"><span data-stu-id="ca1ed-134">String</span></span>|<span data-ttu-id="ca1ed-135">Локальное разрешение DNS-имени в том виде, в котором оно отображается в локальном DNS-кэше (например, в случае замены файла "hosts").</span><span class="sxs-lookup"><span data-stu-id="ca1ed-135">The local DNS name resolution as it appears in the host's local DNS cache (for example, in case the 'hosts' file was tampered with).</span></span>|
|<span data-ttu-id="ca1ed-136">natDestinationAddress</span><span class="sxs-lookup"><span data-stu-id="ca1ed-136">natDestinationAddress</span></span>|<span data-ttu-id="ca1ed-137">String</span><span class="sxs-lookup"><span data-stu-id="ca1ed-137">String</span></span>|<span data-ttu-id="ca1ed-138">Назначение IP-адреса преобразования сетевых адресов.</span><span class="sxs-lookup"><span data-stu-id="ca1ed-138">Network Address Translation destination IP address.</span></span>|
|<span data-ttu-id="ca1ed-139">natDestinationPort</span><span class="sxs-lookup"><span data-stu-id="ca1ed-139">natDestinationPort</span></span>|<span data-ttu-id="ca1ed-140">String</span><span class="sxs-lookup"><span data-stu-id="ca1ed-140">String</span></span>|<span data-ttu-id="ca1ed-141">Конечный порт преобразования сетевых адресов.</span><span class="sxs-lookup"><span data-stu-id="ca1ed-141">Network Address Translation destination port.</span></span>|
|<span data-ttu-id="ca1ed-142">natSourceAddress</span><span class="sxs-lookup"><span data-stu-id="ca1ed-142">natSourceAddress</span></span>|<span data-ttu-id="ca1ed-143">String</span><span class="sxs-lookup"><span data-stu-id="ca1ed-143">String</span></span>|<span data-ttu-id="ca1ed-144">Исходный IP-адрес преобразования сетевых адресов.</span><span class="sxs-lookup"><span data-stu-id="ca1ed-144">Network Address Translation source IP address.</span></span>|
|<span data-ttu-id="ca1ed-145">natSourcePort</span><span class="sxs-lookup"><span data-stu-id="ca1ed-145">natSourcePort</span></span>|<span data-ttu-id="ca1ed-146">String</span><span class="sxs-lookup"><span data-stu-id="ca1ed-146">String</span></span>|<span data-ttu-id="ca1ed-147">Исходный порт преобразования сетевых адресов.</span><span class="sxs-lookup"><span data-stu-id="ca1ed-147">Network Address Translation source port.</span></span>|
|<span data-ttu-id="ca1ed-148">protocol</span><span class="sxs-lookup"><span data-stu-id="ca1ed-148">protocol</span></span>|[<span data-ttu-id="ca1ed-149">securityNetworkProtocol</span><span class="sxs-lookup"><span data-stu-id="ca1ed-149">securityNetworkProtocol</span></span>](securitynetworkprotocol.md)|<span data-ttu-id="ca1ed-150">Сетевой протокол.</span><span class="sxs-lookup"><span data-stu-id="ca1ed-150">Network protocol analysis</span></span> <span data-ttu-id="ca1ed-151">Возможные значения: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd`, `raw`, `ipx`, `spx`, `spxII`.</span><span class="sxs-lookup"><span data-stu-id="ca1ed-151">Possible values are: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd`, `raw`, `ipx`.</span></span>|
|<span data-ttu-id="ca1ed-152">riskScore</span><span class="sxs-lookup"><span data-stu-id="ca1ed-152">riskScore</span></span>|<span data-ttu-id="ca1ed-153">String</span><span class="sxs-lookup"><span data-stu-id="ca1ed-153">String</span></span>|<span data-ttu-id="ca1ed-154">Поставщик создал/вычислил оценку риска для сетевого подключения.</span><span class="sxs-lookup"><span data-stu-id="ca1ed-154">Provider generated/calculated risk score of the network connection.</span></span> <span data-ttu-id="ca1ed-155">Рекомендуемый диапазон значений: от 0 до 1, что соответствует величине в процентах.</span><span class="sxs-lookup"><span data-stu-id="ca1ed-155">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="ca1ed-156">sourceAddress</span><span class="sxs-lookup"><span data-stu-id="ca1ed-156">sourceAddress</span></span>|<span data-ttu-id="ca1ed-157">String</span><span class="sxs-lookup"><span data-stu-id="ca1ed-157">String</span></span>|<span data-ttu-id="ca1ed-158">Источник (т.е. исходный объект) IP-адреса (сетевого подключения).</span><span class="sxs-lookup"><span data-stu-id="ca1ed-158">Source (i.e. origin) IP address (of the network connection).</span></span>|
|<span data-ttu-id="ca1ed-159">SourcePort</span><span class="sxs-lookup"><span data-stu-id="ca1ed-159">sourcePort</span></span>|<span data-ttu-id="ca1ed-160">String</span><span class="sxs-lookup"><span data-stu-id="ca1ed-160">String</span></span>|<span data-ttu-id="ca1ed-161">Источник (т.е. исходный объект) IP-адреса порта (сетевого подключения).</span><span class="sxs-lookup"><span data-stu-id="ca1ed-161">Source (i.e. origin) IP port (of the network connection).</span></span>|
|<span data-ttu-id="ca1ed-162">status</span><span class="sxs-lookup"><span data-stu-id="ca1ed-162">status</span></span>|<span data-ttu-id="ca1ed-163">connectionStatus</span><span class="sxs-lookup"><span data-stu-id="ca1ed-163">ConnectionStatus</span></span>|<span data-ttu-id="ca1ed-164">Состояние сетевого подключения.</span><span class="sxs-lookup"><span data-stu-id="ca1ed-164">Network connection status.</span></span> <span data-ttu-id="ca1ed-165">Возможные значения: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="ca1ed-165">Possible values are: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span></span>|
|<span data-ttu-id="ca1ed-166">urlParameters</span><span class="sxs-lookup"><span data-stu-id="ca1ed-166">urlParameters</span></span>|<span data-ttu-id="ca1ed-167">String</span><span class="sxs-lookup"><span data-stu-id="ca1ed-167">String</span></span>|<span data-ttu-id="ca1ed-168">Параметры (суффикс) URL-адреса назначения.</span><span class="sxs-lookup"><span data-stu-id="ca1ed-168">Parameters (suffix) of the destination URL.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ca1ed-169">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ca1ed-169">JSON representation</span></span>

<span data-ttu-id="ca1ed-170">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ca1ed-170">The following is a JSON representation of the resource.</span></span>

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