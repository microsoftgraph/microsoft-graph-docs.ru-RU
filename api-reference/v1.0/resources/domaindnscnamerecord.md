---
title: Тип ресурса domainDnsCnameRecord
description: Представляет запись CNAME, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от объекта DomainDnsRecord.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 226f067756517771b1d86f053d48268b905dd930
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990497"
---
# <a name="domaindnscnamerecord-resource-type"></a>Тип ресурса domainDnsCnameRecord

Представляет запись CNAME, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от объекта [DomainDnsRecord](domaindnsrecord.md).


## <a name="methods"></a>Методы
Прямые запросы к этому ресурсу не поддерживаются. Сведения о том, как запрашивать записи службы доменов, см. в статье [о доменах](domain.md).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|canonicalName|String| Каноническое имя записи CNAME. Используется для настройки записи CNAME в узле DNS. |
|id|String| Уникальный идентификатор, назначенный этому объекту. Не допускает значения null, только для чтения.|
|isOptional|Boolean| Если имеет значение false, пользователю необходимо настроить запись CNAME на узле DNS, чтобы службы Microsoft Online Services правильно работали с доменом. Не допускает значения null. |
|label|String| Значение, используемое при настройке *псевдонима, узла и имени* для записи CNAME на узле DNS. |
|recordType|String| Тип записи DNS. Это свойство всегда имеет значение *CName*. Ключевое.|
|supportedService|String| Служба или функция Microsoft Online, имеющая зависимость от этой записи CNAME.</br></br>Может иметь одно из следующих значений: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer* или *Intune*.|
|ttl|Int32| Значение, используемое при настройке свойства срока жизни (ttl) записи CNAME на узле DNS. Не допускает значения null. |

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
