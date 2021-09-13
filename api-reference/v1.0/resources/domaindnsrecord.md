---
title: тип ресурса domainDnsRecord
description: Объект DomainDnsRecord используется для вручия записей DNS.
ms.localizationpriority: medium
author: adimitui
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: fdd8dd884b19803aede0109a9c5c95bb3abe8585
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59123798"
---
# <a name="domaindnsrecord-resource-type"></a>тип ресурса domainDnsRecord

Пространство имен: microsoft.graph

Для каждого домена в клиенте может потребоваться добавить запись DNS в файл зоны DNS домена, прежде чем домен может использоваться Microsoft Online Services. Объект **DomainDnsRecord** используется для вручия таких DNS-записей. Базовый объект для сущностей [DomainDnsCnameRecord,](domaindnscnamerecord.md) [DomainDnsMxRecord,](domaindnsmxrecord.md) [DomainDnsSrvRecord](domaindnssrvrecord.md) и [DomainDnsTxtRecord.](domaindnstxtrecord.md)

## <a name="methods"></a>Методы
Прямые запросы на этот ресурс не поддерживаются. Сведения о [том,](domain.md) как запрашивать записи службы домена, см. в разделе домен.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String| Уникальный идентификатор, присвоенный этому объекту. Не является недействительным, только для чтения.|
|isOptional|Логический| Если эта запись является ложной, она должна быть настроена клиентом на хост DNS, чтобы Microsoft Online Services правильно работать с доменом. |
|подпись|Строка| Значение, используемого при настройке имени записи DNS в хосте DNS. |
|recordType|String| Указывает, какой тип записи DNS представляет этот объект.</br></br>Значение может быть одним из следующих: *CName*, *Mx*, *Srv*, *Txt*</br></br>Key |
|supportedService|String| Microsoft Online Service или функция, зависимая от этой записи DNS.</br></br>Может быть одним из следующих значений: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*|
|ttl|Int32| Значение, используемого при настройке свойства "время на жизнь" записи DNS в хосте DNS. Не является недействительным |

## <a name="relationships"></a>Отношения
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

