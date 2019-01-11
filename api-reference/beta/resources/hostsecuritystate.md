---
title: Тип ресурса hostSecurityState
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
ms.openlocfilehash: 1ae1436dd9771d34c37542eb756f81a4f8f0306a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853377"
---
# <a name="hostsecuritystate-resource-type"></a><span data-ttu-id="49a33-104">Тип ресурса hostSecurityState</span><span class="sxs-lookup"><span data-stu-id="49a33-104">hostSecurityState resource type</span></span>

 > <span data-ttu-id="49a33-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="49a33-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="49a33-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="49a33-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="49a33-107">Содержит с сохранением состояния сведения об узле (включая устройства, компьютеры и т. п.).</span><span class="sxs-lookup"><span data-stu-id="49a33-107">Contains stateful information about the host (including devices, computers, and so on).</span></span>

## <a name="properties"></a><span data-ttu-id="49a33-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="49a33-108">Properties</span></span>

| <span data-ttu-id="49a33-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="49a33-109">Property</span></span>   | <span data-ttu-id="49a33-110">Тип</span><span class="sxs-lookup"><span data-stu-id="49a33-110">Type</span></span>|<span data-ttu-id="49a33-111">Описание</span><span class="sxs-lookup"><span data-stu-id="49a33-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="49a33-112">полное доменное имя</span><span class="sxs-lookup"><span data-stu-id="49a33-112">fqdn</span></span>|<span data-ttu-id="49a33-113">Строка</span><span class="sxs-lookup"><span data-stu-id="49a33-113">String</span></span>|<span data-ttu-id="49a33-114">Полное доменное имя (полное доменное имя) (например, machine.company.com) узла.</span><span class="sxs-lookup"><span data-stu-id="49a33-114">Host FQDN (Fully Qualified Domain Name) (for example, machine.company.com).</span></span>|
|<span data-ttu-id="49a33-115">isAzureAadJoined</span><span class="sxs-lookup"><span data-stu-id="49a33-115">isAzureAadJoined</span></span>|<span data-ttu-id="49a33-116">Логический</span><span class="sxs-lookup"><span data-stu-id="49a33-116">Boolean</span></span>|<span data-ttu-id="49a33-117">Значение true, если узел является домен, в состав доменных служб Active Directory Azure.</span><span class="sxs-lookup"><span data-stu-id="49a33-117">True if the host is domain joined to Azure Active Directory Domain Services.</span></span>|
|<span data-ttu-id="49a33-118">isAzureAadRegistered</span><span class="sxs-lookup"><span data-stu-id="49a33-118">isAzureAadRegistered</span></span>|<span data-ttu-id="49a33-119">Логический</span><span class="sxs-lookup"><span data-stu-id="49a33-119">Boolean</span></span>|<span data-ttu-id="49a33-120">Значение true, если узел зарегистрирован устройства регистрации Azure Active Directory (BYOD устройства - то есть, не полностью управляются предприятия).</span><span class="sxs-lookup"><span data-stu-id="49a33-120">True if the host registered with Azure Active Directory Device Registration (BYOD devices - that is, not fully managed by enterprise).</span></span>|
|<span data-ttu-id="49a33-121">isHybridAzureDomainJoined</span><span class="sxs-lookup"><span data-stu-id="49a33-121">isHybridAzureDomainJoined</span></span>|<span data-ttu-id="49a33-122">Логический</span><span class="sxs-lookup"><span data-stu-id="49a33-122">Boolean</span></span>|<span data-ttu-id="49a33-123">Значение true, если узел присоединен к домену на локальный домен Active Directory.</span><span class="sxs-lookup"><span data-stu-id="49a33-123">True if the host is domain joined to an on-premises Active Directory domain.</span></span>|
|<span data-ttu-id="49a33-124">netBiosName</span><span class="sxs-lookup"><span data-stu-id="49a33-124">netBiosName</span></span>|<span data-ttu-id="49a33-125">Строка</span><span class="sxs-lookup"><span data-stu-id="49a33-125">String</span></span>|<span data-ttu-id="49a33-126">Имя локального узла без DNS-имени домена.</span><span class="sxs-lookup"><span data-stu-id="49a33-126">The local host name, without the DNS domain name.</span></span>|
|<span data-ttu-id="49a33-127">операционная система</span><span class="sxs-lookup"><span data-stu-id="49a33-127">os</span></span>|<span data-ttu-id="49a33-128">Строка</span><span class="sxs-lookup"><span data-stu-id="49a33-128">String</span></span>|<span data-ttu-id="49a33-129">Операционной системы.</span><span class="sxs-lookup"><span data-stu-id="49a33-129">Host Operating System.</span></span> <span data-ttu-id="49a33-130">(Например, Windows10, MacOS, RHEL, и т.д.).</span><span class="sxs-lookup"><span data-stu-id="49a33-130">(For example, Windows10, MacOS, RHEL, etc.).</span></span>|
|<span data-ttu-id="49a33-131">privateIpAddress</span><span class="sxs-lookup"><span data-stu-id="49a33-131">privateIpAddress</span></span>|<span data-ttu-id="49a33-132">Строка</span><span class="sxs-lookup"><span data-stu-id="49a33-132">String</span></span>|<span data-ttu-id="49a33-133">Частный (не маршрутизируемые) адрес IPv4 или IPv6 [(см)](https://tools.ietf.org/html/rfc1918)во время оповещения.</span><span class="sxs-lookup"><span data-stu-id="49a33-133">Private (not routable) IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at the time of the alert.</span></span>|
|<span data-ttu-id="49a33-134">publicIpAddress</span><span class="sxs-lookup"><span data-stu-id="49a33-134">publicIpAddress</span></span>|<span data-ttu-id="49a33-135">Строка</span><span class="sxs-lookup"><span data-stu-id="49a33-135">String</span></span>|<span data-ttu-id="49a33-136">Открыто маршрутизируемыми IPv4 или IPv6-адрес [(см)](https://tools.ietf.org/html/rfc1918)во время оповещения.</span><span class="sxs-lookup"><span data-stu-id="49a33-136">Publicly routable IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at time of the alert.</span></span>|
|<span data-ttu-id="49a33-137">riskScore</span><span class="sxs-lookup"><span data-stu-id="49a33-137">riskScore</span></span>|<span data-ttu-id="49a33-138">Строка</span><span class="sxs-lookup"><span data-stu-id="49a33-138">String</span></span>|<span data-ttu-id="49a33-139">Оценка риска поставщика создается/вычисляемые узла.</span><span class="sxs-lookup"><span data-stu-id="49a33-139">Provider-generated/calculated risk score of the host.</span></span>  <span data-ttu-id="49a33-140">Рекомендуемое значение диапазона 0-1, который соответствует в процентах.</span><span class="sxs-lookup"><span data-stu-id="49a33-140">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="49a33-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="49a33-141">JSON representation</span></span>

<span data-ttu-id="49a33-142">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="49a33-142">The following is a JSON representation of the resource.</span></span>

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
