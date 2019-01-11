---
title: Тип ресурса domainDnsSrvRecord
description: Представляет запись SRV, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от объекта DomainDnsRecord.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: c06682753b752980530bf8cfd8f6a32b9bbd569a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810439"
---
# <a name="domaindnssrvrecord-resource-type"></a><span data-ttu-id="dea36-104">Тип ресурса domainDnsSrvRecord</span><span class="sxs-lookup"><span data-stu-id="dea36-104">domainDnsSrvRecord resource type</span></span>

> <span data-ttu-id="dea36-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="dea36-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dea36-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dea36-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dea36-p103">Представляет запись SRV, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от объекта [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="dea36-p103">Represents a SRV record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="dea36-109">Методы</span><span class="sxs-lookup"><span data-stu-id="dea36-109">Methods</span></span>
<span data-ttu-id="dea36-p104">Прямые запросы к этому ресурсу не поддерживаются. Сведения о том, как запрашивать записи службы доменов, см. в статье [о доменах](domain.md).</span><span class="sxs-lookup"><span data-stu-id="dea36-p104">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="dea36-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="dea36-112">Properties</span></span>
| <span data-ttu-id="dea36-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="dea36-113">Property</span></span>     | <span data-ttu-id="dea36-114">Тип</span><span class="sxs-lookup"><span data-stu-id="dea36-114">Type</span></span>   |<span data-ttu-id="dea36-115">Описание</span><span class="sxs-lookup"><span data-stu-id="dea36-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dea36-116">id</span><span class="sxs-lookup"><span data-stu-id="dea36-116">id</span></span>|<span data-ttu-id="dea36-117">Строка</span><span class="sxs-lookup"><span data-stu-id="dea36-117">String</span></span>| <span data-ttu-id="dea36-p105">Уникальный идентификатор, назначенный этому объекту. Не допускает значения null, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dea36-p105">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span>|
|<span data-ttu-id="dea36-120">isOptional</span><span class="sxs-lookup"><span data-stu-id="dea36-120">isOptional</span></span>|<span data-ttu-id="dea36-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="dea36-121">Boolean</span></span>| <span data-ttu-id="dea36-122">Если указано значение false, для правильной работы Microsoft Online Services с доменом пользователь должен настроить запись SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="dea36-122">If false, the SRV record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="dea36-123">label</span><span class="sxs-lookup"><span data-stu-id="dea36-123">label</span></span>|<span data-ttu-id="dea36-124">String</span><span class="sxs-lookup"><span data-stu-id="dea36-124">String</span></span>| <span data-ttu-id="dea36-125">Значение, используемое при настройке свойства *name* записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="dea36-125">Value used when configuring the *name* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="dea36-126">nameTarget</span><span class="sxs-lookup"><span data-stu-id="dea36-126">nameTarget</span></span>|<span data-ttu-id="dea36-127">String</span><span class="sxs-lookup"><span data-stu-id="dea36-127">String</span></span>| <span data-ttu-id="dea36-128">Значение, используемое при настройке свойства *Target* записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="dea36-128">Value to use when configuring the *Target* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="dea36-129">port</span><span class="sxs-lookup"><span data-stu-id="dea36-129">port</span></span>|<span data-ttu-id="dea36-130">Int32</span><span class="sxs-lookup"><span data-stu-id="dea36-130">Int32</span></span>| <span data-ttu-id="dea36-131">Значение, используемое при настройке свойства *port* записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="dea36-131">Value to use when configuring the *port* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="dea36-132">priority</span><span class="sxs-lookup"><span data-stu-id="dea36-132">priority</span></span>|<span data-ttu-id="dea36-133">Int32</span><span class="sxs-lookup"><span data-stu-id="dea36-133">Int32</span></span>| <span data-ttu-id="dea36-134">Значение, используемое при настройке свойства *priority* записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="dea36-134">Value to use when configuring the *priority* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="dea36-135">protocol</span><span class="sxs-lookup"><span data-stu-id="dea36-135">protocol</span></span>|<span data-ttu-id="dea36-136">String</span><span class="sxs-lookup"><span data-stu-id="dea36-136">String</span></span>| <span data-ttu-id="dea36-137">Значение, используемое при настройке свойства *protocol* для записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="dea36-137">Value to use when configuring the *protocol* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="dea36-138">recordType</span><span class="sxs-lookup"><span data-stu-id="dea36-138">recordType</span></span>|<span data-ttu-id="dea36-139">String</span><span class="sxs-lookup"><span data-stu-id="dea36-139">String</span></span>|  <span data-ttu-id="dea36-p106">Тип записи DNS. Это свойство всегда имеет значение *Srv*. Ключ.</span><span class="sxs-lookup"><span data-stu-id="dea36-p106">Type of DNS record. The value is always *Srv*. Key</span></span> |
|<span data-ttu-id="dea36-143">service</span><span class="sxs-lookup"><span data-stu-id="dea36-143">service</span></span>|<span data-ttu-id="dea36-144">String</span><span class="sxs-lookup"><span data-stu-id="dea36-144">String</span></span>| <span data-ttu-id="dea36-145">Значение, используемое при настройке свойства *service* для записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="dea36-145">Value to use when configuring the *service* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="dea36-146">supportedService</span><span class="sxs-lookup"><span data-stu-id="dea36-146">supportedService</span></span>|<span data-ttu-id="dea36-147">String</span><span class="sxs-lookup"><span data-stu-id="dea36-147">String</span></span>| <span data-ttu-id="dea36-148">Служба или компонент Microsoft Online Services, зависящие от этой записи типа SRV.</span><span class="sxs-lookup"><span data-stu-id="dea36-148">Microsoft Online Service or feature that has a dependency on this SRV record.</span></span></br></br><span data-ttu-id="dea36-149">Возможные значения: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*.</span><span class="sxs-lookup"><span data-stu-id="dea36-149">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="dea36-150">ttl</span><span class="sxs-lookup"><span data-stu-id="dea36-150">ttl</span></span>|<span data-ttu-id="dea36-151">Int32</span><span class="sxs-lookup"><span data-stu-id="dea36-151">Int32</span></span>| <span data-ttu-id="dea36-p107">Значение, используемое при настройке свойства *ttl* (срока жизни) для записи SRV на узле DNS. Не допускает значения null.</span><span class="sxs-lookup"><span data-stu-id="dea36-p107">Value to use when configuring the *time-to-live (ttl)* property of the SRV record at the DNS host. Not nullable</span></span> |
|<span data-ttu-id="dea36-154">weight</span><span class="sxs-lookup"><span data-stu-id="dea36-154">weight</span></span>|<span data-ttu-id="dea36-155">Int32</span><span class="sxs-lookup"><span data-stu-id="dea36-155">Int32</span></span>| <span data-ttu-id="dea36-156">Значение, используемое при настройке свойства *weight* записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="dea36-156">Value to use when configuring the *weight* property of the SRV record at the DNS host.</span></span> |

## <a name="relationships"></a><span data-ttu-id="dea36-157">Связи</span><span class="sxs-lookup"><span data-stu-id="dea36-157">Relationships</span></span>
<span data-ttu-id="dea36-158">Нет</span><span class="sxs-lookup"><span data-stu-id="dea36-158">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="dea36-159">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dea36-159">JSON representation</span></span>
<span data-ttu-id="dea36-160">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dea36-160">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsSrvRecord"
}-->

```json
{
  "canonicalName": "String",
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
