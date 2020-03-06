---
title: Тип ресурса Домаинднсткстрекорд
description: Представляет запись TXT, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от объекта DomainDnsRecord.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6a2899081dcc171feb2ae937ae1a742093c5133f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531590"
---
# <a name="domaindnstxtrecord-resource-type"></a>Тип ресурса Домаинднсткстрекорд

Пространство имен: microsoft.graph

Представляет запись TXT, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от объекта [DomainDnsRecord](domaindnsrecord.md) .

## <a name="methods"></a>Методы
Прямые запросы к этому ресурсу не поддерживаются. Сведения о том, как запросить записи службы домена, можно найти в разделе [domain](domain.md) .

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|Строка| Уникальный идентификатор, назначенный этой сущности. Не допускает значения NULL и только для чтения. |
|Переключатель|Boolean| Если этот параметр имеет значение false, запись TXT должна быть настроена клиентом на узле DNS для правильной работы Microsoft Online Services с доменом. |
|label|Строка| Значение, используемое при настройке свойства *Name* записи TXT на узле DNS.|
|recordType|Строка| Тип записи DNS. Значение всегда является *txt*. Key |
|суппортедсервице|Строка| Служба или компонент Microsoft Online, зависящие от этой записи TXT.</br></br>Может принимать одно из следующих значений: **null**, *Email*, *SharePoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune* |
|текст|Строка| Значение, используемое при настройке свойства *Text* на узле DNS. |
|используем|Int32| Значение, используемое при настройке свойства срока *жизни (TTL)* записи MX на узле DNS. Не допускает значение null |

## <a name="relationships"></a>Связи
Нет


## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsTxtRecord"
}-->

```json
{
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
