---
title: Тип ресурса Домаинднссрврекорд
description: Представляет запись SRV, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от объекта DomainDnsRecord.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9f3b4e9b1b65a473492b42322d81c2ef6f6e172c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42505947"
---
# <a name="domaindnssrvrecord-resource-type"></a><span data-ttu-id="902b3-104">Тип ресурса Домаинднссрврекорд</span><span class="sxs-lookup"><span data-stu-id="902b3-104">domainDnsSrvRecord resource type</span></span>

<span data-ttu-id="902b3-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="902b3-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="902b3-106">Представляет запись SRV, добавленную в файл зоны DNS определенного домена в клиенте.</span><span class="sxs-lookup"><span data-stu-id="902b3-106">Represents a SRV record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="902b3-107">Наследуется от объекта [DomainDnsRecord](domaindnsrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="902b3-107">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="902b3-108">Методы</span><span class="sxs-lookup"><span data-stu-id="902b3-108">Methods</span></span>
<span data-ttu-id="902b3-109">Прямые запросы к этому ресурсу не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="902b3-109">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="902b3-110">Сведения о том, как запросить записи службы домена, можно найти в разделе [domain](domain.md) .</span><span class="sxs-lookup"><span data-stu-id="902b3-110">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="902b3-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="902b3-111">Properties</span></span>
| <span data-ttu-id="902b3-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="902b3-112">Property</span></span>     | <span data-ttu-id="902b3-113">Тип</span><span class="sxs-lookup"><span data-stu-id="902b3-113">Type</span></span>   |<span data-ttu-id="902b3-114">Описание</span><span class="sxs-lookup"><span data-stu-id="902b3-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="902b3-115">id</span><span class="sxs-lookup"><span data-stu-id="902b3-115">id</span></span>|<span data-ttu-id="902b3-116">String</span><span class="sxs-lookup"><span data-stu-id="902b3-116">String</span></span>| <span data-ttu-id="902b3-117">Уникальный идентификатор, назначенный этой сущности.</span><span class="sxs-lookup"><span data-stu-id="902b3-117">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="902b3-118">Не допускает значения NULL и только для чтения.</span><span class="sxs-lookup"><span data-stu-id="902b3-118">Not nullable, Read-only.</span></span>|
|<span data-ttu-id="902b3-119">Переключатель</span><span class="sxs-lookup"><span data-stu-id="902b3-119">isOptional</span></span>|<span data-ttu-id="902b3-120">Логический</span><span class="sxs-lookup"><span data-stu-id="902b3-120">Boolean</span></span>| <span data-ttu-id="902b3-121">Если задано значение false, запись SRV должна быть настроена клиентом на узле DNS для правильной работы Microsoft Online Services с доменом.</span><span class="sxs-lookup"><span data-stu-id="902b3-121">If false, the SRV record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="902b3-122">label</span><span class="sxs-lookup"><span data-stu-id="902b3-122">label</span></span>|<span data-ttu-id="902b3-123">String</span><span class="sxs-lookup"><span data-stu-id="902b3-123">String</span></span>| <span data-ttu-id="902b3-124">Значение, используемое при настройке свойства *Name* записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="902b3-124">Value used when configuring the *name* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="902b3-125">наметаржет</span><span class="sxs-lookup"><span data-stu-id="902b3-125">nameTarget</span></span>|<span data-ttu-id="902b3-126">String</span><span class="sxs-lookup"><span data-stu-id="902b3-126">String</span></span>| <span data-ttu-id="902b3-127">Значение, используемое при настройке свойства *Target* записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="902b3-127">Value to use when configuring the *Target* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="902b3-128">порта</span><span class="sxs-lookup"><span data-stu-id="902b3-128">port</span></span>|<span data-ttu-id="902b3-129">Int32</span><span class="sxs-lookup"><span data-stu-id="902b3-129">Int32</span></span>| <span data-ttu-id="902b3-130">Значение, используемое при настройке свойства *Port* записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="902b3-130">Value to use when configuring the *port* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="902b3-131">priority</span><span class="sxs-lookup"><span data-stu-id="902b3-131">priority</span></span>|<span data-ttu-id="902b3-132">Int32</span><span class="sxs-lookup"><span data-stu-id="902b3-132">Int32</span></span>| <span data-ttu-id="902b3-133">Значение, используемое при настройке свойства *Priority* записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="902b3-133">Value to use when configuring the *priority* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="902b3-134">Protocol</span><span class="sxs-lookup"><span data-stu-id="902b3-134">protocol</span></span>|<span data-ttu-id="902b3-135">String</span><span class="sxs-lookup"><span data-stu-id="902b3-135">String</span></span>| <span data-ttu-id="902b3-136">Значение, используемое при настройке свойства *Protocol* записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="902b3-136">Value to use when configuring the *protocol* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="902b3-137">recordType</span><span class="sxs-lookup"><span data-stu-id="902b3-137">recordType</span></span>|<span data-ttu-id="902b3-138">String</span><span class="sxs-lookup"><span data-stu-id="902b3-138">String</span></span>|  <span data-ttu-id="902b3-139">Тип записи DNS.</span><span class="sxs-lookup"><span data-stu-id="902b3-139">Type of DNS record.</span></span> <span data-ttu-id="902b3-140">Значение — всегда *SRV*.</span><span class="sxs-lookup"><span data-stu-id="902b3-140">The value is always *Srv*.</span></span> <span data-ttu-id="902b3-141">Key</span><span class="sxs-lookup"><span data-stu-id="902b3-141">Key</span></span> |
|<span data-ttu-id="902b3-142">service</span><span class="sxs-lookup"><span data-stu-id="902b3-142">service</span></span>|<span data-ttu-id="902b3-143">String</span><span class="sxs-lookup"><span data-stu-id="902b3-143">String</span></span>| <span data-ttu-id="902b3-144">Значение, используемое при настройке свойства *Service* для записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="902b3-144">Value to use when configuring the *service* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="902b3-145">суппортедсервице</span><span class="sxs-lookup"><span data-stu-id="902b3-145">supportedService</span></span>|<span data-ttu-id="902b3-146">String</span><span class="sxs-lookup"><span data-stu-id="902b3-146">String</span></span>| <span data-ttu-id="902b3-147">Служба или компонент Microsoft Online, который имеет зависимость от этой записи SRV.</span><span class="sxs-lookup"><span data-stu-id="902b3-147">Microsoft Online Service or feature that has a dependency on this SRV record.</span></span></br></br><span data-ttu-id="902b3-148">Может принимать одно из следующих значений: **null**, *Email*, *SharePoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="902b3-148">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="902b3-149">используем</span><span class="sxs-lookup"><span data-stu-id="902b3-149">ttl</span></span>|<span data-ttu-id="902b3-150">Int32</span><span class="sxs-lookup"><span data-stu-id="902b3-150">Int32</span></span>| <span data-ttu-id="902b3-151">Значение, используемое при настройке свойства срока *жизни (TTL)* записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="902b3-151">Value to use when configuring the *time-to-live (ttl)* property of the SRV record at the DNS host.</span></span> <span data-ttu-id="902b3-152">Не допускает значение null</span><span class="sxs-lookup"><span data-stu-id="902b3-152">Not nullable</span></span> |
|<span data-ttu-id="902b3-153">weight</span><span class="sxs-lookup"><span data-stu-id="902b3-153">weight</span></span>|<span data-ttu-id="902b3-154">Int32</span><span class="sxs-lookup"><span data-stu-id="902b3-154">Int32</span></span>| <span data-ttu-id="902b3-155">Значение, используемое при настройке свойства *Weight* записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="902b3-155">Value to use when configuring the *weight* property of the SRV record at the DNS host.</span></span> |

## <a name="relationships"></a><span data-ttu-id="902b3-156">Связи</span><span class="sxs-lookup"><span data-stu-id="902b3-156">Relationships</span></span>
<span data-ttu-id="902b3-157">Нет</span><span class="sxs-lookup"><span data-stu-id="902b3-157">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="902b3-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="902b3-158">JSON representation</span></span>
<span data-ttu-id="902b3-159">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="902b3-159">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "domainDnsSrvRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
