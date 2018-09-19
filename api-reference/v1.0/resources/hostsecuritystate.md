# <a name="hostsecuritystate-resource-type"></a><span data-ttu-id="c8c79-101">тип ресурса hostSecurityState</span><span class="sxs-lookup"><span data-stu-id="c8c79-101">hostSecurityState resource type</span></span>

<span data-ttu-id="c8c79-102">Содержит сведения о состоянии узла (в том числе устройств, компьютеров и т.п.).</span><span class="sxs-lookup"><span data-stu-id="c8c79-102">Contains stateful information about the host (including devices, computers, and so on).</span></span>

## <a name="properties"></a><span data-ttu-id="c8c79-103">Свойства</span><span class="sxs-lookup"><span data-stu-id="c8c79-103">Properties</span></span>

| <span data-ttu-id="c8c79-104">Свойство</span><span class="sxs-lookup"><span data-stu-id="c8c79-104">Property</span></span>   | <span data-ttu-id="c8c79-105">Тип</span><span class="sxs-lookup"><span data-stu-id="c8c79-105">Type</span></span>|<span data-ttu-id="c8c79-106">Описание</span><span class="sxs-lookup"><span data-stu-id="c8c79-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c8c79-107">fqdn</span><span class="sxs-lookup"><span data-stu-id="c8c79-107">FQDN</span></span>|<span data-ttu-id="c8c79-108">Строка</span><span class="sxs-lookup"><span data-stu-id="c8c79-108">String</span></span>|<span data-ttu-id="c8c79-109">FQDN  (полное доменное имя) узла (например, `machine.company.com`).</span><span class="sxs-lookup"><span data-stu-id="c8c79-109">Host FQDN (Fully Qualified Domain Name) (for example, `machine.company.com`).</span></span>|
|<span data-ttu-id="c8c79-110">isAzureAadJoined</span><span class="sxs-lookup"><span data-stu-id="c8c79-110">isAzureAadJoined</span></span>|<span data-ttu-id="c8c79-111">Логический</span><span class="sxs-lookup"><span data-stu-id="c8c79-111">Boolean</span></span>|<span data-ttu-id="c8c79-112">Имеет значение true, если узел является доменом в составе доменных служб Active Directory Azure.</span><span class="sxs-lookup"><span data-stu-id="c8c79-112">True if the host is domain joined to Azure Active Directory Domain Services.</span></span>|
|<span data-ttu-id="c8c79-113">isAzureAadRegistered</span><span class="sxs-lookup"><span data-stu-id="c8c79-113">isAzureAadRegistered</span></span>|<span data-ttu-id="c8c79-114">Логический</span><span class="sxs-lookup"><span data-stu-id="c8c79-114">Boolean</span></span>|<span data-ttu-id="c8c79-115">Имеет значение true, если узел зарегистрирован в регистрации устройств Azure Active Directory (BYOD-устройства - то есть устройства, не полностью управляемые предприятием).</span><span class="sxs-lookup"><span data-stu-id="c8c79-115">True if the host registered with Azure Active Directory Device Registration (BYOD devices - that is, not fully managed by enterprise).</span></span>|
|<span data-ttu-id="c8c79-116">isHybridAzureDomainJoined</span><span class="sxs-lookup"><span data-stu-id="c8c79-116">isHybridAzureDomainJoined</span></span>|<span data-ttu-id="c8c79-117">Логический</span><span class="sxs-lookup"><span data-stu-id="c8c79-117">Boolean</span></span>|<span data-ttu-id="c8c79-118">Имеет значение true, если узел входит в локальный домен Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c8c79-118">True if the host is domain joined to an on-premises Active Directory domain.</span></span>|
|<span data-ttu-id="c8c79-119">netBiosName</span><span class="sxs-lookup"><span data-stu-id="c8c79-119">netBiosName</span></span>|<span data-ttu-id="c8c79-120">Строка</span><span class="sxs-lookup"><span data-stu-id="c8c79-120">String</span></span>|<span data-ttu-id="c8c79-121">Имя локального узла без доменного имени DNS.</span><span class="sxs-lookup"><span data-stu-id="c8c79-121">The local host name, without the DNS domain name.</span></span>|
|<span data-ttu-id="c8c79-122">os</span><span class="sxs-lookup"><span data-stu-id="c8c79-122">OS</span></span>|<span data-ttu-id="c8c79-123">Строка</span><span class="sxs-lookup"><span data-stu-id="c8c79-123">String</span></span>|<span data-ttu-id="c8c79-124">Операционная система узла.</span><span class="sxs-lookup"><span data-stu-id="c8c79-124">Host Operating System.</span></span> <span data-ttu-id="c8c79-125">(Например, Windows10, MacOS, RHEL, и т.д.).</span><span class="sxs-lookup"><span data-stu-id="c8c79-125">(For example, Windows10, MacOS, RHEL, etc.).</span></span>|
|<span data-ttu-id="c8c79-126">privateIpAddress</span><span class="sxs-lookup"><span data-stu-id="c8c79-126">privateIpAddress</span></span>|<span data-ttu-id="c8c79-127">Строка</span><span class="sxs-lookup"><span data-stu-id="c8c79-127">String</span></span>|<span data-ttu-id="c8c79-128">Частный (немаршрутизируемыц) адрес IPv4 или IPv6 (см. [RFC 1918](https://tools.ietf.org/html/rfc1918)) на момент оповещения.</span><span class="sxs-lookup"><span data-stu-id="c8c79-128">Private (not routable) IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at the time of the alert.</span></span>|
|<span data-ttu-id="c8c79-129">publicIpAddress</span><span class="sxs-lookup"><span data-stu-id="c8c79-129">publicIpAddress</span></span>|<span data-ttu-id="c8c79-130">Строка</span><span class="sxs-lookup"><span data-stu-id="c8c79-130">String</span></span>|<span data-ttu-id="c8c79-131">Общедоступный маршрутизируемый адрес IPv4 или IPv6 (см. [RFC 1918](https://tools.ietf.org/html/rfc1918)) на момент оповещения.</span><span class="sxs-lookup"><span data-stu-id="c8c79-131">Publicly routable IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at time of the alert.</span></span>|
|<span data-ttu-id="c8c79-132">riskScore</span><span class="sxs-lookup"><span data-stu-id="c8c79-132">riskScore</span></span>|<span data-ttu-id="c8c79-133">Строка</span><span class="sxs-lookup"><span data-stu-id="c8c79-133">String</span></span>|<span data-ttu-id="c8c79-134">Выполняемая поставщиком / рассчитываемая оценка рисков для узла.</span><span class="sxs-lookup"><span data-stu-id="c8c79-134">Provider-generated/calculated risk score of the host.</span></span>  <span data-ttu-id="c8c79-135">Рекомендуемый диапазон значений: от 0 до 1, что соответствует величине в процентах.</span><span class="sxs-lookup"><span data-stu-id="c8c79-135">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c8c79-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c8c79-136">JSON representation</span></span>

<span data-ttu-id="c8c79-137">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c8c79-137">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.hostSecurityState"
}-->

```json
{
  "fqdn": "String",
  "isAzureAadJoined": true,
  "isAzureAadRegistered": true,
  "isHybridAzureDomainJoined": true,
  "netBiosName": "String",
  "os": "String",
  "privateIpAddress": "String",
  "publicIpAddress": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "hostSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
