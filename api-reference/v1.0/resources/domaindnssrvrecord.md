---
title: Тип ресурса domainDnsSrvRecord
description: Представляет запись SRV, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от объекта DomainDnsRecord.
author: lleonard-msft
ms.openlocfilehash: d8fbdb6a99e2a4c88b38d350ace3976842eb7f92
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27318825"
---
# <a name="domaindnssrvrecord-resource-type"></a><span data-ttu-id="b0342-104">Тип ресурса domainDnsSrvRecord</span><span class="sxs-lookup"><span data-stu-id="b0342-104">domainDnsSrvRecord resource type</span></span>

<span data-ttu-id="b0342-p102">Представляет запись SRV, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от объекта [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="b0342-p102">Represents a SRV record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="b0342-107">Методы</span><span class="sxs-lookup"><span data-stu-id="b0342-107">Methods</span></span>
<span data-ttu-id="b0342-p103">Прямые запросы к этому ресурсу не поддерживаются. Сведения о том, как запрашивать записи службы доменов, см. в статье [о доменах](domain.md).</span><span class="sxs-lookup"><span data-stu-id="b0342-p103">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="b0342-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="b0342-110">Properties</span></span>
| <span data-ttu-id="b0342-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="b0342-111">Property</span></span>     | <span data-ttu-id="b0342-112">Тип</span><span class="sxs-lookup"><span data-stu-id="b0342-112">Type</span></span>   |<span data-ttu-id="b0342-113">Описание</span><span class="sxs-lookup"><span data-stu-id="b0342-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b0342-114">id</span><span class="sxs-lookup"><span data-stu-id="b0342-114">id</span></span>|<span data-ttu-id="b0342-115">Строка</span><span class="sxs-lookup"><span data-stu-id="b0342-115">String</span></span>| <span data-ttu-id="b0342-p104">Уникальный идентификатор, назначенный этому объекту. Не допускает значения null, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b0342-p104">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span>|
|<span data-ttu-id="b0342-118">isOptional</span><span class="sxs-lookup"><span data-stu-id="b0342-118">isOptional</span></span>|<span data-ttu-id="b0342-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="b0342-119">Boolean</span></span>| <span data-ttu-id="b0342-120">Если указано значение false, для правильной работы Microsoft Online Services с доменом пользователь должен настроить запись SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="b0342-120">If false, the SRV record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="b0342-121">label</span><span class="sxs-lookup"><span data-stu-id="b0342-121">label</span></span>|<span data-ttu-id="b0342-122">String</span><span class="sxs-lookup"><span data-stu-id="b0342-122">String</span></span>| <span data-ttu-id="b0342-123">Значение, используемое при настройке свойства *name* записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="b0342-123">Value used when configuring the *name* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="b0342-124">nameTarget</span><span class="sxs-lookup"><span data-stu-id="b0342-124">nameTarget</span></span>|<span data-ttu-id="b0342-125">String</span><span class="sxs-lookup"><span data-stu-id="b0342-125">String</span></span>| <span data-ttu-id="b0342-126">Значение, используемое при настройке свойства *Target* записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="b0342-126">Value to use when configuring the *Target* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="b0342-127">port</span><span class="sxs-lookup"><span data-stu-id="b0342-127">port</span></span>|<span data-ttu-id="b0342-128">Int32</span><span class="sxs-lookup"><span data-stu-id="b0342-128">Int32</span></span>| <span data-ttu-id="b0342-129">Значение, используемое при настройке свойства *port* записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="b0342-129">Value to use when configuring the *port* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="b0342-130">priority</span><span class="sxs-lookup"><span data-stu-id="b0342-130">priority</span></span>|<span data-ttu-id="b0342-131">Int32</span><span class="sxs-lookup"><span data-stu-id="b0342-131">Int32</span></span>| <span data-ttu-id="b0342-132">Значение, используемое при настройке свойства *priority* записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="b0342-132">Value to use when configuring the *priority* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="b0342-133">protocol</span><span class="sxs-lookup"><span data-stu-id="b0342-133">protocol</span></span>|<span data-ttu-id="b0342-134">String</span><span class="sxs-lookup"><span data-stu-id="b0342-134">String</span></span>| <span data-ttu-id="b0342-135">Значение, используемое при настройке свойства *protocol* для записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="b0342-135">Value to use when configuring the *protocol* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="b0342-136">recordType</span><span class="sxs-lookup"><span data-stu-id="b0342-136">recordType</span></span>|<span data-ttu-id="b0342-137">String</span><span class="sxs-lookup"><span data-stu-id="b0342-137">String</span></span>|  <span data-ttu-id="b0342-p105">Тип записи DNS. Это свойство всегда имеет значение *Srv*. Ключ.</span><span class="sxs-lookup"><span data-stu-id="b0342-p105">Type of DNS record. The value is always *Srv*. Key</span></span> |
|<span data-ttu-id="b0342-141">service</span><span class="sxs-lookup"><span data-stu-id="b0342-141">service</span></span>|<span data-ttu-id="b0342-142">String</span><span class="sxs-lookup"><span data-stu-id="b0342-142">String</span></span>| <span data-ttu-id="b0342-143">Значение, используемое при настройке свойства *service* для записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="b0342-143">Value to use when configuring the *service* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="b0342-144">supportedService</span><span class="sxs-lookup"><span data-stu-id="b0342-144">supportedService</span></span>|<span data-ttu-id="b0342-145">String</span><span class="sxs-lookup"><span data-stu-id="b0342-145">String</span></span>| <span data-ttu-id="b0342-146">Служба или компонент Microsoft Online Services, зависящие от этой записи типа SRV.</span><span class="sxs-lookup"><span data-stu-id="b0342-146">Microsoft Online Service or feature that has a dependency on this SRV record.</span></span></br></br><span data-ttu-id="b0342-147">Возможные значения: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*.</span><span class="sxs-lookup"><span data-stu-id="b0342-147">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="b0342-148">ttl</span><span class="sxs-lookup"><span data-stu-id="b0342-148">ttl</span></span>|<span data-ttu-id="b0342-149">Int32</span><span class="sxs-lookup"><span data-stu-id="b0342-149">Int32</span></span>| <span data-ttu-id="b0342-p106">Значение, используемое при настройке свойства *ttl* (срока жизни) для записи SRV на узле DNS. Не допускает значения null.</span><span class="sxs-lookup"><span data-stu-id="b0342-p106">Value to use when configuring the *time-to-live (ttl)* property of the SRV record at the DNS host. Not nullable</span></span> |
|<span data-ttu-id="b0342-152">weight</span><span class="sxs-lookup"><span data-stu-id="b0342-152">weight</span></span>|<span data-ttu-id="b0342-153">Int32</span><span class="sxs-lookup"><span data-stu-id="b0342-153">Int32</span></span>| <span data-ttu-id="b0342-154">Значение, используемое при настройке свойства *weight* записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="b0342-154">Value to use when configuring the *weight* property of the SRV record at the DNS host.</span></span> |

## <a name="relationships"></a><span data-ttu-id="b0342-155">Связи</span><span class="sxs-lookup"><span data-stu-id="b0342-155">Relationships</span></span>
<span data-ttu-id="b0342-156">Нет</span><span class="sxs-lookup"><span data-stu-id="b0342-156">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="b0342-157">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b0342-157">JSON representation</span></span>
<span data-ttu-id="b0342-158">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b0342-158">Here is a JSON representation of the resource.</span></span>

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