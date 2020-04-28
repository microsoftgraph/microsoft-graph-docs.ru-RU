---
title: Тип ресурса logonUser
description: Содержит сведения о состоянии пользователя, вошедшего в систему на этом узле
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: b9a7bb439863a39ce165235b31642e542b1bb331
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522899"
---
# <a name="logonuser-resource-type"></a>Тип ресурса logonUser

Пространство имен: microsoft.graph

Содержит сведения о состоянии пользователя, вошедшего в систему на этом узле

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|аккаунтдомаин|String|Домен учетной записи пользователя, используемой для входа в систему.|
|имя_учетной_записи|String|Имя учетной записи пользователя, используемой для входа в систему.|
|accountType|String|Тип учетной записи пользователя для каждого определения Windows. Возможные значения: `unknown`, `standard`, `power`, `administrator`.|
|фирстсиндатетиме|DateTimeOffset|Значение даты и времени, по достижении которого выполнялась самая ранняя учетная запись пользователя (период, определенный поставщиком). Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|ластсиндатетиме|DateTimeOffset|Дата и время последнего входа в систему с учетной записью пользователя. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|логонид|String|Идентификатор входа пользователя.|
|Logontypes задано|Коллекция объектов string|Коллекция типов входа в систему для вошедшего пользователя, начиная с первого до последнего обнаружения. Возможные значения: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.|

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
