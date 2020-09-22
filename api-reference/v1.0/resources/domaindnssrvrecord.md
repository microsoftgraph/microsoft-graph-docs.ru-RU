---
title: Тип ресурса Домаинднссрврекорд
description: Представляет запись SRV, добавленную в файл зоны DNS определенного домена в клиенте.
author: adimitui
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1c0ac0fce1291c5f6a5134bf7439cbe01c841fe9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018657"
---
# <a name="domaindnssrvrecord-resource-type"></a><span data-ttu-id="e5082-103">Тип ресурса Домаинднссрврекорд</span><span class="sxs-lookup"><span data-stu-id="e5082-103">domainDnsSrvRecord resource type</span></span>

<span data-ttu-id="e5082-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5082-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e5082-105">Представляет запись SRV, добавленную в файл зоны DNS определенного домена в клиенте.</span><span class="sxs-lookup"><span data-stu-id="e5082-105">Represents a SRV record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="e5082-106">Наследуется от объекта [DomainDnsRecord](domaindnsrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="e5082-106">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="e5082-107">Методы</span><span class="sxs-lookup"><span data-stu-id="e5082-107">Methods</span></span>
<span data-ttu-id="e5082-108">Прямые запросы к этому ресурсу не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="e5082-108">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="e5082-109">Сведения о том, как запросить записи службы домена, можно найти в разделе [domain](domain.md) .</span><span class="sxs-lookup"><span data-stu-id="e5082-109">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="e5082-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="e5082-110">Properties</span></span>
| <span data-ttu-id="e5082-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="e5082-111">Property</span></span>     | <span data-ttu-id="e5082-112">Тип</span><span class="sxs-lookup"><span data-stu-id="e5082-112">Type</span></span>   |<span data-ttu-id="e5082-113">Описание</span><span class="sxs-lookup"><span data-stu-id="e5082-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e5082-114">id</span><span class="sxs-lookup"><span data-stu-id="e5082-114">id</span></span>|<span data-ttu-id="e5082-115">String</span><span class="sxs-lookup"><span data-stu-id="e5082-115">String</span></span>| <span data-ttu-id="e5082-116">Уникальный идентификатор, назначенный этой сущности.</span><span class="sxs-lookup"><span data-stu-id="e5082-116">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="e5082-117">Не допускает значения NULL и только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e5082-117">Not nullable, Read-only.</span></span>|
|<span data-ttu-id="e5082-118">Переключатель</span><span class="sxs-lookup"><span data-stu-id="e5082-118">isOptional</span></span>|<span data-ttu-id="e5082-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5082-119">Boolean</span></span>| <span data-ttu-id="e5082-120">Если задано значение false, запись SRV должна быть настроена клиентом на узле DNS для правильной работы Microsoft Online Services с доменом.</span><span class="sxs-lookup"><span data-stu-id="e5082-120">If false, the SRV record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="e5082-121">label</span><span class="sxs-lookup"><span data-stu-id="e5082-121">label</span></span>|<span data-ttu-id="e5082-122">String</span><span class="sxs-lookup"><span data-stu-id="e5082-122">String</span></span>| <span data-ttu-id="e5082-123">Значение, используемое при настройке свойства *Name* записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="e5082-123">Value used when configuring the *name* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="e5082-124">наметаржет</span><span class="sxs-lookup"><span data-stu-id="e5082-124">nameTarget</span></span>|<span data-ttu-id="e5082-125">String</span><span class="sxs-lookup"><span data-stu-id="e5082-125">String</span></span>| <span data-ttu-id="e5082-126">Значение, используемое при настройке свойства *Target* записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="e5082-126">Value to use when configuring the *Target* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="e5082-127">порта</span><span class="sxs-lookup"><span data-stu-id="e5082-127">port</span></span>|<span data-ttu-id="e5082-128">Int32</span><span class="sxs-lookup"><span data-stu-id="e5082-128">Int32</span></span>| <span data-ttu-id="e5082-129">Значение, используемое при настройке свойства *Port* записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="e5082-129">Value to use when configuring the *port* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="e5082-130">priority</span><span class="sxs-lookup"><span data-stu-id="e5082-130">priority</span></span>|<span data-ttu-id="e5082-131">Int32</span><span class="sxs-lookup"><span data-stu-id="e5082-131">Int32</span></span>| <span data-ttu-id="e5082-132">Значение, используемое при настройке свойства *Priority* записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="e5082-132">Value to use when configuring the *priority* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="e5082-133">Protocol</span><span class="sxs-lookup"><span data-stu-id="e5082-133">protocol</span></span>|<span data-ttu-id="e5082-134">String</span><span class="sxs-lookup"><span data-stu-id="e5082-134">String</span></span>| <span data-ttu-id="e5082-135">Значение, используемое при настройке свойства *Protocol* записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="e5082-135">Value to use when configuring the *protocol* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="e5082-136">recordType</span><span class="sxs-lookup"><span data-stu-id="e5082-136">recordType</span></span>|<span data-ttu-id="e5082-137">String</span><span class="sxs-lookup"><span data-stu-id="e5082-137">String</span></span>|  <span data-ttu-id="e5082-138">Тип записи DNS.</span><span class="sxs-lookup"><span data-stu-id="e5082-138">Type of DNS record.</span></span> <span data-ttu-id="e5082-139">Значение — всегда *SRV*.</span><span class="sxs-lookup"><span data-stu-id="e5082-139">The value is always *Srv*.</span></span> <span data-ttu-id="e5082-140">Key</span><span class="sxs-lookup"><span data-stu-id="e5082-140">Key</span></span> |
|<span data-ttu-id="e5082-141">service</span><span class="sxs-lookup"><span data-stu-id="e5082-141">service</span></span>|<span data-ttu-id="e5082-142">String</span><span class="sxs-lookup"><span data-stu-id="e5082-142">String</span></span>| <span data-ttu-id="e5082-143">Значение, используемое при настройке свойства *Service* для записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="e5082-143">Value to use when configuring the *service* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="e5082-144">суппортедсервице</span><span class="sxs-lookup"><span data-stu-id="e5082-144">supportedService</span></span>|<span data-ttu-id="e5082-145">String</span><span class="sxs-lookup"><span data-stu-id="e5082-145">String</span></span>| <span data-ttu-id="e5082-146">Служба или компонент Microsoft Online, который имеет зависимость от этой записи SRV.</span><span class="sxs-lookup"><span data-stu-id="e5082-146">Microsoft Online Service or feature that has a dependency on this SRV record.</span></span></br></br><span data-ttu-id="e5082-147">Может принимать одно из следующих значений: **null**, *Email*, *SharePoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="e5082-147">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="e5082-148">используем</span><span class="sxs-lookup"><span data-stu-id="e5082-148">ttl</span></span>|<span data-ttu-id="e5082-149">Int32</span><span class="sxs-lookup"><span data-stu-id="e5082-149">Int32</span></span>| <span data-ttu-id="e5082-150">Значение, используемое при настройке свойства срока *жизни (TTL)* записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="e5082-150">Value to use when configuring the *time-to-live (ttl)* property of the SRV record at the DNS host.</span></span> <span data-ttu-id="e5082-151">Не допускает значение null</span><span class="sxs-lookup"><span data-stu-id="e5082-151">Not nullable</span></span> |
|<span data-ttu-id="e5082-152">weight</span><span class="sxs-lookup"><span data-stu-id="e5082-152">weight</span></span>|<span data-ttu-id="e5082-153">Int32</span><span class="sxs-lookup"><span data-stu-id="e5082-153">Int32</span></span>| <span data-ttu-id="e5082-154">Значение, используемое при настройке свойства *Weight* записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="e5082-154">Value to use when configuring the *weight* property of the SRV record at the DNS host.</span></span> |

## <a name="relationships"></a><span data-ttu-id="e5082-155">Связи</span><span class="sxs-lookup"><span data-stu-id="e5082-155">Relationships</span></span>
<span data-ttu-id="e5082-156">Нет</span><span class="sxs-lookup"><span data-stu-id="e5082-156">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e5082-157">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e5082-157">JSON representation</span></span>
<span data-ttu-id="e5082-158">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e5082-158">Here is a JSON representation of the resource.</span></span>

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

