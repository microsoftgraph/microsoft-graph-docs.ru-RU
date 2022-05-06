---
title: Тип ресурса domainDnsRecord
description: Сущность domainDnsRecord используется для представления записей DNS.
ms.localizationpriority: medium
author: adimitui
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 327a07fcbca5c9c02bca90e46ceff9454c3267f3
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2022
ms.locfileid: "65246561"
---
# <a name="domaindnsrecord-resource-type"></a>Тип ресурса domainDnsRecord

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Для каждого [домена](domain.md) в клиенте может потребоваться добавить записи DNS в файл зоны DNS домена, прежде чем домен может использоваться Microsoft Online Services. Сущность **domainDnsRecord** используется для представления таких записей DNS. Этот тип ресурса является базовой сущностью для следующих ресурсов:
+ [domainDnsCnameRecord](domaindnscnamerecord.md);
+ [domainDnsMxRecord](domaindnsmxrecord.md);
+ [domainDnsSrvRecord](domaindnssrvrecord.md);
+ [domainDnsTxtRecord](domaindnstxtrecord.md);
+ [domainDnsUnavailableRecord](domaindnsunavailablerecord.md).

## <a name="methods"></a>Методы

Нет.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|String| Уникальный идентификатор, назначенный этой сущности. Не допускает значения NULL, только для чтения.|
|isOptional|Boolean| Если значение равно false, эта запись должна быть настроена клиентом на узле DNS для правильной работы microsoft Online Services с доменом. |
|label|String| Значение, используемое при настройке имени записи DNS на узле DNS. |
|recordType|String| Указывает, какой тип записи DNS представляет эта сущность.</br></br>Значение может быть одним из следующих: `CName`, , `Mx``Srv`, `Txt`. |
|supportedService|String| Microsoft Online Service или компонент, который зависит от этой записи DNS.</br></br>Может иметь одно из следующих значений: `null`, , `Email`, `Sharepoint`, `EmailInternalRelayOnly`, `OfficeCommunicationsOnline`, `FullRedelegation``SharePointDefaultDomain`, `SharePointPublic`, `OrgIdAuthentication``Yammer`. `Intune`|
|Ttl|Int32| Значение, используемое при настройке свойства срока жизни (ttl) записи DNS на узле DNS. Значение null не допускается. |

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
<!--
{
  "type": "#page.annotation",
  "description": "domainDnsRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


