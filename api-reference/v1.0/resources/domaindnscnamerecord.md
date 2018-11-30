---
title: Тип ресурса domainDnsCnameRecord
description: Представляет запись CNAME, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от объекта DomainDnsRecord.
ms.openlocfilehash: 1c8df7148a4d843d5cd6278f5cbcc03358159424
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026891"
---
# <a name="domaindnscnamerecord-resource-type"></a><span data-ttu-id="e6148-104">Тип ресурса domainDnsCnameRecord</span><span class="sxs-lookup"><span data-stu-id="e6148-104">domainDnsCnameRecord resource type</span></span>

<span data-ttu-id="e6148-p102">Представляет запись CNAME, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от объекта [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="e6148-p102">Represents a CNAME record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>


## <a name="methods"></a><span data-ttu-id="e6148-107">Методы</span><span class="sxs-lookup"><span data-stu-id="e6148-107">Methods</span></span>
<span data-ttu-id="e6148-p103">Прямые запросы к этому ресурсу не поддерживаются. Сведения о том, как запрашивать записи службы доменов, см. в статье [о доменах](domain.md).</span><span class="sxs-lookup"><span data-stu-id="e6148-p103">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="e6148-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="e6148-110">Properties</span></span>
| <span data-ttu-id="e6148-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="e6148-111">Property</span></span>     | <span data-ttu-id="e6148-112">Тип</span><span class="sxs-lookup"><span data-stu-id="e6148-112">Type</span></span>   |<span data-ttu-id="e6148-113">Описание</span><span class="sxs-lookup"><span data-stu-id="e6148-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e6148-114">canonicalName</span><span class="sxs-lookup"><span data-stu-id="e6148-114">canonicalName</span></span>|<span data-ttu-id="e6148-115">String</span><span class="sxs-lookup"><span data-stu-id="e6148-115">String</span></span>| <span data-ttu-id="e6148-p104">Каноническое имя записи CNAME. Используется для настройки записи CNAME в узле DNS.</span><span class="sxs-lookup"><span data-stu-id="e6148-p104">The canonical name of the CNAME record. Used to configure the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="e6148-118">id</span><span class="sxs-lookup"><span data-stu-id="e6148-118">id</span></span>|<span data-ttu-id="e6148-119">String</span><span class="sxs-lookup"><span data-stu-id="e6148-119">String</span></span>| <span data-ttu-id="e6148-p105">Уникальный идентификатор, назначенный этому объекту. Не допускает значения null, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e6148-p105">Unique identifier assigned to this entity. Not nullable, Read-only</span></span>|
|<span data-ttu-id="e6148-122">isOptional</span><span class="sxs-lookup"><span data-stu-id="e6148-122">isOptional</span></span>|<span data-ttu-id="e6148-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6148-123">Boolean</span></span>| <span data-ttu-id="e6148-p106">Если имеет значение false, пользователю необходимо настроить запись CNAME на узле DNS, чтобы службы Microsoft Online Services правильно работали с доменом. Не допускает значения null.</span><span class="sxs-lookup"><span data-stu-id="e6148-p106">If false, the CNAME record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain. Not nullable</span></span> |
|<span data-ttu-id="e6148-126">label</span><span class="sxs-lookup"><span data-stu-id="e6148-126">label</span></span>|<span data-ttu-id="e6148-127">String</span><span class="sxs-lookup"><span data-stu-id="e6148-127">String</span></span>| <span data-ttu-id="e6148-128">Значение, используемое при настройке *псевдонима, узла и имени* для записи CNAME на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="e6148-128">Value used when configuring the *alias/host/name* of the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="e6148-129">recordType</span><span class="sxs-lookup"><span data-stu-id="e6148-129">recordType</span></span>|<span data-ttu-id="e6148-130">String</span><span class="sxs-lookup"><span data-stu-id="e6148-130">String</span></span>| <span data-ttu-id="e6148-p107">Тип записи DNS. Это свойство всегда имеет значение *CName*. Ключевое.</span><span class="sxs-lookup"><span data-stu-id="e6148-p107">Type of DNS record. The value is always *CName*. Key</span></span>|
|<span data-ttu-id="e6148-134">supportedService</span><span class="sxs-lookup"><span data-stu-id="e6148-134">supportedService</span></span>|<span data-ttu-id="e6148-135">String</span><span class="sxs-lookup"><span data-stu-id="e6148-135">String</span></span>| <span data-ttu-id="e6148-136">Служба или функция Microsoft Online, имеющая зависимость от этой записи CNAME.</span><span class="sxs-lookup"><span data-stu-id="e6148-136">Microsoft Online Service or feature that has a dependency on this CNAME record.</span></span></br></br><span data-ttu-id="e6148-137">Может иметь одно из следующих значений: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer* или *Intune*.</span><span class="sxs-lookup"><span data-stu-id="e6148-137">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="e6148-138">ttl</span><span class="sxs-lookup"><span data-stu-id="e6148-138">ttl</span></span>|<span data-ttu-id="e6148-139">Int32</span><span class="sxs-lookup"><span data-stu-id="e6148-139">Int32</span></span>| <span data-ttu-id="e6148-p108">Значение, используемое при настройке свойства срока жизни (ttl) записи CNAME на узле DNS. Не допускает значения null.</span><span class="sxs-lookup"><span data-stu-id="e6148-p108">Value to use when configuring the time-to-live (ttl) property of the CNAME record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="e6148-142">Связи</span><span class="sxs-lookup"><span data-stu-id="e6148-142">Relationships</span></span>
<span data-ttu-id="e6148-143">Нет</span><span class="sxs-lookup"><span data-stu-id="e6148-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e6148-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e6148-144">JSON representation</span></span>
<span data-ttu-id="e6148-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e6148-145">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsCnameRecord"
}-->

```json
{
  "canonicalName": "String",
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "ttl": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsCnameRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->