---
title: тип ресурса domainDnsMxRecord
description: Представляет запись MX, добавленную в файл зоны DNS определенного домена в клиенте.
author: adimitui
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 41f09764ab4fe2cfde183908db35c99965cce087
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59056111"
---
# <a name="domaindnsmxrecord-resource-type"></a>тип ресурса domainDnsMxRecord

Пространство имен: microsoft.graph

Представляет запись MX, добавленную в файл зоны DNS определенного домена в клиенте. Наследуется от [объекта DomainDnsRecord.](domaindnsrecord.md)

## <a name="methods"></a>Методы
Прямые запросы на этот ресурс не поддерживаются. Сведения о [том,](domain.md) как запрашивать записи службы домена, см. в разделе домен.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String| Уникальный идентификатор, присвоенный этому объекту. Не является недействительным, только для чтения.|
|isOptional|Логический| Если это не так, запись MX должна быть настроена клиентом в хосте DNS, чтобы Microsoft Online Services правильно работать с доменом. |
|подпись|Строка| Значение, используемого при настройке свойства *псевдонима/хоста/имени* записи MX в хосте DNS. |
|mailExchange|Строка| Значение, используемого при настройке *ответа/назначения/значения* записи MX в хосте DNS.|
|предпочтение|Int32| Значение, используемое при настройке свойства *Preference/Priority* записи MX в хосте DNS. |
|recordType|String| Тип записи DNS. Значение всегда *Mx*. Key |
|supportedService|Строка| Microsoft Online Service или функция, зависимая от этой записи MX.</br></br>Может быть одним из следующих значений: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune* |
|ttl|Int32| Значение, используемого при настройке свойства времени для жизни *(ttl)* записи MX в хосте DNS. Не является недействительным |

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

