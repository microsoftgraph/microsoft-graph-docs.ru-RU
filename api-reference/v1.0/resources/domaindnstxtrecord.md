---
title: тип ресурса domainDnsTxtRecord
description: Представляет запись TXT, добавленную в файл зоны DNS определенного домена в клиенте.
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: d30821011aacc0ed0b7643237b745d2f0bec962d4fad53f1f195de2224021890
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54202443"
---
# <a name="domaindnstxtrecord-resource-type"></a>тип ресурса domainDnsTxtRecord

Пространство имен: microsoft.graph

Представляет запись TXT, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от [объекта DomainDnsRecord.](domaindnsrecord.md)

## <a name="methods"></a>Методы
Прямые запросы на этот ресурс не поддерживаются. Сведения о [том,](domain.md) как запрашивать записи службы домена, см. в разделе домен.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String| Уникальный идентификатор, присвоенный этому объекту. Не является недействительным, только для чтения. |
|isOptional|Логический| Если это неверно, запись TXT должна быть настроена клиентом на хост DNS, чтобы Microsoft Online Services правильно работать с доменом. |
|label|String| Значение, которое необходимо  использовать при настройке свойства имени записи TXT в хосте DNS.|
|recordType|String| Тип записи DNS. Значение всегда *Txt*. Key |
|supportedService|String| Microsoft Online Service или функция, зависимая от этой записи TXT.</br></br>Может быть одним из следующих значений: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune* |
|текст|String| Значение, используемее при настройке *свойства текста* в хосте DNS. |
|ttl|Int32| Значение, используемого при настройке свойства времени для жизни *(ttl)* записи MX в хосте DNS. Не является недействительным |

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

