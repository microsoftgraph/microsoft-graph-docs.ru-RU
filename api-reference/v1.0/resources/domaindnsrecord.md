---
title: Тип ресурса domainDnsRecord
description: Объект DomainDnsRecord используется для представить записи DNS.
localization_priority: Normal
author: adimitui
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: ba4955c670548b3670dc90a574bc1b4fd8a11c58
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135109"
---
# <a name="domaindnsrecord-resource-type"></a>Тип ресурса domainDnsRecord

Пространство имен: microsoft.graph

Для каждого домена в клиенте может потребоваться добавить записи DNS в DNS-файл зоны домена, прежде чем домен сможет использоваться Microsoft Online Services. Объект **DomainDnsRecord используется** для представить такие записи DNS. Базовый объект для сущностей [DomainDnsCnameRecord,](domaindnscnamerecord.md) [DomainDnsMxRecord,](domaindnsmxrecord.md) [DomainDnsSrvRecord](domaindnssrvrecord.md) и [DomainDnsTxtRecord.](domaindnstxtrecord.md)

## <a name="methods"></a>Methods
Прямые запросы к этому ресурсу не поддерживаются. Сведения о [том,](domain.md) как запрашивать записи доменной службы, см. в разделе "Домен".

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String| Уникальный идентификатор, присвоенный этой сущности. Не имеет null, только для чтения.|
|isOptional|Boolean| Если установлено false, эта запись должна быть настроена клиентом на DNS-Microsoft Online Services для правильной работы с доменом. |
|label|String| Значение, используемого при настройке имени DNS-записи на DNS-хосте. |
|recordType|String| Указывает, какой тип DNS-записи представляет этот объект.</br></br>Может иметь одно из следующих значений: *CName,* *Mx,* *Srv,* *Txt*</br></br>Key |
|supportedService|String| Microsoft Online Service или функция, которая зависит от этой записи DNS.</br></br>Может иметь одно из следующих значений: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*|
|ttl|Int32| Значение, используемого при настройке свойства времени жизни (ttl) записи DNS на DNS-хосте. Не nullable |

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
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

