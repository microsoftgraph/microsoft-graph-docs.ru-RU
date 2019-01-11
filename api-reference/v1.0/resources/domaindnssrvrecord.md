---
title: Тип ресурса domainDnsSrvRecord
description: Представляет запись SRV, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от объекта DomainDnsRecord.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 655dc6fcbccdcb6e1794c94d97dd8e7fc4837f04
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835793"
---
# <a name="domaindnssrvrecord-resource-type"></a><span data-ttu-id="fc325-104">Тип ресурса domainDnsSrvRecord</span><span class="sxs-lookup"><span data-stu-id="fc325-104">domainDnsSrvRecord resource type</span></span>

<span data-ttu-id="fc325-p102">Представляет запись SRV, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от объекта [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="fc325-p102">Represents a SRV record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="fc325-107">Методы</span><span class="sxs-lookup"><span data-stu-id="fc325-107">Methods</span></span>
<span data-ttu-id="fc325-p103">Прямые запросы к этому ресурсу не поддерживаются. Сведения о том, как запрашивать записи службы доменов, см. в статье [о доменах](domain.md).</span><span class="sxs-lookup"><span data-stu-id="fc325-p103">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="fc325-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="fc325-110">Properties</span></span>
| <span data-ttu-id="fc325-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="fc325-111">Property</span></span>     | <span data-ttu-id="fc325-112">Тип</span><span class="sxs-lookup"><span data-stu-id="fc325-112">Type</span></span>   |<span data-ttu-id="fc325-113">Описание</span><span class="sxs-lookup"><span data-stu-id="fc325-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fc325-114">id</span><span class="sxs-lookup"><span data-stu-id="fc325-114">id</span></span>|<span data-ttu-id="fc325-115">Строка</span><span class="sxs-lookup"><span data-stu-id="fc325-115">String</span></span>| <span data-ttu-id="fc325-p104">Уникальный идентификатор, назначенный этому объекту. Не допускает значения null, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fc325-p104">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span>|
|<span data-ttu-id="fc325-118">isOptional</span><span class="sxs-lookup"><span data-stu-id="fc325-118">isOptional</span></span>|<span data-ttu-id="fc325-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc325-119">Boolean</span></span>| <span data-ttu-id="fc325-120">Если указано значение false, для правильной работы Microsoft Online Services с доменом пользователь должен настроить запись SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="fc325-120">If false, the SRV record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="fc325-121">label</span><span class="sxs-lookup"><span data-stu-id="fc325-121">label</span></span>|<span data-ttu-id="fc325-122">String</span><span class="sxs-lookup"><span data-stu-id="fc325-122">String</span></span>| <span data-ttu-id="fc325-123">Значение, используемое при настройке свойства *name* записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="fc325-123">Value used when configuring the *name* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="fc325-124">nameTarget</span><span class="sxs-lookup"><span data-stu-id="fc325-124">nameTarget</span></span>|<span data-ttu-id="fc325-125">String</span><span class="sxs-lookup"><span data-stu-id="fc325-125">String</span></span>| <span data-ttu-id="fc325-126">Значение, используемое при настройке свойства *Target* записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="fc325-126">Value to use when configuring the *Target* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="fc325-127">port</span><span class="sxs-lookup"><span data-stu-id="fc325-127">port</span></span>|<span data-ttu-id="fc325-128">Int32</span><span class="sxs-lookup"><span data-stu-id="fc325-128">Int32</span></span>| <span data-ttu-id="fc325-129">Значение, используемое при настройке свойства *port* записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="fc325-129">Value to use when configuring the *port* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="fc325-130">priority</span><span class="sxs-lookup"><span data-stu-id="fc325-130">priority</span></span>|<span data-ttu-id="fc325-131">Int32</span><span class="sxs-lookup"><span data-stu-id="fc325-131">Int32</span></span>| <span data-ttu-id="fc325-132">Значение, используемое при настройке свойства *priority* записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="fc325-132">Value to use when configuring the *priority* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="fc325-133">protocol</span><span class="sxs-lookup"><span data-stu-id="fc325-133">protocol</span></span>|<span data-ttu-id="fc325-134">String</span><span class="sxs-lookup"><span data-stu-id="fc325-134">String</span></span>| <span data-ttu-id="fc325-135">Значение, используемое при настройке свойства *protocol* для записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="fc325-135">Value to use when configuring the *protocol* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="fc325-136">recordType</span><span class="sxs-lookup"><span data-stu-id="fc325-136">recordType</span></span>|<span data-ttu-id="fc325-137">String</span><span class="sxs-lookup"><span data-stu-id="fc325-137">String</span></span>|  <span data-ttu-id="fc325-p105">Тип записи DNS. Это свойство всегда имеет значение *Srv*. Ключ.</span><span class="sxs-lookup"><span data-stu-id="fc325-p105">Type of DNS record. The value is always *Srv*. Key</span></span> |
|<span data-ttu-id="fc325-141">service</span><span class="sxs-lookup"><span data-stu-id="fc325-141">service</span></span>|<span data-ttu-id="fc325-142">String</span><span class="sxs-lookup"><span data-stu-id="fc325-142">String</span></span>| <span data-ttu-id="fc325-143">Значение, используемое при настройке свойства *service* для записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="fc325-143">Value to use when configuring the *service* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="fc325-144">supportedService</span><span class="sxs-lookup"><span data-stu-id="fc325-144">supportedService</span></span>|<span data-ttu-id="fc325-145">String</span><span class="sxs-lookup"><span data-stu-id="fc325-145">String</span></span>| <span data-ttu-id="fc325-146">Служба или компонент Microsoft Online Services, зависящие от этой записи типа SRV.</span><span class="sxs-lookup"><span data-stu-id="fc325-146">Microsoft Online Service or feature that has a dependency on this SRV record.</span></span></br></br><span data-ttu-id="fc325-147">Возможные значения: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*.</span><span class="sxs-lookup"><span data-stu-id="fc325-147">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="fc325-148">ttl</span><span class="sxs-lookup"><span data-stu-id="fc325-148">ttl</span></span>|<span data-ttu-id="fc325-149">Int32</span><span class="sxs-lookup"><span data-stu-id="fc325-149">Int32</span></span>| <span data-ttu-id="fc325-p106">Значение, используемое при настройке свойства *ttl* (срока жизни) для записи SRV на узле DNS. Не допускает значения null.</span><span class="sxs-lookup"><span data-stu-id="fc325-p106">Value to use when configuring the *time-to-live (ttl)* property of the SRV record at the DNS host. Not nullable</span></span> |
|<span data-ttu-id="fc325-152">weight</span><span class="sxs-lookup"><span data-stu-id="fc325-152">weight</span></span>|<span data-ttu-id="fc325-153">Int32</span><span class="sxs-lookup"><span data-stu-id="fc325-153">Int32</span></span>| <span data-ttu-id="fc325-154">Значение, используемое при настройке свойства *weight* записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="fc325-154">Value to use when configuring the *weight* property of the SRV record at the DNS host.</span></span> |

## <a name="relationships"></a><span data-ttu-id="fc325-155">Связи</span><span class="sxs-lookup"><span data-stu-id="fc325-155">Relationships</span></span>
<span data-ttu-id="fc325-156">Нет</span><span class="sxs-lookup"><span data-stu-id="fc325-156">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="fc325-157">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fc325-157">JSON representation</span></span>
<span data-ttu-id="fc325-158">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fc325-158">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsSrvRecord"
}-->

```json
{
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "nameTarget": "String",
  "port": 1024,
  "priority": 1024,
  "protocol": "String",
  "recordType": "String",
  "service": "String",
  "supportedService": "String",
  "ttl": 1024,
  "weight": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsSrvRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
