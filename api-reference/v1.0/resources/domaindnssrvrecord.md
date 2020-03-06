---
title: Тип ресурса Домаинднссрврекорд
description: Представляет запись SRV, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от объекта DomainDnsRecord.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 32a9461cb28bc51489ddca6f3b569871bcc584d0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531597"
---
# <a name="domaindnssrvrecord-resource-type"></a><span data-ttu-id="d596c-104">Тип ресурса Домаинднссрврекорд</span><span class="sxs-lookup"><span data-stu-id="d596c-104">domainDnsSrvRecord resource type</span></span>

<span data-ttu-id="d596c-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d596c-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d596c-106">Представляет запись SRV, добавленную в файл зоны DNS определенного домена в клиенте.</span><span class="sxs-lookup"><span data-stu-id="d596c-106">Represents a SRV record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="d596c-107">Наследуется от объекта [DomainDnsRecord](domaindnsrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="d596c-107">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="d596c-108">Методы</span><span class="sxs-lookup"><span data-stu-id="d596c-108">Methods</span></span>
<span data-ttu-id="d596c-109">Прямые запросы к этому ресурсу не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="d596c-109">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="d596c-110">Сведения о том, как запросить записи службы домена, можно найти в разделе [domain](domain.md) .</span><span class="sxs-lookup"><span data-stu-id="d596c-110">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="d596c-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="d596c-111">Properties</span></span>
| <span data-ttu-id="d596c-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="d596c-112">Property</span></span>     | <span data-ttu-id="d596c-113">Тип</span><span class="sxs-lookup"><span data-stu-id="d596c-113">Type</span></span>   |<span data-ttu-id="d596c-114">Описание</span><span class="sxs-lookup"><span data-stu-id="d596c-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d596c-115">id</span><span class="sxs-lookup"><span data-stu-id="d596c-115">id</span></span>|<span data-ttu-id="d596c-116">Строка</span><span class="sxs-lookup"><span data-stu-id="d596c-116">String</span></span>| <span data-ttu-id="d596c-117">Уникальный идентификатор, назначенный этой сущности.</span><span class="sxs-lookup"><span data-stu-id="d596c-117">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="d596c-118">Не допускает значения NULL и только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d596c-118">Not nullable, Read-only.</span></span>|
|<span data-ttu-id="d596c-119">Переключатель</span><span class="sxs-lookup"><span data-stu-id="d596c-119">isOptional</span></span>|<span data-ttu-id="d596c-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="d596c-120">Boolean</span></span>| <span data-ttu-id="d596c-121">Если задано значение false, запись SRV должна быть настроена клиентом на узле DNS для правильной работы Microsoft Online Services с доменом.</span><span class="sxs-lookup"><span data-stu-id="d596c-121">If false, the SRV record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="d596c-122">label</span><span class="sxs-lookup"><span data-stu-id="d596c-122">label</span></span>|<span data-ttu-id="d596c-123">Строка</span><span class="sxs-lookup"><span data-stu-id="d596c-123">String</span></span>| <span data-ttu-id="d596c-124">Значение, используемое при настройке свойства *Name* записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="d596c-124">Value used when configuring the *name* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="d596c-125">наметаржет</span><span class="sxs-lookup"><span data-stu-id="d596c-125">nameTarget</span></span>|<span data-ttu-id="d596c-126">Строка</span><span class="sxs-lookup"><span data-stu-id="d596c-126">String</span></span>| <span data-ttu-id="d596c-127">Значение, используемое при настройке свойства *Target* записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="d596c-127">Value to use when configuring the *Target* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="d596c-128">порта</span><span class="sxs-lookup"><span data-stu-id="d596c-128">port</span></span>|<span data-ttu-id="d596c-129">Int32</span><span class="sxs-lookup"><span data-stu-id="d596c-129">Int32</span></span>| <span data-ttu-id="d596c-130">Значение, используемое при настройке свойства *Port* записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="d596c-130">Value to use when configuring the *port* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="d596c-131">priority</span><span class="sxs-lookup"><span data-stu-id="d596c-131">priority</span></span>|<span data-ttu-id="d596c-132">Int32</span><span class="sxs-lookup"><span data-stu-id="d596c-132">Int32</span></span>| <span data-ttu-id="d596c-133">Значение, используемое при настройке свойства *Priority* записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="d596c-133">Value to use when configuring the *priority* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="d596c-134">Protocol</span><span class="sxs-lookup"><span data-stu-id="d596c-134">protocol</span></span>|<span data-ttu-id="d596c-135">Строка</span><span class="sxs-lookup"><span data-stu-id="d596c-135">String</span></span>| <span data-ttu-id="d596c-136">Значение, используемое при настройке свойства *Protocol* записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="d596c-136">Value to use when configuring the *protocol* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="d596c-137">recordType</span><span class="sxs-lookup"><span data-stu-id="d596c-137">recordType</span></span>|<span data-ttu-id="d596c-138">Строка</span><span class="sxs-lookup"><span data-stu-id="d596c-138">String</span></span>|  <span data-ttu-id="d596c-139">Тип записи DNS.</span><span class="sxs-lookup"><span data-stu-id="d596c-139">Type of DNS record.</span></span> <span data-ttu-id="d596c-140">Значение — всегда *SRV*.</span><span class="sxs-lookup"><span data-stu-id="d596c-140">The value is always *Srv*.</span></span> <span data-ttu-id="d596c-141">Key</span><span class="sxs-lookup"><span data-stu-id="d596c-141">Key</span></span> |
|<span data-ttu-id="d596c-142">service</span><span class="sxs-lookup"><span data-stu-id="d596c-142">service</span></span>|<span data-ttu-id="d596c-143">String</span><span class="sxs-lookup"><span data-stu-id="d596c-143">String</span></span>| <span data-ttu-id="d596c-144">Значение, используемое при настройке свойства *Service* для записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="d596c-144">Value to use when configuring the *service* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="d596c-145">суппортедсервице</span><span class="sxs-lookup"><span data-stu-id="d596c-145">supportedService</span></span>|<span data-ttu-id="d596c-146">Строка</span><span class="sxs-lookup"><span data-stu-id="d596c-146">String</span></span>| <span data-ttu-id="d596c-147">Служба или компонент Microsoft Online, который имеет зависимость от этой записи SRV.</span><span class="sxs-lookup"><span data-stu-id="d596c-147">Microsoft Online Service or feature that has a dependency on this SRV record.</span></span></br></br><span data-ttu-id="d596c-148">Может принимать одно из следующих значений: **null**, *Email*, *SharePoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="d596c-148">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="d596c-149">используем</span><span class="sxs-lookup"><span data-stu-id="d596c-149">ttl</span></span>|<span data-ttu-id="d596c-150">Int32</span><span class="sxs-lookup"><span data-stu-id="d596c-150">Int32</span></span>| <span data-ttu-id="d596c-151">Значение, используемое при настройке свойства срока *жизни (TTL)* записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="d596c-151">Value to use when configuring the *time-to-live (ttl)* property of the SRV record at the DNS host.</span></span> <span data-ttu-id="d596c-152">Не допускает значение null</span><span class="sxs-lookup"><span data-stu-id="d596c-152">Not nullable</span></span> |
|<span data-ttu-id="d596c-153">weight</span><span class="sxs-lookup"><span data-stu-id="d596c-153">weight</span></span>|<span data-ttu-id="d596c-154">Int32</span><span class="sxs-lookup"><span data-stu-id="d596c-154">Int32</span></span>| <span data-ttu-id="d596c-155">Значение, используемое при настройке свойства *Weight* записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="d596c-155">Value to use when configuring the *weight* property of the SRV record at the DNS host.</span></span> |

## <a name="relationships"></a><span data-ttu-id="d596c-156">Связи</span><span class="sxs-lookup"><span data-stu-id="d596c-156">Relationships</span></span>
<span data-ttu-id="d596c-157">Нет</span><span class="sxs-lookup"><span data-stu-id="d596c-157">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d596c-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d596c-158">JSON representation</span></span>
<span data-ttu-id="d596c-159">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d596c-159">Here is a JSON representation of the resource.</span></span>

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
