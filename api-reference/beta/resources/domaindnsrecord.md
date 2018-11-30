---
title: Тип ресурса domainDnsRecord
description: Для каждого домена в клиентов может потребоваться добавление записи DNS для файла зоны DNS домена этого домена, которые могут использоваться с Microsoft Online Services. Сущность **DomainDnsRecord** используется для представления таких записей DNS. Базовая сущность для DomainDnsCnameRecord, DomainDnsMxRecord, DomainDnsSrvRecord и DomainDnsSrvRecord сущностей.
ms.openlocfilehash: 766e3b241550ac1b0c7abdecaa22fe010955d05a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075540"
---
# <a name="domaindnsrecord-resource-type"></a>Тип ресурса domainDnsRecord

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Для работы служб Microsoft Online Services с доменом необходимо добавить записи DNS в файл зоны DNS домена. Объект **DomainDnsRecord** представляет такие записи DNS. Базовый объект для объектов [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md) и [DomainDnsSrvRecord](domaindnssrvrecord.md).

## <a name="methods"></a>Методы
Прямые запросы к этому ресурсу не поддерживаются. Сведения о том, как запрашивать записи службы доменов, см. в статье [о доменах](domain.md).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String| Уникальный идентификатор, назначенный этому объекту. Не допускает значения null, только для чтения.|
|isOptional|Логический| Если указано значение false, для правильной работы служб Microsoft Online Services с доменом клиент должен настроить эту запись на узле DNS. |
|label|Строка| Значение, используемое при настройке имени записи DNS на узле DNS. |
|recordType|Строка| Указывает, какой тип записи DNS представляет этот объект.</br></br>Возможные значения: *CName*, *Mx*, *Srv*, *Txt*.</br></br>Ключ |
|supportedService|Строка| Веб-служба или функция Майкрософт, зависящая от этой записи DNS.</br></br>Возможные значения: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*|
|ttl|Int32| Значение, используемое при настройке свойства срока жизни (ttl) записи DNS на узле DNS. Не допускает значение null. |

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
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