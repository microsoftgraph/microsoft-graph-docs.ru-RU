---
title: Тип ресурса Домаинднскнамерекорд
description: Представляет запись CNAME, добавленную в файл зоны DNS определенного домена в клиенте. НаСледуется от объекта DomainDnsRecord.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f270075556843625d1ec408f06be8ed4a065c831
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543202"
---
# <a name="domaindnscnamerecord-resource-type"></a>Тип ресурса Домаинднскнамерекорд

Представляет запись CNAME, добавленную в файл зоны DNS определенного домена в клиенте. НаСледуется от объекта [DomainDnsRecord](domaindnsrecord.md) .


## <a name="methods"></a>Методы
Прямые запросы к этому ресурсу не поддерживаются. Сведения о том, как запросить записи службы домена, можно найти в разделе [domain](domain.md) .

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|Каноникалнаме|String| Каноническое имя записи CNAME. Используется для настройки записи CNAME на узле DNS. |
|id|String| Уникальный идентификатор, назначенный этой сущности. Не допускает значение null, доступно только для чтения|
|Переключатель|Логический| Если значение равно false, запись CNAME должна быть настроена клиентом на узле DNS для правильной работы Microsoft Online Services с доменом. Не допускает значение null |
|label|String| Значение, используемое при настройке *псевдонима/узла или имени* записи CNAME на узле DNS. |
|recordType|String| Тип записи DNS. Значение всегда равно *CNAME*. Ключ|
|Суппортедсервице|String| Служба или компонент Microsoft Online, который имеет зависимость от этой записи CNAME.</br></br>Может принимать одно из следующих значений: **null**, *Email*, *SharePoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic *, *OrgIdAuthentication*, *Yammer*, *Intune*|
|используем|Int32| Значение, используемое при настройке свойства срока жизни (TTL) записи CNAME на узле DNS. Не допускает значение null |

## <a name="relationships"></a>Отношения
Нет


## <a name="json-representation"></a>Представление в формате JSON
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
