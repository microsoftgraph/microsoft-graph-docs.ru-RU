---
title: Тип ресурса domainDnsSrvRecord
description: Представляет запись SRV, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от объекта DomainDnsRecord.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: db8b64397bd8d2904567555759a40186f740a1ed
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962816"
---
# <a name="domaindnssrvrecord-resource-type"></a><span data-ttu-id="032f4-104">Тип ресурса domainDnsSrvRecord</span><span class="sxs-lookup"><span data-stu-id="032f4-104">domainDnsSrvRecord resource type</span></span>

> <span data-ttu-id="032f4-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="032f4-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="032f4-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="032f4-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="032f4-p103">Представляет запись SRV, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от объекта [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="032f4-p103">Represents a SRV record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="032f4-109">Методы</span><span class="sxs-lookup"><span data-stu-id="032f4-109">Methods</span></span>
<span data-ttu-id="032f4-p104">Прямые запросы к этому ресурсу не поддерживаются. Сведения о том, как запрашивать записи службы доменов, см. в статье [о доменах](domain.md).</span><span class="sxs-lookup"><span data-stu-id="032f4-p104">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="032f4-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="032f4-112">Properties</span></span>
| <span data-ttu-id="032f4-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="032f4-113">Property</span></span>     | <span data-ttu-id="032f4-114">Тип</span><span class="sxs-lookup"><span data-stu-id="032f4-114">Type</span></span>   |<span data-ttu-id="032f4-115">Описание</span><span class="sxs-lookup"><span data-stu-id="032f4-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="032f4-116">id</span><span class="sxs-lookup"><span data-stu-id="032f4-116">id</span></span>|<span data-ttu-id="032f4-117">Строка</span><span class="sxs-lookup"><span data-stu-id="032f4-117">String</span></span>| <span data-ttu-id="032f4-p105">Уникальный идентификатор, назначенный этому объекту. Не допускает значения null, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="032f4-p105">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span>|
|<span data-ttu-id="032f4-120">isOptional</span><span class="sxs-lookup"><span data-stu-id="032f4-120">isOptional</span></span>|<span data-ttu-id="032f4-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="032f4-121">Boolean</span></span>| <span data-ttu-id="032f4-122">Если указано значение false, для правильной работы Microsoft Online Services с доменом пользователь должен настроить запись SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="032f4-122">If false, the SRV record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="032f4-123">label</span><span class="sxs-lookup"><span data-stu-id="032f4-123">label</span></span>|<span data-ttu-id="032f4-124">String</span><span class="sxs-lookup"><span data-stu-id="032f4-124">String</span></span>| <span data-ttu-id="032f4-125">Значение, используемое при настройке свойства *name* записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="032f4-125">Value used when configuring the *name* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="032f4-126">nameTarget</span><span class="sxs-lookup"><span data-stu-id="032f4-126">nameTarget</span></span>|<span data-ttu-id="032f4-127">String</span><span class="sxs-lookup"><span data-stu-id="032f4-127">String</span></span>| <span data-ttu-id="032f4-128">Значение, используемое при настройке свойства *Target* записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="032f4-128">Value to use when configuring the *Target* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="032f4-129">port</span><span class="sxs-lookup"><span data-stu-id="032f4-129">port</span></span>|<span data-ttu-id="032f4-130">Int32</span><span class="sxs-lookup"><span data-stu-id="032f4-130">Int32</span></span>| <span data-ttu-id="032f4-131">Значение, используемое при настройке свойства *port* записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="032f4-131">Value to use when configuring the *port* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="032f4-132">priority</span><span class="sxs-lookup"><span data-stu-id="032f4-132">priority</span></span>|<span data-ttu-id="032f4-133">Int32</span><span class="sxs-lookup"><span data-stu-id="032f4-133">Int32</span></span>| <span data-ttu-id="032f4-134">Значение, используемое при настройке свойства *priority* записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="032f4-134">Value to use when configuring the *priority* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="032f4-135">protocol</span><span class="sxs-lookup"><span data-stu-id="032f4-135">protocol</span></span>|<span data-ttu-id="032f4-136">String</span><span class="sxs-lookup"><span data-stu-id="032f4-136">String</span></span>| <span data-ttu-id="032f4-137">Значение, используемое при настройке свойства *protocol* для записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="032f4-137">Value to use when configuring the *protocol* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="032f4-138">recordType</span><span class="sxs-lookup"><span data-stu-id="032f4-138">recordType</span></span>|<span data-ttu-id="032f4-139">String</span><span class="sxs-lookup"><span data-stu-id="032f4-139">String</span></span>|  <span data-ttu-id="032f4-p106">Тип записи DNS. Это свойство всегда имеет значение *Srv*. Ключ.</span><span class="sxs-lookup"><span data-stu-id="032f4-p106">Type of DNS record. The value is always *Srv*. Key</span></span> |
|<span data-ttu-id="032f4-143">service</span><span class="sxs-lookup"><span data-stu-id="032f4-143">service</span></span>|<span data-ttu-id="032f4-144">String</span><span class="sxs-lookup"><span data-stu-id="032f4-144">String</span></span>| <span data-ttu-id="032f4-145">Значение, используемое при настройке свойства *service* для записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="032f4-145">Value to use when configuring the *service* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="032f4-146">supportedService</span><span class="sxs-lookup"><span data-stu-id="032f4-146">supportedService</span></span>|<span data-ttu-id="032f4-147">String</span><span class="sxs-lookup"><span data-stu-id="032f4-147">String</span></span>| <span data-ttu-id="032f4-148">Служба или компонент Microsoft Online Services, зависящие от этой записи типа SRV.</span><span class="sxs-lookup"><span data-stu-id="032f4-148">Microsoft Online Service or feature that has a dependency on this SRV record.</span></span></br></br><span data-ttu-id="032f4-149">Возможные значения: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*.</span><span class="sxs-lookup"><span data-stu-id="032f4-149">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="032f4-150">ttl</span><span class="sxs-lookup"><span data-stu-id="032f4-150">ttl</span></span>|<span data-ttu-id="032f4-151">Int32</span><span class="sxs-lookup"><span data-stu-id="032f4-151">Int32</span></span>| <span data-ttu-id="032f4-p107">Значение, используемое при настройке свойства *ttl* (срока жизни) для записи SRV на узле DNS. Не допускает значения null.</span><span class="sxs-lookup"><span data-stu-id="032f4-p107">Value to use when configuring the *time-to-live (ttl)* property of the SRV record at the DNS host. Not nullable</span></span> |
|<span data-ttu-id="032f4-154">weight</span><span class="sxs-lookup"><span data-stu-id="032f4-154">weight</span></span>|<span data-ttu-id="032f4-155">Int32</span><span class="sxs-lookup"><span data-stu-id="032f4-155">Int32</span></span>| <span data-ttu-id="032f4-156">Значение, используемое при настройке свойства *weight* записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="032f4-156">Value to use when configuring the *weight* property of the SRV record at the DNS host.</span></span> |

## <a name="relationships"></a><span data-ttu-id="032f4-157">Связи</span><span class="sxs-lookup"><span data-stu-id="032f4-157">Relationships</span></span>
<span data-ttu-id="032f4-158">Нет</span><span class="sxs-lookup"><span data-stu-id="032f4-158">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="032f4-159">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="032f4-159">JSON representation</span></span>
<span data-ttu-id="032f4-160">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="032f4-160">Here is a JSON representation of the resource.</span></span>

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
