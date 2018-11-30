---
title: Тип ресурса domainDnsMxRecord
description: Представляет запись MX, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от объекта DomainDnsRecord.
ms.openlocfilehash: 54a72f8e420d0313303b0787e803933888fb1e57
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025945"
---
# <a name="domaindnsmxrecord-resource-type"></a><span data-ttu-id="4739a-104">Тип ресурса domainDnsMxRecord</span><span class="sxs-lookup"><span data-stu-id="4739a-104">domainDnsMxRecord resource type</span></span>

<span data-ttu-id="4739a-p102">Представляет запись MX, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от объекта [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="4739a-p102">Represents a MX record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="4739a-107">Методы</span><span class="sxs-lookup"><span data-stu-id="4739a-107">Methods</span></span>
<span data-ttu-id="4739a-p103">Прямые запросы к этому ресурсу не поддерживаются. Сведения о том, как запрашивать записи службы доменов, см. в статье [о доменах](domain.md).</span><span class="sxs-lookup"><span data-stu-id="4739a-p103">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="4739a-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="4739a-110">Properties</span></span>
| <span data-ttu-id="4739a-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="4739a-111">Property</span></span>     | <span data-ttu-id="4739a-112">Тип</span><span class="sxs-lookup"><span data-stu-id="4739a-112">Type</span></span>   |<span data-ttu-id="4739a-113">Описание</span><span class="sxs-lookup"><span data-stu-id="4739a-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4739a-114">id</span><span class="sxs-lookup"><span data-stu-id="4739a-114">id</span></span>|<span data-ttu-id="4739a-115">String</span><span class="sxs-lookup"><span data-stu-id="4739a-115">String</span></span>| <span data-ttu-id="4739a-p104">Уникальный идентификатор, назначенный этому объекту. Не допускает значения null, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4739a-p104">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span>|
|<span data-ttu-id="4739a-118">isOptional</span><span class="sxs-lookup"><span data-stu-id="4739a-118">isOptional</span></span>|<span data-ttu-id="4739a-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="4739a-119">Boolean</span></span>| <span data-ttu-id="4739a-120">Если указано значение false, для правильной работы Microsoft Online Services с доменом пользователь должен настроить запись MX на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="4739a-120">If false, the MX record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="4739a-121">label</span><span class="sxs-lookup"><span data-stu-id="4739a-121">label</span></span>|<span data-ttu-id="4739a-122">String</span><span class="sxs-lookup"><span data-stu-id="4739a-122">String</span></span>| <span data-ttu-id="4739a-123">Значение, используемое при настройке свойства *псевдонима, узла или имени* для записи MX на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="4739a-123">Value used when configuring the *alias/host/name* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="4739a-124">mailExchange</span><span class="sxs-lookup"><span data-stu-id="4739a-124">mailExchange</span></span>|<span data-ttu-id="4739a-125">String</span><span class="sxs-lookup"><span data-stu-id="4739a-125">String</span></span>| <span data-ttu-id="4739a-126">Значение, используемое при настройке *значения, ответа или целевого объекта* для записи MX на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="4739a-126">Value used when configuring the *answer/destination/value* of the MX record at the DNS host.</span></span>|
|<span data-ttu-id="4739a-127">preference</span><span class="sxs-lookup"><span data-stu-id="4739a-127">preference</span></span>|<span data-ttu-id="4739a-128">Int32</span><span class="sxs-lookup"><span data-stu-id="4739a-128">Int32</span></span>| <span data-ttu-id="4739a-129">Значение, используемое при настройке свойства *приоритета или предпочтения* для записи MX на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="4739a-129">Value used when configuring the *Preference/Priority* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="4739a-130">recordType</span><span class="sxs-lookup"><span data-stu-id="4739a-130">recordType</span></span>|<span data-ttu-id="4739a-131">String</span><span class="sxs-lookup"><span data-stu-id="4739a-131">String</span></span>| <span data-ttu-id="4739a-p105">Тип записи DNS. Это свойство всегда имеет значение *Mx*. Ключ.</span><span class="sxs-lookup"><span data-stu-id="4739a-p105">Type of DNS record. The value is always *Mx*. Key</span></span> |
|<span data-ttu-id="4739a-135">supportedService</span><span class="sxs-lookup"><span data-stu-id="4739a-135">supportedService</span></span>|<span data-ttu-id="4739a-136">String</span><span class="sxs-lookup"><span data-stu-id="4739a-136">String</span></span>| <span data-ttu-id="4739a-137">Служба или компонент Microsoft Online Services, зависящие от этой записи типа MX.</span><span class="sxs-lookup"><span data-stu-id="4739a-137">Microsoft Online Service or feature that has a dependency on this MX record.</span></span></br></br><span data-ttu-id="4739a-138">Возможные значения: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*.</span><span class="sxs-lookup"><span data-stu-id="4739a-138">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="4739a-139">ttl</span><span class="sxs-lookup"><span data-stu-id="4739a-139">ttl</span></span>|<span data-ttu-id="4739a-140">Int32</span><span class="sxs-lookup"><span data-stu-id="4739a-140">Int32</span></span>| <span data-ttu-id="4739a-p106">Значение, используемое при настройке свойства *ttl* (срока жизни) для записи MX на узле DNS. Не допускает значения null.</span><span class="sxs-lookup"><span data-stu-id="4739a-p106">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="4739a-143">Связи</span><span class="sxs-lookup"><span data-stu-id="4739a-143">Relationships</span></span>
<span data-ttu-id="4739a-144">Нет</span><span class="sxs-lookup"><span data-stu-id="4739a-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4739a-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4739a-145">JSON representation</span></span>
<span data-ttu-id="4739a-146">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4739a-146">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsMxRecord"
}-->

```json
{
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "mailExchange": "String",
  "preference": 1024,
  "recordType": "String",
  "supportedService": "String",
  "ttl": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsMxRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->