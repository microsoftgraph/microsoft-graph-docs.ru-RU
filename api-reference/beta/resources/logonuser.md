---
title: Тип ресурса logonUser
description: Содержит сведения с отслеживанием состояния пользователя, вошедщего в систему на этом узле.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: security
author: preetikr
ms.openlocfilehash: d665906abbbea3f49d352de5600c647f62d8bff6
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176785"
---
# <a name="logonuser-resource-type"></a>Тип ресурса logonUser

Пространство имен: microsoft.graph

Содержит сведения с отслеживанием состояния пользователя, вошедщего в систему на этом узле.

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|accountDomain|Строка|Домен учетной записи пользователя, используемой для входа в систему.|
|Accountname|Строка|Имя учетной записи пользователя, используемой для входа в систему.|
|accountType|Строка|Тип учетной записи пользователя на Windows определения. Возможные значения: `unknown`, `standard`, `power`, `administrator`.|
|firstSeenDateTime|DateTimeOffset|Дата и время, когда произошло время входа в систему этой учетной записи пользователя (определенный поставщиком период). Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|lastSeenDateTime|DateTimeOffset|Дата и время последнего входа этой учетной записи пользователя. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|LogonId|Строка|Идентификатор входа пользователя.|
|LogonTypes|Коллекция строк|Коллекция типов входа, наблюдаемых для пользователя, выполнив вход с первого по последний просмотр. Возможные значения: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.logonUser"
}-->

```json
{
  "accountDomain": "String",
  "accountName": "String",
  "accountType": "String",
  "firstSeenDateTime": "String (timestamp)",
  "lastSeenDateTime": "String (timestamp)",
  "logonId": "String",
  "logonTypes": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "logonUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


