---
title: Тип ресурса domainDnsMxRecord
description: Представляет запись MX, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от объекта DomainDnsRecord.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 90744a9a800fd3a330b9df41299e335c5852446a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923511"
---
# <a name="domaindnsmxrecord-resource-type"></a><span data-ttu-id="ef50e-104">Тип ресурса domainDnsMxRecord</span><span class="sxs-lookup"><span data-stu-id="ef50e-104">domainDnsMxRecord resource type</span></span>

> <span data-ttu-id="ef50e-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ef50e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ef50e-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef50e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ef50e-p103">Представляет запись MX, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от объекта [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="ef50e-p103">Represents a MX record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="ef50e-109">Методы</span><span class="sxs-lookup"><span data-stu-id="ef50e-109">Methods</span></span>
<span data-ttu-id="ef50e-p104">Прямые запросы к этому ресурсу не поддерживаются. Сведения о том, как запрашивать записи службы доменов, см. в статье [о доменах](domain.md).</span><span class="sxs-lookup"><span data-stu-id="ef50e-p104">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="ef50e-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="ef50e-112">Properties</span></span>
| <span data-ttu-id="ef50e-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="ef50e-113">Property</span></span>     | <span data-ttu-id="ef50e-114">Тип</span><span class="sxs-lookup"><span data-stu-id="ef50e-114">Type</span></span>   |<span data-ttu-id="ef50e-115">Описание</span><span class="sxs-lookup"><span data-stu-id="ef50e-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ef50e-116">id</span><span class="sxs-lookup"><span data-stu-id="ef50e-116">id</span></span>|<span data-ttu-id="ef50e-117">Строка</span><span class="sxs-lookup"><span data-stu-id="ef50e-117">String</span></span>| <span data-ttu-id="ef50e-p105">Уникальный идентификатор, назначенный этому объекту. Не допускает значения null, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ef50e-p105">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span>|
|<span data-ttu-id="ef50e-120">isOptional</span><span class="sxs-lookup"><span data-stu-id="ef50e-120">isOptional</span></span>|<span data-ttu-id="ef50e-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef50e-121">Boolean</span></span>| <span data-ttu-id="ef50e-122">Если указано значение false, для правильной работы Microsoft Online Services с доменом пользователь должен настроить запись MX на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="ef50e-122">If false, the MX record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="ef50e-123">label</span><span class="sxs-lookup"><span data-stu-id="ef50e-123">label</span></span>|<span data-ttu-id="ef50e-124">String</span><span class="sxs-lookup"><span data-stu-id="ef50e-124">String</span></span>| <span data-ttu-id="ef50e-125">Значение, используемое при настройке свойства *псевдонима, узла или имени* для записи MX на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="ef50e-125">Value used when configuring the *alias/host/name* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="ef50e-126">mailExchange</span><span class="sxs-lookup"><span data-stu-id="ef50e-126">mailExchange</span></span>|<span data-ttu-id="ef50e-127">String</span><span class="sxs-lookup"><span data-stu-id="ef50e-127">String</span></span>| <span data-ttu-id="ef50e-128">Значение, используемое при настройке *значения, ответа или целевого объекта* для записи MX на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="ef50e-128">Value used when configuring the *answer/destination/value* of the MX record at the DNS host.</span></span>|
|<span data-ttu-id="ef50e-129">preference</span><span class="sxs-lookup"><span data-stu-id="ef50e-129">preference</span></span>|<span data-ttu-id="ef50e-130">Int32</span><span class="sxs-lookup"><span data-stu-id="ef50e-130">Int32</span></span>| <span data-ttu-id="ef50e-131">Значение, используемое при настройке свойства *приоритета или предпочтения* для записи MX на узле DNS.</span><span class="sxs-lookup"><span data-stu-id="ef50e-131">Value used when configuring the *Preference/Priority* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="ef50e-132">recordType</span><span class="sxs-lookup"><span data-stu-id="ef50e-132">recordType</span></span>|<span data-ttu-id="ef50e-133">String</span><span class="sxs-lookup"><span data-stu-id="ef50e-133">String</span></span>| <span data-ttu-id="ef50e-p106">Тип записи DNS. Это свойство всегда имеет значение *Mx*. Ключ.</span><span class="sxs-lookup"><span data-stu-id="ef50e-p106">Type of DNS record. The value is always *Mx*. Key</span></span> |
|<span data-ttu-id="ef50e-137">supportedService</span><span class="sxs-lookup"><span data-stu-id="ef50e-137">supportedService</span></span>|<span data-ttu-id="ef50e-138">String</span><span class="sxs-lookup"><span data-stu-id="ef50e-138">String</span></span>| <span data-ttu-id="ef50e-139">Служба или компонент Microsoft Online Services, зависящие от этой записи типа MX.</span><span class="sxs-lookup"><span data-stu-id="ef50e-139">Microsoft Online Service or feature that has a dependency on this MX record.</span></span></br></br><span data-ttu-id="ef50e-140">Возможные значения: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*.</span><span class="sxs-lookup"><span data-stu-id="ef50e-140">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="ef50e-141">ttl</span><span class="sxs-lookup"><span data-stu-id="ef50e-141">ttl</span></span>|<span data-ttu-id="ef50e-142">Int32</span><span class="sxs-lookup"><span data-stu-id="ef50e-142">Int32</span></span>| <span data-ttu-id="ef50e-p107">Значение, используемое при настройке свойства *ttl* (срока жизни) для записи MX на узле DNS. Не допускает значения null.</span><span class="sxs-lookup"><span data-stu-id="ef50e-p107">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="ef50e-145">Связи</span><span class="sxs-lookup"><span data-stu-id="ef50e-145">Relationships</span></span>
<span data-ttu-id="ef50e-146">Нет</span><span class="sxs-lookup"><span data-stu-id="ef50e-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ef50e-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ef50e-147">JSON representation</span></span>
<span data-ttu-id="ef50e-148">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ef50e-148">Here is a JSON representation of the resource.</span></span>

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
