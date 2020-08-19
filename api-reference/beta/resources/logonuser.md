---
title: Тип ресурса logonUser
description: Содержит сведения о состоянии пользователя, вошедшего в систему на этом узле
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: f480ff8c67c602512d7d8ef3f090366734f0ca7e
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808664"
---
# <a name="logonuser-resource-type"></a>Тип ресурса logonUser

Пространство имен: microsoft.graph

Содержит сведения о состоянии пользователя, вошедшего в систему на этом узле

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|аккаунтдомаин|String|Домен учетной записи пользователя, используемой для входа в систему.|
|accountName|String|Имя учетной записи пользователя, используемой для входа в систему.|
|accountType|String|Тип учетной записи пользователя для каждого определения Windows. Возможные значения: `unknown`, `standard`, `power`, `administrator`.|
|фирстсиндатетиме|DateTimeOffset|Значение даты и времени, по достижении которого выполнялась самая ранняя учетная запись пользователя (период, определенный поставщиком). Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|ластсиндатетиме|DateTimeOffset|Дата и время последнего входа в систему с учетной записью пользователя. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|логонид|String|Идентификатор входа пользователя.|
|Logontypes задано|Коллекция String|Коллекция типов входа в систему для вошедшего пользователя, начиная с первого до последнего обнаружения. Возможные значения: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.|

## <a name="json-representation"></a>Представление в формате JSON

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
