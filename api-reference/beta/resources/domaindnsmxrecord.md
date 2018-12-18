---
title: Тип ресурса domainDnsMxRecord
description: Представляет запись MX, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от объекта DomainDnsRecord.
author: lleonard-msft
ms.openlocfilehash: 562afbd6998ad1678f4f055dacf89af9b1ed4446
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320652"
---
# <a name="domaindnsmxrecord-resource-type"></a><span data-ttu-id="60bbf-104">Тип ресурса domainDnsMxRecord</span><span class="sxs-lookup"><span data-stu-id="60bbf-104">domainDnsMxRecord resource type</span></span>

> <span data-ttu-id="60bbf-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="60bbf-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="60bbf-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60bbf-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="60bbf-p103">Представляет запись MX, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от объекта [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="60bbf-p103">Represents a MX record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="60bbf-109">Методы</span><span class="sxs-lookup"><span data-stu-id="60bbf-109">Methods</span></span>
<span data-ttu-id="60bbf-p104">Прямые запросы к этому ресурсу не поддерживаются. Сведения о том, как запрашивать записи службы доменов, см. в статье [о доменах](domain.md).</span><span class="sxs-lookup"><span data-stu-id="60bbf-p104">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="60bbf-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="60bbf-112">Properties</span></span>
| <span data-ttu-id="60bbf-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="60bbf-113">Property</span></span>     | <span data-ttu-id="60bbf-114">Тип</span><span class="sxs-lookup"><span data-stu-id="60bbf-114">Type</span></span>   |<span data-ttu-id="60bbf-115">Описание</span><span class="sxs-lookup"><span data-stu-id="60bbf-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="60bbf-116">id</span><span class="sxs-lookup"><span data-stu-id="60bbf-116">id</span></span>|<span data-ttu-id="60bbf-117">Строка</span><span class="sxs-lookup"><span data-stu-id="60bbf-117">String</span></span>| <span data-ttu-id="60bbf-p105">Уникальный идентификатор, назначенный этому объекту. Не допускает значения null, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="60bbf-p105">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span>|
|<span data-ttu-id="60bbf-120">isOptional</span><span class="sxs-lookup"><span data-stu-id="60bbf-120">isOptional</span></span>|<span data-ttu-id="60bbf-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="60bbf-121">Boolean</span></span>| <span data-ttu-id="60bbf-122">Если указано значение false, для правильной работы Microsoft Online Services с доменом пользователь должен настроить запись MX на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="60bbf-122">If false, the MX record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="60bbf-123">label</span><span class="sxs-lookup"><span data-stu-id="60bbf-123">label</span></span>|<span data-ttu-id="60bbf-124">String</span><span class="sxs-lookup"><span data-stu-id="60bbf-124">String</span></span>| <span data-ttu-id="60bbf-125">Значение, используемое при настройке свойства *псевдонима, узла или имени* для записи MX на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="60bbf-125">Value used when configuring the *alias/host/name* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="60bbf-126">mailExchange</span><span class="sxs-lookup"><span data-stu-id="60bbf-126">mailExchange</span></span>|<span data-ttu-id="60bbf-127">String</span><span class="sxs-lookup"><span data-stu-id="60bbf-127">String</span></span>| <span data-ttu-id="60bbf-128">Значение, используемое при настройке *значения, ответа или целевого объекта* для записи MX на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="60bbf-128">Value used when configuring the *answer/destination/value* of the MX record at the DNS host.</span></span>|
|<span data-ttu-id="60bbf-129">preference</span><span class="sxs-lookup"><span data-stu-id="60bbf-129">preference</span></span>|<span data-ttu-id="60bbf-130">Int32</span><span class="sxs-lookup"><span data-stu-id="60bbf-130">Int32</span></span>| <span data-ttu-id="60bbf-131">Значение, используемое при настройке свойства *приоритета или предпочтения* для записи MX на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="60bbf-131">Value used when configuring the *Preference/Priority* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="60bbf-132">recordType</span><span class="sxs-lookup"><span data-stu-id="60bbf-132">recordType</span></span>|<span data-ttu-id="60bbf-133">String</span><span class="sxs-lookup"><span data-stu-id="60bbf-133">String</span></span>| <span data-ttu-id="60bbf-p106">Тип записи DNS. Это свойство всегда имеет значение *Mx*. Ключ.</span><span class="sxs-lookup"><span data-stu-id="60bbf-p106">Type of DNS record. The value is always *Mx*. Key</span></span> |
|<span data-ttu-id="60bbf-137">supportedService</span><span class="sxs-lookup"><span data-stu-id="60bbf-137">supportedService</span></span>|<span data-ttu-id="60bbf-138">String</span><span class="sxs-lookup"><span data-stu-id="60bbf-138">String</span></span>| <span data-ttu-id="60bbf-139">Служба или компонент Microsoft Online Services, зависящие от этой записи типа MX.</span><span class="sxs-lookup"><span data-stu-id="60bbf-139">Microsoft Online Service or feature that has a dependency on this MX record.</span></span></br></br><span data-ttu-id="60bbf-140">Возможные значения: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*.</span><span class="sxs-lookup"><span data-stu-id="60bbf-140">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="60bbf-141">ttl</span><span class="sxs-lookup"><span data-stu-id="60bbf-141">ttl</span></span>|<span data-ttu-id="60bbf-142">Int32</span><span class="sxs-lookup"><span data-stu-id="60bbf-142">Int32</span></span>| <span data-ttu-id="60bbf-p107">Значение, используемое при настройке свойства *ttl* (срока жизни) для записи MX на узле DNS. Не допускает значения null.</span><span class="sxs-lookup"><span data-stu-id="60bbf-p107">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="60bbf-145">Связи</span><span class="sxs-lookup"><span data-stu-id="60bbf-145">Relationships</span></span>
<span data-ttu-id="60bbf-146">Нет</span><span class="sxs-lookup"><span data-stu-id="60bbf-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="60bbf-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="60bbf-147">JSON representation</span></span>
<span data-ttu-id="60bbf-148">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="60bbf-148">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsMxRecord"
}-->

```json
{
  "canonicalName": "String",
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