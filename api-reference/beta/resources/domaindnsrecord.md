---
title: Тип ресурса domainDnsRecord
description: Для каждого домена в клиентов может потребоваться добавление записи DNS для файла зоны DNS домена этого домена, которые могут использоваться с Microsoft Online Services. Сущность **DomainDnsRecord** используется для представления таких записей DNS. Базовая сущность для DomainDnsCnameRecord, DomainDnsMxRecord, DomainDnsSrvRecord и DomainDnsSrvRecord сущностей.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f5c760ba9a2100bbefd0353c2c02019e7a04354b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912962"
---
# <a name="domaindnsrecord-resource-type"></a><span data-ttu-id="0871d-105">Тип ресурса domainDnsRecord</span><span class="sxs-lookup"><span data-stu-id="0871d-105">domainDnsRecord resource type</span></span>

> <span data-ttu-id="0871d-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0871d-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0871d-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0871d-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0871d-p103">Для работы служб Microsoft Online Services с доменом необходимо добавить записи DNS в файл зоны DNS домена. Объект **DomainDnsRecord** представляет такие записи DNS. Базовый объект для объектов [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md) и [DomainDnsSrvRecord](domaindnssrvrecord.md).</span><span class="sxs-lookup"><span data-stu-id="0871d-p103">For each domain in the tenant, you may be required to add DNS record(s) to the DNS zone file of the domain before the domain can be used by Microsoft Online Services. The **DomainDnsRecord** entity is used to present such DNS records. Base entity for [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md) and [DomainDnsSrvRecord](domaindnssrvrecord.md) entities.</span></span>

## <a name="methods"></a><span data-ttu-id="0871d-111">Методы</span><span class="sxs-lookup"><span data-stu-id="0871d-111">Methods</span></span>
<span data-ttu-id="0871d-p104">Прямые запросы к этому ресурсу не поддерживаются. Сведения о том, как запрашивать записи службы доменов, см. в статье [о доменах](domain.md).</span><span class="sxs-lookup"><span data-stu-id="0871d-p104">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="0871d-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="0871d-114">Properties</span></span>
| <span data-ttu-id="0871d-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="0871d-115">Property</span></span>     | <span data-ttu-id="0871d-116">Тип</span><span class="sxs-lookup"><span data-stu-id="0871d-116">Type</span></span>   |<span data-ttu-id="0871d-117">Описание</span><span class="sxs-lookup"><span data-stu-id="0871d-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0871d-118">id</span><span class="sxs-lookup"><span data-stu-id="0871d-118">id</span></span>|<span data-ttu-id="0871d-119">Строка</span><span class="sxs-lookup"><span data-stu-id="0871d-119">String</span></span>| <span data-ttu-id="0871d-p105">Уникальный идентификатор, назначенный этому объекту. Не допускает значения null, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0871d-p105">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span>|
|<span data-ttu-id="0871d-122">isOptional</span><span class="sxs-lookup"><span data-stu-id="0871d-122">isOptional</span></span>|<span data-ttu-id="0871d-123">Логический</span><span class="sxs-lookup"><span data-stu-id="0871d-123">Boolean</span></span>| <span data-ttu-id="0871d-124">Если указано значение false, для правильной работы служб Microsoft Online Services с доменом клиент должен настроить эту запись на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="0871d-124">If false, this record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="0871d-125">label</span><span class="sxs-lookup"><span data-stu-id="0871d-125">label</span></span>|<span data-ttu-id="0871d-126">Строка</span><span class="sxs-lookup"><span data-stu-id="0871d-126">String</span></span>| <span data-ttu-id="0871d-127">Значение, используемое при настройке имени записи DNS на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="0871d-127">Value used when configuring the name of the DNS record at the DNS host.</span></span> |
|<span data-ttu-id="0871d-128">recordType</span><span class="sxs-lookup"><span data-stu-id="0871d-128">recordType</span></span>|<span data-ttu-id="0871d-129">Строка</span><span class="sxs-lookup"><span data-stu-id="0871d-129">String</span></span>| <span data-ttu-id="0871d-130">Указывает, какой тип записи DNS представляет этот объект.</span><span class="sxs-lookup"><span data-stu-id="0871d-130">Indicates what type of DNS record this entity represents.</span></span></br></br><span data-ttu-id="0871d-131">Возможные значения: *CName*, *Mx*, *Srv*, *Txt*.</span><span class="sxs-lookup"><span data-stu-id="0871d-131">The value can be one of the following: *CName*, *Mx*, *Srv*, *Txt*</span></span></br></br><span data-ttu-id="0871d-132">Ключ</span><span class="sxs-lookup"><span data-stu-id="0871d-132">Key</span></span> |
|<span data-ttu-id="0871d-133">supportedService</span><span class="sxs-lookup"><span data-stu-id="0871d-133">supportedService</span></span>|<span data-ttu-id="0871d-134">Строка</span><span class="sxs-lookup"><span data-stu-id="0871d-134">String</span></span>| <span data-ttu-id="0871d-135">Веб-служба или функция Майкрософт, зависящая от этой записи DNS.</span><span class="sxs-lookup"><span data-stu-id="0871d-135">Microsoft Online Service or feature that has a dependency on this DNS record.</span></span></br></br><span data-ttu-id="0871d-136">Возможные значения: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="0871d-136">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="0871d-137">ttl</span><span class="sxs-lookup"><span data-stu-id="0871d-137">ttl</span></span>|<span data-ttu-id="0871d-138">Int32</span><span class="sxs-lookup"><span data-stu-id="0871d-138">Int32</span></span>| <span data-ttu-id="0871d-p106">Значение, используемое при настройке свойства срока жизни (ttl) записи DNS на узле DNS. Не допускает значение null.</span><span class="sxs-lookup"><span data-stu-id="0871d-p106">Value to use when configuring the time-to-live (ttl) property of the DNS record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="0871d-141">Связи</span><span class="sxs-lookup"><span data-stu-id="0871d-141">Relationships</span></span>
<span data-ttu-id="0871d-142">Нет</span><span class="sxs-lookup"><span data-stu-id="0871d-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0871d-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0871d-143">JSON representation</span></span>
<span data-ttu-id="0871d-144">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0871d-144">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsRecord"
}-->

```json
{
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
  "description": "domainDnsRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
