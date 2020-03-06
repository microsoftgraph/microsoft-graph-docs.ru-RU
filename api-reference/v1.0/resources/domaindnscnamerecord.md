---
title: Тип ресурса Домаинднскнамерекорд
description: Представляет запись CNAME, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от объекта DomainDnsRecord.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 938a11bc1cc7790e2e521c86a51b258882dfad86
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531617"
---
# <a name="domaindnscnamerecord-resource-type"></a>Тип ресурса Домаинднскнамерекорд

Пространство имен: microsoft.graph

Представляет запись CNAME, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от объекта [DomainDnsRecord](domaindnsrecord.md) .


## <a name="methods"></a>Методы
Прямые запросы к этому ресурсу не поддерживаются. Сведения о том, как запросить записи службы домена, можно найти в разделе [domain](domain.md) .

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|каноникалнаме|Строка| Каноническое имя записи CNAME. Используется для настройки записи CNAME на узле DNS. |
|id|Строка| Уникальный идентификатор, назначенный этой сущности. Не допускает значение null, доступно только для чтения|
|Переключатель|Boolean| Если значение равно false, запись CNAME должна быть настроена клиентом на узле DNS для правильной работы Microsoft Online Services с доменом. Не допускает значение null |
|label|Строка| Значение, используемое при настройке *псевдонима/узла или имени* записи CNAME на узле DNS. |
|recordType|Строка| Тип записи DNS. Значение всегда равно *CNAME*. Key|
|суппортедсервице|Строка| Служба или компонент Microsoft Online, который имеет зависимость от этой записи CNAME.</br></br>Может принимать одно из следующих значений: **null**, *Email*, *SharePoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*|
|используем|Int32| Значение, используемое при настройке свойства срока жизни (TTL) записи CNAME на узле DNS. Не допускает значение null |

## <a name="relationships"></a>Связи
Нет


## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

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
