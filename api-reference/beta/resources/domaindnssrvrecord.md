---
title: Тип ресурса domainDnsSrvRecord
description: Представляет запись SRV, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от объекта DomainDnsRecord.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bdbc2246340d5cd15529dd05101567bc04d1e607
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524480"
---
# <a name="domaindnssrvrecord-resource-type"></a><span data-ttu-id="7a6c0-104">Тип ресурса domainDnsSrvRecord</span><span class="sxs-lookup"><span data-stu-id="7a6c0-104">domainDnsSrvRecord resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a6c0-p102">Представляет запись SRV, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от объекта [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="7a6c0-p102">Represents a SRV record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="7a6c0-107">Методы</span><span class="sxs-lookup"><span data-stu-id="7a6c0-107">Methods</span></span>
<span data-ttu-id="7a6c0-p103">Прямые запросы к этому ресурсу не поддерживаются. Сведения о том, как запрашивать записи службы доменов, см. в статье [о доменах](domain.md).</span><span class="sxs-lookup"><span data-stu-id="7a6c0-p103">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="7a6c0-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="7a6c0-110">Properties</span></span>
| <span data-ttu-id="7a6c0-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="7a6c0-111">Property</span></span>     | <span data-ttu-id="7a6c0-112">Тип</span><span class="sxs-lookup"><span data-stu-id="7a6c0-112">Type</span></span>   |<span data-ttu-id="7a6c0-113">Описание</span><span class="sxs-lookup"><span data-stu-id="7a6c0-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7a6c0-114">id</span><span class="sxs-lookup"><span data-stu-id="7a6c0-114">id</span></span>|<span data-ttu-id="7a6c0-115">String</span><span class="sxs-lookup"><span data-stu-id="7a6c0-115">String</span></span>| <span data-ttu-id="7a6c0-p104">Уникальный идентификатор, назначенный этому объекту. Не допускает значения null, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7a6c0-p104">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span>|
|<span data-ttu-id="7a6c0-118">isOptional</span><span class="sxs-lookup"><span data-stu-id="7a6c0-118">isOptional</span></span>|<span data-ttu-id="7a6c0-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="7a6c0-119">Boolean</span></span>| <span data-ttu-id="7a6c0-120">Если указано значение false, для правильной работы Microsoft Online Services с доменом пользователь должен настроить запись SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="7a6c0-120">If false, the SRV record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="7a6c0-121">label</span><span class="sxs-lookup"><span data-stu-id="7a6c0-121">label</span></span>|<span data-ttu-id="7a6c0-122">String</span><span class="sxs-lookup"><span data-stu-id="7a6c0-122">String</span></span>| <span data-ttu-id="7a6c0-123">Значение, используемое при настройке свойства *name* записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="7a6c0-123">Value used when configuring the *name* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="7a6c0-124">nameTarget</span><span class="sxs-lookup"><span data-stu-id="7a6c0-124">nameTarget</span></span>|<span data-ttu-id="7a6c0-125">String</span><span class="sxs-lookup"><span data-stu-id="7a6c0-125">String</span></span>| <span data-ttu-id="7a6c0-126">Значение, используемое при настройке свойства *Target* записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="7a6c0-126">Value to use when configuring the *Target* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="7a6c0-127">port</span><span class="sxs-lookup"><span data-stu-id="7a6c0-127">port</span></span>|<span data-ttu-id="7a6c0-128">Int32</span><span class="sxs-lookup"><span data-stu-id="7a6c0-128">Int32</span></span>| <span data-ttu-id="7a6c0-129">Значение, используемое при настройке свойства *port* записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="7a6c0-129">Value to use when configuring the *port* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="7a6c0-130">priority</span><span class="sxs-lookup"><span data-stu-id="7a6c0-130">priority</span></span>|<span data-ttu-id="7a6c0-131">Int32</span><span class="sxs-lookup"><span data-stu-id="7a6c0-131">Int32</span></span>| <span data-ttu-id="7a6c0-132">Значение, используемое при настройке свойства *priority* записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="7a6c0-132">Value to use when configuring the *priority* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="7a6c0-133">protocol</span><span class="sxs-lookup"><span data-stu-id="7a6c0-133">protocol</span></span>|<span data-ttu-id="7a6c0-134">String</span><span class="sxs-lookup"><span data-stu-id="7a6c0-134">String</span></span>| <span data-ttu-id="7a6c0-135">Значение, используемое при настройке свойства *protocol* для записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="7a6c0-135">Value to use when configuring the *protocol* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="7a6c0-136">recordType</span><span class="sxs-lookup"><span data-stu-id="7a6c0-136">recordType</span></span>|<span data-ttu-id="7a6c0-137">String</span><span class="sxs-lookup"><span data-stu-id="7a6c0-137">String</span></span>|  <span data-ttu-id="7a6c0-p105">Тип записи DNS. Это свойство всегда имеет значение *Srv*. Ключ.</span><span class="sxs-lookup"><span data-stu-id="7a6c0-p105">Type of DNS record. The value is always *Srv*. Key</span></span> |
|<span data-ttu-id="7a6c0-141">service</span><span class="sxs-lookup"><span data-stu-id="7a6c0-141">service</span></span>|<span data-ttu-id="7a6c0-142">String</span><span class="sxs-lookup"><span data-stu-id="7a6c0-142">String</span></span>| <span data-ttu-id="7a6c0-143">Значение, используемое при настройке свойства *service* для записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="7a6c0-143">Value to use when configuring the *service* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="7a6c0-144">supportedService</span><span class="sxs-lookup"><span data-stu-id="7a6c0-144">supportedService</span></span>|<span data-ttu-id="7a6c0-145">Строка</span><span class="sxs-lookup"><span data-stu-id="7a6c0-145">String</span></span>| <span data-ttu-id="7a6c0-146">Служба или компонент Microsoft Online Services, зависящие от этой записи типа SRV.</span><span class="sxs-lookup"><span data-stu-id="7a6c0-146">Microsoft Online Service or feature that has a dependency on this SRV record.</span></span></br></br><span data-ttu-id="7a6c0-147">Возможные значения: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*.</span><span class="sxs-lookup"><span data-stu-id="7a6c0-147">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="7a6c0-148">ttl</span><span class="sxs-lookup"><span data-stu-id="7a6c0-148">ttl</span></span>|<span data-ttu-id="7a6c0-149">Int32</span><span class="sxs-lookup"><span data-stu-id="7a6c0-149">Int32</span></span>| <span data-ttu-id="7a6c0-p106">Значение, используемое при настройке свойства *ttl* (срока жизни) для записи SRV на узле DNS. Не допускает значения null.</span><span class="sxs-lookup"><span data-stu-id="7a6c0-p106">Value to use when configuring the *time-to-live (ttl)* property of the SRV record at the DNS host. Not nullable</span></span> |
|<span data-ttu-id="7a6c0-152">weight</span><span class="sxs-lookup"><span data-stu-id="7a6c0-152">weight</span></span>|<span data-ttu-id="7a6c0-153">Int32</span><span class="sxs-lookup"><span data-stu-id="7a6c0-153">Int32</span></span>| <span data-ttu-id="7a6c0-154">Значение, используемое при настройке свойства *weight* записи SRV на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="7a6c0-154">Value to use when configuring the *weight* property of the SRV record at the DNS host.</span></span> |

## <a name="relationships"></a><span data-ttu-id="7a6c0-155">Связи</span><span class="sxs-lookup"><span data-stu-id="7a6c0-155">Relationships</span></span>
<span data-ttu-id="7a6c0-156">Нет</span><span class="sxs-lookup"><span data-stu-id="7a6c0-156">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="7a6c0-157">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7a6c0-157">JSON representation</span></span>
<span data-ttu-id="7a6c0-158">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7a6c0-158">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/domaindnssrvrecord.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
