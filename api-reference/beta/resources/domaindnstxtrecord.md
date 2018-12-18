---
title: Тип ресурса domainDnsTxtRecord
description: Представляет запись типа TXT, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от объекта DomainDnsRecord.
author: lleonard-msft
ms.openlocfilehash: caefb97b39219c282c45949b504c3d0b91cdada9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349016"
---
# <a name="domaindnstxtrecord-resource-type"></a><span data-ttu-id="979ed-104">Тип ресурса domainDnsTxtRecord</span><span class="sxs-lookup"><span data-stu-id="979ed-104">domainDnsTxtRecord resource type</span></span>

> <span data-ttu-id="979ed-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="979ed-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="979ed-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="979ed-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="979ed-p103">Представляет запись типа TXT, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от объекта [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="979ed-p103">Represents a TXT record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="979ed-109">Методы</span><span class="sxs-lookup"><span data-stu-id="979ed-109">Methods</span></span>
<span data-ttu-id="979ed-p104">Прямые запросы к этому ресурсу не поддерживаются. Сведения о том, как запрашивать записи службы доменов, см. в статье [о доменах](domain.md).</span><span class="sxs-lookup"><span data-stu-id="979ed-p104">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="979ed-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="979ed-112">Properties</span></span>
| <span data-ttu-id="979ed-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="979ed-113">Property</span></span>     | <span data-ttu-id="979ed-114">Тип</span><span class="sxs-lookup"><span data-stu-id="979ed-114">Type</span></span>   |<span data-ttu-id="979ed-115">Описание</span><span class="sxs-lookup"><span data-stu-id="979ed-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="979ed-116">id</span><span class="sxs-lookup"><span data-stu-id="979ed-116">id</span></span>|<span data-ttu-id="979ed-117">Строка</span><span class="sxs-lookup"><span data-stu-id="979ed-117">String</span></span>| <span data-ttu-id="979ed-p105">Уникальный идентификатор, назначенный этому объекту. Не допускает значения null, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="979ed-p105">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span> |
|<span data-ttu-id="979ed-120">isOptional</span><span class="sxs-lookup"><span data-stu-id="979ed-120">isOptional</span></span>|<span data-ttu-id="979ed-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="979ed-121">Boolean</span></span>| <span data-ttu-id="979ed-122">Если имеет значение false, пользователю необходимо настроить запись типа TXT на узле DNS, чтобы службы Microsoft Online Services правильно работали с доменом.</span><span class="sxs-lookup"><span data-stu-id="979ed-122">If false, the TXT record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="979ed-123">label</span><span class="sxs-lookup"><span data-stu-id="979ed-123">label</span></span>|<span data-ttu-id="979ed-124">String</span><span class="sxs-lookup"><span data-stu-id="979ed-124">String</span></span>| <span data-ttu-id="979ed-125">Значение, используемое при настройке свойства *name* для записи типа TXT на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="979ed-125">Value to use when configuring the *name* property of the TXT record at the DNS host.</span></span>|
|<span data-ttu-id="979ed-126">recordType</span><span class="sxs-lookup"><span data-stu-id="979ed-126">recordType</span></span>|<span data-ttu-id="979ed-127">String</span><span class="sxs-lookup"><span data-stu-id="979ed-127">String</span></span>| <span data-ttu-id="979ed-p106">Тип записи DNS. Это свойство всегда имеет значение *Txt*. Ключ.</span><span class="sxs-lookup"><span data-stu-id="979ed-p106">Type of DNS record. The value is always *Txt*. Key</span></span> |
|<span data-ttu-id="979ed-131">supportedService</span><span class="sxs-lookup"><span data-stu-id="979ed-131">supportedService</span></span>|<span data-ttu-id="979ed-132">String</span><span class="sxs-lookup"><span data-stu-id="979ed-132">String</span></span>| <span data-ttu-id="979ed-133">Служба или компонент Microsoft Online Services, зависящие от этой записи типа TXT.</span><span class="sxs-lookup"><span data-stu-id="979ed-133">Microsoft Online Service or feature that has a dependency on this TXT record.</span></span></br></br><span data-ttu-id="979ed-134">Возможные значения: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*.</span><span class="sxs-lookup"><span data-stu-id="979ed-134">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="979ed-135">text</span><span class="sxs-lookup"><span data-stu-id="979ed-135">text</span></span>|<span data-ttu-id="979ed-136">String</span><span class="sxs-lookup"><span data-stu-id="979ed-136">String</span></span>| <span data-ttu-id="979ed-137">Значение, используемое при настройке свойства *text* на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="979ed-137">Value used when configuring the *text* property at the DNS host.</span></span> |
|<span data-ttu-id="979ed-138">ttl</span><span class="sxs-lookup"><span data-stu-id="979ed-138">ttl</span></span>|<span data-ttu-id="979ed-139">Int32</span><span class="sxs-lookup"><span data-stu-id="979ed-139">Int32</span></span>| <span data-ttu-id="979ed-p107">Значение, используемое при настройке свойства *ttl* (срока жизни) для записи MX на узле DNS. Не допускает значения null.</span><span class="sxs-lookup"><span data-stu-id="979ed-p107">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="979ed-142">Связи</span><span class="sxs-lookup"><span data-stu-id="979ed-142">Relationships</span></span>
<span data-ttu-id="979ed-143">Нет</span><span class="sxs-lookup"><span data-stu-id="979ed-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="979ed-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="979ed-144">JSON representation</span></span>
<span data-ttu-id="979ed-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="979ed-145">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsTxtRecord"
}-->

```json
{
  "canonicalName": "String",
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "text": "String",
  "ttl": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsTxtRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->