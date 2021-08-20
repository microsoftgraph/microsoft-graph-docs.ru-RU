---
title: тип ресурса logonUser
description: Содержит сведения о входе пользователя в этот хост
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 20a5f4ab827a09fd6254f3cbe8a590eb20fd76223eb8f24445fbe3b52a5f3ea5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54193484"
---
# <a name="logonuser-resource-type"></a>тип ресурса logonUser

Пространство имен: microsoft.graph

Содержит сведения о входе пользователя в этот хост

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|accountDomain|Строка|Домен учетной записи пользователя, используемый для логона.|
|имя учетной записи|Строка|Имя учетной записи учетной записи пользователя, используемой для логона.|
|accountType|Строка|Тип учетной записи пользователя, Windows определение. Возможные значения: `unknown`, `standard`, `power`, `administrator`.|
|firstSeenDateTime|DateTimeOffset|DateTime, в котором произошел самый ранний логотип этой учетной записи пользователя (период, определяемый поставщиком). Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|lastSeenDateTime|DateTimeOffset|DateTime, в котором произошел последний логотип этой учетной записи пользователя. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|logonId|String|ID логотипа пользователя.|
|logonTypes|Коллекция String|Коллекция типов логотипов, наблюдаемых для входа в систему пользователя с первого до последнего вида. Возможные значения: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.|

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


