---
title: Тип ресурса Домаинднссрврекорд
description: Представляет запись SRV, добавленную в файл зоны DNS определенного домена в клиенте.
author: adimitui
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6854b30dec759726fefaf93e13ad23a49195e381
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48010341"
---
# <a name="domaindnssrvrecord-resource-type"></a>Тип ресурса Домаинднссрврекорд

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет запись SRV, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от объекта [DomainDnsRecord](domaindnsrecord.md) .

## <a name="methods"></a>Методы
Прямые запросы к этому ресурсу не поддерживаются. Сведения о том, как запросить записи службы домена, можно найти в разделе [domain](domain.md) .

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String| Уникальный идентификатор, назначенный этой сущности. Не допускает значения NULL и только для чтения.|
|Переключатель|Boolean| Если задано значение false, запись SRV должна быть настроена клиентом на узле DNS для правильной работы Microsoft Online Services с доменом. |
|label|String| Значение, используемое при настройке свойства *Name* записи SRV на узле DNS. |
|наметаржет|String| Значение, используемое при настройке свойства *Target* записи SRV на узле DNS. |
|порта|Int32| Значение, используемое при настройке свойства *Port* записи SRV на узле DNS. |
|priority|Int32| Значение, используемое при настройке свойства *Priority* записи SRV на узле DNS. |
|Protocol|String| Значение, используемое при настройке свойства *Protocol* записи SRV на узле DNS. |
|recordType|String|  Тип записи DNS. Значение — всегда *SRV*. Key |
|service|String| Значение, используемое при настройке свойства *Service* для записи SRV на узле DNS. |
|суппортедсервице|String| Служба или компонент Microsoft Online, который имеет зависимость от этой записи SRV.</br></br>Может принимать одно из следующих значений: **null**, *Email*, *SharePoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune* |
|используем|Int32| Значение, используемое при настройке свойства срока *жизни (TTL)* записи SRV на узле DNS. Не допускает значение null |
|weight|Int32| Значение, используемое при настройке свойства *Weight* записи SRV на узле DNS. |

## <a name="relationships"></a>Отношения
Нет


## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsSrvRecord"
}-->

```json
{
  "canonicalName": "String",
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "nameTarget": "String",
  "port": 1024,
  "priority": 1024,
  "protocol": "String",
  "recordType": "String",
  "service": "String",
  "supportedService": "String",
  "ttl": 1024,
  "weight": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "domainDnsSrvRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


