---
title: Тип ресурса domainDnsCnameRecord
description: Представляет запись CNAME, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от объекта DomainDnsRecord.
author: lleonard-msft
ms.openlocfilehash: 0ce5a748d9a1b558b4ac49e104eb9498efe674aa
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315843"
---
# <a name="domaindnscnamerecord-resource-type"></a><span data-ttu-id="3de8a-104">Тип ресурса domainDnsCnameRecord</span><span class="sxs-lookup"><span data-stu-id="3de8a-104">domainDnsCnameRecord resource type</span></span>

> <span data-ttu-id="3de8a-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3de8a-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3de8a-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3de8a-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3de8a-p103">Представляет запись CNAME, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от объекта [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="3de8a-p103">Represents a CNAME record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>


## <a name="methods"></a><span data-ttu-id="3de8a-109">Методы</span><span class="sxs-lookup"><span data-stu-id="3de8a-109">Methods</span></span>
<span data-ttu-id="3de8a-p104">Прямые запросы к этому ресурсу не поддерживаются. Сведения о том, как запрашивать записи службы доменов, см. в статье [о доменах](domain.md).</span><span class="sxs-lookup"><span data-stu-id="3de8a-p104">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="3de8a-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="3de8a-112">Properties</span></span>
| <span data-ttu-id="3de8a-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="3de8a-113">Property</span></span>     | <span data-ttu-id="3de8a-114">Тип</span><span class="sxs-lookup"><span data-stu-id="3de8a-114">Type</span></span>   |<span data-ttu-id="3de8a-115">Описание</span><span class="sxs-lookup"><span data-stu-id="3de8a-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3de8a-116">canonicalName</span><span class="sxs-lookup"><span data-stu-id="3de8a-116">canonicalName</span></span>|<span data-ttu-id="3de8a-117">String</span><span class="sxs-lookup"><span data-stu-id="3de8a-117">String</span></span>| <span data-ttu-id="3de8a-p105">Каноническое имя записи CNAME. Используется для настройки записи CNAME в узле DNS.</span><span class="sxs-lookup"><span data-stu-id="3de8a-p105">The canonical name of the CNAME record. Used to configure the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="3de8a-120">id</span><span class="sxs-lookup"><span data-stu-id="3de8a-120">id</span></span>|<span data-ttu-id="3de8a-121">String</span><span class="sxs-lookup"><span data-stu-id="3de8a-121">String</span></span>| <span data-ttu-id="3de8a-p106">Уникальный идентификатор, назначенный этому объекту. Не допускает значения null, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3de8a-p106">Unique identifier assigned to this entity. Not nullable, Read-only</span></span>|
|<span data-ttu-id="3de8a-124">isOptional</span><span class="sxs-lookup"><span data-stu-id="3de8a-124">isOptional</span></span>|<span data-ttu-id="3de8a-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="3de8a-125">Boolean</span></span>| <span data-ttu-id="3de8a-p107">Если имеет значение false, пользователю необходимо настроить запись CNAME на узле DNS, чтобы службы Microsoft Online Services правильно работали с доменом. Не допускает значения null.</span><span class="sxs-lookup"><span data-stu-id="3de8a-p107">If false, the CNAME record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain. Not nullable</span></span> |
|<span data-ttu-id="3de8a-128">label</span><span class="sxs-lookup"><span data-stu-id="3de8a-128">label</span></span>|<span data-ttu-id="3de8a-129">String</span><span class="sxs-lookup"><span data-stu-id="3de8a-129">String</span></span>| <span data-ttu-id="3de8a-130">Значение, используемое при настройке *псевдонима, узла и имени* для записи CNAME на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="3de8a-130">Value used when configuring the *alias/host/name* of the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="3de8a-131">recordType</span><span class="sxs-lookup"><span data-stu-id="3de8a-131">recordType</span></span>|<span data-ttu-id="3de8a-132">String</span><span class="sxs-lookup"><span data-stu-id="3de8a-132">String</span></span>| <span data-ttu-id="3de8a-p108">Тип записи DNS. Это свойство всегда имеет значение *CName*. Ключевое.</span><span class="sxs-lookup"><span data-stu-id="3de8a-p108">Type of DNS record. The value is always *CName*. Key</span></span>|
|<span data-ttu-id="3de8a-136">supportedService</span><span class="sxs-lookup"><span data-stu-id="3de8a-136">supportedService</span></span>|<span data-ttu-id="3de8a-137">String</span><span class="sxs-lookup"><span data-stu-id="3de8a-137">String</span></span>| <span data-ttu-id="3de8a-138">Служба или функция Microsoft Online, имеющая зависимость от этой записи CNAME.</span><span class="sxs-lookup"><span data-stu-id="3de8a-138">Microsoft Online Service or feature that has a dependency on this CNAME record.</span></span></br></br><span data-ttu-id="3de8a-139">Может иметь одно из следующих значений: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer* или *Intune*.</span><span class="sxs-lookup"><span data-stu-id="3de8a-139">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="3de8a-140">ttl</span><span class="sxs-lookup"><span data-stu-id="3de8a-140">ttl</span></span>|<span data-ttu-id="3de8a-141">Int32</span><span class="sxs-lookup"><span data-stu-id="3de8a-141">Int32</span></span>| <span data-ttu-id="3de8a-p109">Значение, используемое при настройке свойства срока жизни (ttl) записи CNAME на узле DNS. Не допускает значения null.</span><span class="sxs-lookup"><span data-stu-id="3de8a-p109">Value to use when configuring the time-to-live (ttl) property of the CNAME record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="3de8a-144">Связи</span><span class="sxs-lookup"><span data-stu-id="3de8a-144">Relationships</span></span>
<span data-ttu-id="3de8a-145">Нет</span><span class="sxs-lookup"><span data-stu-id="3de8a-145">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="3de8a-146">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3de8a-146">JSON representation</span></span>
<span data-ttu-id="3de8a-147">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3de8a-147">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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