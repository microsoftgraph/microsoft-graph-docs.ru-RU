---
title: тип ресурса domainDnsSrvRecord
description: Представляет запись SRV, добавленную в файл зоны DNS определенного домена в клиенте.
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 7755779218b7120e24cc25f6e0a5a97d4c42db5d
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761200"
---
# <a name="domaindnssrvrecord-resource-type"></a><span data-ttu-id="dd0f4-103">тип ресурса domainDnsSrvRecord</span><span class="sxs-lookup"><span data-stu-id="dd0f4-103">domainDnsSrvRecord resource type</span></span>

<span data-ttu-id="dd0f4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd0f4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dd0f4-105">Представляет запись SRV, добавленную в файл зоны DNS определенного домена в клиенте.</span><span class="sxs-lookup"><span data-stu-id="dd0f4-105">Represents a SRV record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="dd0f4-106">Наследуется от [объекта DomainDnsRecord.](domaindnsrecord.md)</span><span class="sxs-lookup"><span data-stu-id="dd0f4-106">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="dd0f4-107">Методы</span><span class="sxs-lookup"><span data-stu-id="dd0f4-107">Methods</span></span>
<span data-ttu-id="dd0f4-108">Прямые запросы на этот ресурс не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="dd0f4-108">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="dd0f4-109">Сведения о [том,](domain.md) как запрашивать записи службы домена, см. в разделе домен.</span><span class="sxs-lookup"><span data-stu-id="dd0f4-109">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="dd0f4-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="dd0f4-110">Properties</span></span>
| <span data-ttu-id="dd0f4-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="dd0f4-111">Property</span></span>     | <span data-ttu-id="dd0f4-112">Тип</span><span class="sxs-lookup"><span data-stu-id="dd0f4-112">Type</span></span>   |<span data-ttu-id="dd0f4-113">Описание</span><span class="sxs-lookup"><span data-stu-id="dd0f4-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dd0f4-114">id</span><span class="sxs-lookup"><span data-stu-id="dd0f4-114">id</span></span>|<span data-ttu-id="dd0f4-115">String</span><span class="sxs-lookup"><span data-stu-id="dd0f4-115">String</span></span>| <span data-ttu-id="dd0f4-116">Уникальный идентификатор, присвоенный этому объекту.</span><span class="sxs-lookup"><span data-stu-id="dd0f4-116">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="dd0f4-117">Не является недействительным, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dd0f4-117">Not nullable, Read-only.</span></span>|
|<span data-ttu-id="dd0f4-118">isOptional</span><span class="sxs-lookup"><span data-stu-id="dd0f4-118">isOptional</span></span>|<span data-ttu-id="dd0f4-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd0f4-119">Boolean</span></span>| <span data-ttu-id="dd0f4-120">Если это неверно, запись SRV должна быть настроена клиентом на хост DNS, чтобы Microsoft Online Services правильно работать с доменом.</span><span class="sxs-lookup"><span data-stu-id="dd0f4-120">If false, the SRV record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="dd0f4-121">label</span><span class="sxs-lookup"><span data-stu-id="dd0f4-121">label</span></span>|<span data-ttu-id="dd0f4-122">String</span><span class="sxs-lookup"><span data-stu-id="dd0f4-122">String</span></span>| <span data-ttu-id="dd0f4-123">Значение, используемого при настройке *свойства* имени записи SRV в хосте DNS.</span><span class="sxs-lookup"><span data-stu-id="dd0f4-123">Value used when configuring the *name* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="dd0f4-124">nameTarget</span><span class="sxs-lookup"><span data-stu-id="dd0f4-124">nameTarget</span></span>|<span data-ttu-id="dd0f4-125">String</span><span class="sxs-lookup"><span data-stu-id="dd0f4-125">String</span></span>| <span data-ttu-id="dd0f4-126">Значение, используемого при настройке *целевого* свойства записи SRV в хосте DNS.</span><span class="sxs-lookup"><span data-stu-id="dd0f4-126">Value to use when configuring the *Target* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="dd0f4-127">порт</span><span class="sxs-lookup"><span data-stu-id="dd0f4-127">port</span></span>|<span data-ttu-id="dd0f4-128">Int32</span><span class="sxs-lookup"><span data-stu-id="dd0f4-128">Int32</span></span>| <span data-ttu-id="dd0f4-129">Значение, используемого при  настройке свойства порта записи SRV в хосте DNS.</span><span class="sxs-lookup"><span data-stu-id="dd0f4-129">Value to use when configuring the *port* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="dd0f4-130">priority</span><span class="sxs-lookup"><span data-stu-id="dd0f4-130">priority</span></span>|<span data-ttu-id="dd0f4-131">Int32</span><span class="sxs-lookup"><span data-stu-id="dd0f4-131">Int32</span></span>| <span data-ttu-id="dd0f4-132">Значение, используемое при настройке *приоритетного* свойства записи SRV в хосте DNS.</span><span class="sxs-lookup"><span data-stu-id="dd0f4-132">Value to use when configuring the *priority* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="dd0f4-133">протокол</span><span class="sxs-lookup"><span data-stu-id="dd0f4-133">protocol</span></span>|<span data-ttu-id="dd0f4-134">String</span><span class="sxs-lookup"><span data-stu-id="dd0f4-134">String</span></span>| <span data-ttu-id="dd0f4-135">Значение, используемого при настройке свойства *протокола* записи SRV в DNS-хозяйне.</span><span class="sxs-lookup"><span data-stu-id="dd0f4-135">Value to use when configuring the *protocol* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="dd0f4-136">recordType</span><span class="sxs-lookup"><span data-stu-id="dd0f4-136">recordType</span></span>|<span data-ttu-id="dd0f4-137">String</span><span class="sxs-lookup"><span data-stu-id="dd0f4-137">String</span></span>|  <span data-ttu-id="dd0f4-138">Тип записи DNS.</span><span class="sxs-lookup"><span data-stu-id="dd0f4-138">Type of DNS record.</span></span> <span data-ttu-id="dd0f4-139">Значение всегда *Srv*.</span><span class="sxs-lookup"><span data-stu-id="dd0f4-139">The value is always *Srv*.</span></span> <span data-ttu-id="dd0f4-140">Key</span><span class="sxs-lookup"><span data-stu-id="dd0f4-140">Key</span></span> |
|<span data-ttu-id="dd0f4-141">service</span><span class="sxs-lookup"><span data-stu-id="dd0f4-141">service</span></span>|<span data-ttu-id="dd0f4-142">String</span><span class="sxs-lookup"><span data-stu-id="dd0f4-142">String</span></span>| <span data-ttu-id="dd0f4-143">Значение, используемого при  настройке свойства службы записи SRV в DNS-хозяйне.</span><span class="sxs-lookup"><span data-stu-id="dd0f4-143">Value to use when configuring the *service* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="dd0f4-144">supportedService</span><span class="sxs-lookup"><span data-stu-id="dd0f4-144">supportedService</span></span>|<span data-ttu-id="dd0f4-145">String</span><span class="sxs-lookup"><span data-stu-id="dd0f4-145">String</span></span>| <span data-ttu-id="dd0f4-146">Microsoft Online Service или функция, зависимая от этой записи SRV.</span><span class="sxs-lookup"><span data-stu-id="dd0f4-146">Microsoft Online Service or feature that has a dependency on this SRV record.</span></span></br></br><span data-ttu-id="dd0f4-147">Может быть одним из следующих значений: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="dd0f4-147">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="dd0f4-148">ttl</span><span class="sxs-lookup"><span data-stu-id="dd0f4-148">ttl</span></span>|<span data-ttu-id="dd0f4-149">Int32</span><span class="sxs-lookup"><span data-stu-id="dd0f4-149">Int32</span></span>| <span data-ttu-id="dd0f4-150">Значение, используемого при настройке свойства "время на *жизнь"* записи SRV в DNS-хозяйне.</span><span class="sxs-lookup"><span data-stu-id="dd0f4-150">Value to use when configuring the *time-to-live (ttl)* property of the SRV record at the DNS host.</span></span> <span data-ttu-id="dd0f4-151">Не является недействительным</span><span class="sxs-lookup"><span data-stu-id="dd0f4-151">Not nullable</span></span> |
|<span data-ttu-id="dd0f4-152">weight</span><span class="sxs-lookup"><span data-stu-id="dd0f4-152">weight</span></span>|<span data-ttu-id="dd0f4-153">Int32</span><span class="sxs-lookup"><span data-stu-id="dd0f4-153">Int32</span></span>| <span data-ttu-id="dd0f4-154">Значение, используемого при  настройке свойства веса записи SRV в хосте DNS.</span><span class="sxs-lookup"><span data-stu-id="dd0f4-154">Value to use when configuring the *weight* property of the SRV record at the DNS host.</span></span> |

## <a name="relationships"></a><span data-ttu-id="dd0f4-155">Связи</span><span class="sxs-lookup"><span data-stu-id="dd0f4-155">Relationships</span></span>
<span data-ttu-id="dd0f4-156">Нет</span><span class="sxs-lookup"><span data-stu-id="dd0f4-156">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="dd0f4-157">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dd0f4-157">JSON representation</span></span>
<span data-ttu-id="dd0f4-158">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dd0f4-158">Here is a JSON representation of the resource.</span></span>

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

