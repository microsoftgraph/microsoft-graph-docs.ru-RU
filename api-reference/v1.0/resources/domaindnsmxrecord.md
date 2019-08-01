---
title: Тип ресурса Домаинднсмксрекорд
description: Представляет запись MX, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от объекта DomainDnsRecord.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1d837ce660ebceda300d63d428b92836b3173fba
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032664"
---
# <a name="domaindnsmxrecord-resource-type"></a>Тип ресурса Домаинднсмксрекорд

Представляет запись MX, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от объекта [DomainDnsRecord](domaindnsrecord.md) .

## <a name="methods"></a>Методы
Прямые запросы к этому ресурсу не поддерживаются. Сведения о том, как запросить записи службы домена, можно найти в разделе [domain](domain.md) .

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String| Уникальный идентификатор, назначенный этой сущности. Не допускает значения NULL и только для чтения.|
|Переключатель|Boolean| Если задано значение false, запись MX должна быть настроена клиентом на узле DNS для правильной работы Microsoft Online Services с доменом. |
|label|String| Значение, используемое при настройке свойства *Alias/Host/Name* для записи MX на узле DNS. |
|Маилексчанже|String| Значение, используемое при настройке *ответа/назначения/значения* для записи MX на узле DNS.|
|параметров|Int32| Значение, используемое при настройке свойства *предпочтения/приоритета* записи MX на узле DNS. |
|recordType|String| Тип записи DNS. Значение — это всегда *MX*. Key |
|Суппортедсервице|String| Служба или компонент Microsoft Online, который имеет зависимость от этой записи MX.</br></br>Может принимать одно из следующих значений: **null**, *Email*, *SharePoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic *, *OrgIdAuthentication*, *Yammer*, *Intune* |
|используем|Int32| Значение, используемое при настройке свойства срока *жизни (TTL)* записи MX на узле DNS. Не допускает значение null |

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsMxRecord"
}-->

```json
{
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
