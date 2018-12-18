---
title: Тип ресурса domainDnsMxRecord
description: Представляет запись MX, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от объекта DomainDnsRecord.
author: lleonard-msft
ms.openlocfilehash: e06b3c405f4ad5e2e561e57876ef010bddb1068d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27345838"
---
# <a name="domaindnsmxrecord-resource-type"></a><span data-ttu-id="ae839-104">Тип ресурса domainDnsMxRecord</span><span class="sxs-lookup"><span data-stu-id="ae839-104">domainDnsMxRecord resource type</span></span>

<span data-ttu-id="ae839-p102">Представляет запись MX, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от объекта [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="ae839-p102">Represents a MX record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="ae839-107">Методы</span><span class="sxs-lookup"><span data-stu-id="ae839-107">Methods</span></span>
<span data-ttu-id="ae839-p103">Прямые запросы к этому ресурсу не поддерживаются. Сведения о том, как запрашивать записи службы доменов, см. в статье [о доменах](domain.md).</span><span class="sxs-lookup"><span data-stu-id="ae839-p103">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="ae839-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="ae839-110">Properties</span></span>
| <span data-ttu-id="ae839-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="ae839-111">Property</span></span>     | <span data-ttu-id="ae839-112">Тип</span><span class="sxs-lookup"><span data-stu-id="ae839-112">Type</span></span>   |<span data-ttu-id="ae839-113">Описание</span><span class="sxs-lookup"><span data-stu-id="ae839-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ae839-114">id</span><span class="sxs-lookup"><span data-stu-id="ae839-114">id</span></span>|<span data-ttu-id="ae839-115">Строка</span><span class="sxs-lookup"><span data-stu-id="ae839-115">String</span></span>| <span data-ttu-id="ae839-p104">Уникальный идентификатор, назначенный этому объекту. Не допускает значения null, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ae839-p104">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span>|
|<span data-ttu-id="ae839-118">isOptional</span><span class="sxs-lookup"><span data-stu-id="ae839-118">isOptional</span></span>|<span data-ttu-id="ae839-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae839-119">Boolean</span></span>| <span data-ttu-id="ae839-120">Если указано значение false, для правильной работы Microsoft Online Services с доменом пользователь должен настроить запись MX на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="ae839-120">If false, the MX record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="ae839-121">label</span><span class="sxs-lookup"><span data-stu-id="ae839-121">label</span></span>|<span data-ttu-id="ae839-122">String</span><span class="sxs-lookup"><span data-stu-id="ae839-122">String</span></span>| <span data-ttu-id="ae839-123">Значение, используемое при настройке свойства *псевдонима, узла или имени* для записи MX на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="ae839-123">Value used when configuring the *alias/host/name* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="ae839-124">mailExchange</span><span class="sxs-lookup"><span data-stu-id="ae839-124">mailExchange</span></span>|<span data-ttu-id="ae839-125">String</span><span class="sxs-lookup"><span data-stu-id="ae839-125">String</span></span>| <span data-ttu-id="ae839-126">Значение, используемое при настройке *значения, ответа или целевого объекта* для записи MX на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="ae839-126">Value used when configuring the *answer/destination/value* of the MX record at the DNS host.</span></span>|
|<span data-ttu-id="ae839-127">preference</span><span class="sxs-lookup"><span data-stu-id="ae839-127">preference</span></span>|<span data-ttu-id="ae839-128">Int32</span><span class="sxs-lookup"><span data-stu-id="ae839-128">Int32</span></span>| <span data-ttu-id="ae839-129">Значение, используемое при настройке свойства *приоритета или предпочтения* для записи MX на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="ae839-129">Value used when configuring the *Preference/Priority* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="ae839-130">recordType</span><span class="sxs-lookup"><span data-stu-id="ae839-130">recordType</span></span>|<span data-ttu-id="ae839-131">String</span><span class="sxs-lookup"><span data-stu-id="ae839-131">String</span></span>| <span data-ttu-id="ae839-p105">Тип записи DNS. Это свойство всегда имеет значение *Mx*. Ключ.</span><span class="sxs-lookup"><span data-stu-id="ae839-p105">Type of DNS record. The value is always *Mx*. Key</span></span> |
|<span data-ttu-id="ae839-135">supportedService</span><span class="sxs-lookup"><span data-stu-id="ae839-135">supportedService</span></span>|<span data-ttu-id="ae839-136">String</span><span class="sxs-lookup"><span data-stu-id="ae839-136">String</span></span>| <span data-ttu-id="ae839-137">Служба или компонент Microsoft Online Services, зависящие от этой записи типа MX.</span><span class="sxs-lookup"><span data-stu-id="ae839-137">Microsoft Online Service or feature that has a dependency on this MX record.</span></span></br></br><span data-ttu-id="ae839-138">Возможные значения: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*.</span><span class="sxs-lookup"><span data-stu-id="ae839-138">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="ae839-139">ttl</span><span class="sxs-lookup"><span data-stu-id="ae839-139">ttl</span></span>|<span data-ttu-id="ae839-140">Int32</span><span class="sxs-lookup"><span data-stu-id="ae839-140">Int32</span></span>| <span data-ttu-id="ae839-p106">Значение, используемое при настройке свойства *ttl* (срока жизни) для записи MX на узле DNS. Не допускает значения null.</span><span class="sxs-lookup"><span data-stu-id="ae839-p106">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="ae839-143">Связи</span><span class="sxs-lookup"><span data-stu-id="ae839-143">Relationships</span></span>
<span data-ttu-id="ae839-144">Нет</span><span class="sxs-lookup"><span data-stu-id="ae839-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ae839-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ae839-145">JSON representation</span></span>
<span data-ttu-id="ae839-146">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ae839-146">Here is a JSON representation of the resource.</span></span>

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