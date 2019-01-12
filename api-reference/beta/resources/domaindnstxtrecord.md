---
title: Тип ресурса domainDnsTxtRecord
description: Представляет запись типа TXT, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от объекта DomainDnsRecord.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f0cb76e0c90a681eae775a687999a43b741a2df2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918130"
---
# <a name="domaindnstxtrecord-resource-type"></a><span data-ttu-id="78b3b-104">Тип ресурса domainDnsTxtRecord</span><span class="sxs-lookup"><span data-stu-id="78b3b-104">domainDnsTxtRecord resource type</span></span>

> <span data-ttu-id="78b3b-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="78b3b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="78b3b-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="78b3b-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="78b3b-p103">Представляет запись типа TXT, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от объекта [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="78b3b-p103">Represents a TXT record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="78b3b-109">Методы</span><span class="sxs-lookup"><span data-stu-id="78b3b-109">Methods</span></span>
<span data-ttu-id="78b3b-p104">Прямые запросы к этому ресурсу не поддерживаются. Сведения о том, как запрашивать записи службы доменов, см. в статье [о доменах](domain.md).</span><span class="sxs-lookup"><span data-stu-id="78b3b-p104">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="78b3b-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="78b3b-112">Properties</span></span>
| <span data-ttu-id="78b3b-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="78b3b-113">Property</span></span>     | <span data-ttu-id="78b3b-114">Тип</span><span class="sxs-lookup"><span data-stu-id="78b3b-114">Type</span></span>   |<span data-ttu-id="78b3b-115">Описание</span><span class="sxs-lookup"><span data-stu-id="78b3b-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="78b3b-116">id</span><span class="sxs-lookup"><span data-stu-id="78b3b-116">id</span></span>|<span data-ttu-id="78b3b-117">Строка</span><span class="sxs-lookup"><span data-stu-id="78b3b-117">String</span></span>| <span data-ttu-id="78b3b-p105">Уникальный идентификатор, назначенный этому объекту. Не допускает значения null, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="78b3b-p105">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span> |
|<span data-ttu-id="78b3b-120">isOptional</span><span class="sxs-lookup"><span data-stu-id="78b3b-120">isOptional</span></span>|<span data-ttu-id="78b3b-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="78b3b-121">Boolean</span></span>| <span data-ttu-id="78b3b-122">Если имеет значение false, пользователю необходимо настроить запись типа TXT на узле DNS, чтобы службы Microsoft Online Services правильно работали с доменом.</span><span class="sxs-lookup"><span data-stu-id="78b3b-122">If false, the TXT record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="78b3b-123">label</span><span class="sxs-lookup"><span data-stu-id="78b3b-123">label</span></span>|<span data-ttu-id="78b3b-124">String</span><span class="sxs-lookup"><span data-stu-id="78b3b-124">String</span></span>| <span data-ttu-id="78b3b-125">Значение, используемое при настройке свойства *name* для записи типа TXT на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="78b3b-125">Value to use when configuring the *name* property of the TXT record at the DNS host.</span></span>|
|<span data-ttu-id="78b3b-126">recordType</span><span class="sxs-lookup"><span data-stu-id="78b3b-126">recordType</span></span>|<span data-ttu-id="78b3b-127">String</span><span class="sxs-lookup"><span data-stu-id="78b3b-127">String</span></span>| <span data-ttu-id="78b3b-p106">Тип записи DNS. Это свойство всегда имеет значение *Txt*. Ключ.</span><span class="sxs-lookup"><span data-stu-id="78b3b-p106">Type of DNS record. The value is always *Txt*. Key</span></span> |
|<span data-ttu-id="78b3b-131">supportedService</span><span class="sxs-lookup"><span data-stu-id="78b3b-131">supportedService</span></span>|<span data-ttu-id="78b3b-132">String</span><span class="sxs-lookup"><span data-stu-id="78b3b-132">String</span></span>| <span data-ttu-id="78b3b-133">Служба или компонент Microsoft Online Services, зависящие от этой записи типа TXT.</span><span class="sxs-lookup"><span data-stu-id="78b3b-133">Microsoft Online Service or feature that has a dependency on this TXT record.</span></span></br></br><span data-ttu-id="78b3b-134">Возможные значения: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*.</span><span class="sxs-lookup"><span data-stu-id="78b3b-134">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="78b3b-135">text</span><span class="sxs-lookup"><span data-stu-id="78b3b-135">text</span></span>|<span data-ttu-id="78b3b-136">String</span><span class="sxs-lookup"><span data-stu-id="78b3b-136">String</span></span>| <span data-ttu-id="78b3b-137">Значение, используемое при настройке свойства *text* на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="78b3b-137">Value used when configuring the *text* property at the DNS host.</span></span> |
|<span data-ttu-id="78b3b-138">ttl</span><span class="sxs-lookup"><span data-stu-id="78b3b-138">ttl</span></span>|<span data-ttu-id="78b3b-139">Int32</span><span class="sxs-lookup"><span data-stu-id="78b3b-139">Int32</span></span>| <span data-ttu-id="78b3b-p107">Значение, используемое при настройке свойства *ttl* (срока жизни) для записи MX на узле DNS. Не допускает значения null.</span><span class="sxs-lookup"><span data-stu-id="78b3b-p107">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="78b3b-142">Связи</span><span class="sxs-lookup"><span data-stu-id="78b3b-142">Relationships</span></span>
<span data-ttu-id="78b3b-143">Нет</span><span class="sxs-lookup"><span data-stu-id="78b3b-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="78b3b-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="78b3b-144">JSON representation</span></span>
<span data-ttu-id="78b3b-145">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="78b3b-145">Here is a JSON representation of the resource.</span></span>

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
