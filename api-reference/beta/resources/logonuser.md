---
title: тип ресурса logonUser
description: Содержит сведения о входе пользователя в этот хост
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: c7c696850acfa66d4dfbbc345f518234c4698aac
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59120040"
---
# <a name="logonuser-resource-type"></a>тип ресурса logonUser

Пространство имен: microsoft.graph

Содержит сведения о входе пользователя в этот хост

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|accountDomain|String|Домен учетной записи пользователя, используемый для логона.|
|имя учетной записи|String|Имя учетной записи учетной записи пользователя, используемой для логона.|
|accountType|String|Тип учетной записи пользователя, Windows определение. Возможные значения: `unknown`, `standard`, `power`, `administrator`.|
|firstSeenDateTime|DateTimeOffset|DateTime, в котором произошел самый ранний логотип этой учетной записи пользователя (период, определяемый поставщиком). Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|lastSeenDateTime|DateTimeOffset|DateTime, в котором произошел последний логотип этой учетной записи пользователя. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|logonId|String|ID логотипа пользователя.|
|logonTypes|Коллекция объектов string|Коллекция типов логотипов, наблюдаемых для входа в систему пользователя с первого до последнего вида. Возможные значения: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.|

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


