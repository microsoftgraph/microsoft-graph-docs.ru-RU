---
title: Тип ресурса logonUser
description: Содержит сведения о состоянии пользователя, вошедшего в систему на этом узле
localization_priority: Normal
ms.openlocfilehash: 3b7862555c62eb16aaceaa53d4df58541426e08a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562659"
---
# <a name="logonuser-resource-type"></a>Тип ресурса logonUser

Содержит сведения о состоянии пользователя, вошедшего в систему на этом узле

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|Аккаунтдомаин|String|Домен учетной записи пользователя, используемой для входа в систему.|
|имя_учетной_записи|String|Имя учетной записи пользователя, используемой для входа в систему.|
|accountType|String|Тип учетной записи пользователя для каждого определения Windows. Возможные значения: `unknown`, `standard`, `power`, `administrator`.|
|Фирстсиндатетиме|DateTimeOffset|Значение даты и времени, по достижении которого выполнялась самая ранняя учетная запись пользователя (период, определенный поставщиком). Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|Ластсиндатетиме|DateTimeOffset|Дата и время последнего входа в систему с учетной записью пользователя. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|Логонид|String|Идентификатор входа пользователя.|
|Logontypes задано|Коллекция String|Коллекция типов входа в систему для вошедшего пользователя, начиная с первого до последнего обнаружения. Возможные значения: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.|

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
