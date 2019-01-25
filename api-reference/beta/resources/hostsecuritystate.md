---
title: Тип ресурса hostSecurityState
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
ms.openlocfilehash: d6f566a2bd42163c570fe837d2419057c62664bb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526699"
---
# <a name="hostsecuritystate-resource-type"></a><span data-ttu-id="8f5b5-104">Тип ресурса hostSecurityState</span><span class="sxs-lookup"><span data-stu-id="8f5b5-104">hostSecurityState resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f5b5-105">Содержит с сохранением состояния сведения об узле (включая устройства, компьютеры и т. п.).</span><span class="sxs-lookup"><span data-stu-id="8f5b5-105">Contains stateful information about the host (including devices, computers, and so on).</span></span>

## <a name="properties"></a><span data-ttu-id="8f5b5-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="8f5b5-106">Properties</span></span>

| <span data-ttu-id="8f5b5-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="8f5b5-107">Property</span></span>   | <span data-ttu-id="8f5b5-108">Тип</span><span class="sxs-lookup"><span data-stu-id="8f5b5-108">Type</span></span>|<span data-ttu-id="8f5b5-109">Описание</span><span class="sxs-lookup"><span data-stu-id="8f5b5-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8f5b5-110">полное доменное имя</span><span class="sxs-lookup"><span data-stu-id="8f5b5-110">fqdn</span></span>|<span data-ttu-id="8f5b5-111">String</span><span class="sxs-lookup"><span data-stu-id="8f5b5-111">String</span></span>|<span data-ttu-id="8f5b5-112">Полное доменное имя (полное доменное имя) (например, machine.company.com) узла.</span><span class="sxs-lookup"><span data-stu-id="8f5b5-112">Host FQDN (Fully Qualified Domain Name) (for example, machine.company.com).</span></span>|
|<span data-ttu-id="8f5b5-113">isAzureAadJoined</span><span class="sxs-lookup"><span data-stu-id="8f5b5-113">isAzureAadJoined</span></span>|<span data-ttu-id="8f5b5-114">Логическое</span><span class="sxs-lookup"><span data-stu-id="8f5b5-114">Boolean</span></span>|<span data-ttu-id="8f5b5-115">Значение true, если узел является домен, в состав доменных служб Active Directory Azure.</span><span class="sxs-lookup"><span data-stu-id="8f5b5-115">True if the host is domain joined to Azure Active Directory Domain Services.</span></span>|
|<span data-ttu-id="8f5b5-116">isAzureAadRegistered</span><span class="sxs-lookup"><span data-stu-id="8f5b5-116">isAzureAadRegistered</span></span>|<span data-ttu-id="8f5b5-117">Логическое</span><span class="sxs-lookup"><span data-stu-id="8f5b5-117">Boolean</span></span>|<span data-ttu-id="8f5b5-118">Значение true, если узел зарегистрирован устройства регистрации Azure Active Directory (BYOD устройства - то есть, не полностью управляются предприятия).</span><span class="sxs-lookup"><span data-stu-id="8f5b5-118">True if the host registered with Azure Active Directory Device Registration (BYOD devices - that is, not fully managed by enterprise).</span></span>|
|<span data-ttu-id="8f5b5-119">isHybridAzureDomainJoined</span><span class="sxs-lookup"><span data-stu-id="8f5b5-119">isHybridAzureDomainJoined</span></span>|<span data-ttu-id="8f5b5-120">Логическое</span><span class="sxs-lookup"><span data-stu-id="8f5b5-120">Boolean</span></span>|<span data-ttu-id="8f5b5-121">Значение true, если узел присоединен к домену на локальный домен Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8f5b5-121">True if the host is domain joined to an on-premises Active Directory domain.</span></span>|
|<span data-ttu-id="8f5b5-122">netBiosName</span><span class="sxs-lookup"><span data-stu-id="8f5b5-122">netBiosName</span></span>|<span data-ttu-id="8f5b5-123">String</span><span class="sxs-lookup"><span data-stu-id="8f5b5-123">String</span></span>|<span data-ttu-id="8f5b5-124">Имя локального узла без DNS-имени домена.</span><span class="sxs-lookup"><span data-stu-id="8f5b5-124">The local host name, without the DNS domain name.</span></span>|
|<span data-ttu-id="8f5b5-125">И-5.</span><span class="sxs-lookup"><span data-stu-id="8f5b5-125">os</span></span>|<span data-ttu-id="8f5b5-126">String</span><span class="sxs-lookup"><span data-stu-id="8f5b5-126">String</span></span>|<span data-ttu-id="8f5b5-127">Операционной системы.</span><span class="sxs-lookup"><span data-stu-id="8f5b5-127">Host Operating System.</span></span> <span data-ttu-id="8f5b5-128">(Например, Windows10, MacOS, RHEL, и т.д.).</span><span class="sxs-lookup"><span data-stu-id="8f5b5-128">(For example, Windows10, MacOS, RHEL, etc.).</span></span>|
|<span data-ttu-id="8f5b5-129">privateIpAddress</span><span class="sxs-lookup"><span data-stu-id="8f5b5-129">privateIpAddress</span></span>|<span data-ttu-id="8f5b5-130">String</span><span class="sxs-lookup"><span data-stu-id="8f5b5-130">String</span></span>|<span data-ttu-id="8f5b5-131">Частный (не маршрутизируемые) адрес IPv4 или IPv6 [(см)](https://tools.ietf.org/html/rfc1918)во время оповещения.</span><span class="sxs-lookup"><span data-stu-id="8f5b5-131">Private (not routable) IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at the time of the alert.</span></span>|
|<span data-ttu-id="8f5b5-132">publicIpAddress</span><span class="sxs-lookup"><span data-stu-id="8f5b5-132">publicIpAddress</span></span>|<span data-ttu-id="8f5b5-133">String</span><span class="sxs-lookup"><span data-stu-id="8f5b5-133">String</span></span>|<span data-ttu-id="8f5b5-134">Открыто маршрутизируемыми IPv4 или IPv6-адрес [(см)](https://tools.ietf.org/html/rfc1918)во время оповещения.</span><span class="sxs-lookup"><span data-stu-id="8f5b5-134">Publicly routable IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at time of the alert.</span></span>|
|<span data-ttu-id="8f5b5-135">riskScore</span><span class="sxs-lookup"><span data-stu-id="8f5b5-135">riskScore</span></span>|<span data-ttu-id="8f5b5-136">String</span><span class="sxs-lookup"><span data-stu-id="8f5b5-136">String</span></span>|<span data-ttu-id="8f5b5-137">Оценка риска поставщика создается/вычисляемые узла.</span><span class="sxs-lookup"><span data-stu-id="8f5b5-137">Provider-generated/calculated risk score of the host.</span></span>  <span data-ttu-id="8f5b5-138">Рекомендуемое значение диапазона 0-1, который соответствует в процентах.</span><span class="sxs-lookup"><span data-stu-id="8f5b5-138">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8f5b5-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8f5b5-139">JSON representation</span></span>

<span data-ttu-id="8f5b5-140">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8f5b5-140">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "hostSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/hostsecuritystate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
