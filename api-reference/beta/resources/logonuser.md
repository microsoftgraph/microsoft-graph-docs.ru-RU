---
title: Тип ресурса logonUser
description: Содержит информацию о состояниях о пользователя, выполнившего вход на этом узле
ms.openlocfilehash: 80ff69453e99f5cd5103f85cd7d8c45696057f7c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081792"
---
# <a name="logonuser-resource-type"></a>Тип ресурса logonUser

Содержит информацию о состояниях о пользователя, выполнившего вход на этом узле

## <a name="properties"></a>Свойства

| Свойство   | Тип |Description|
|:---------------|:--------|:----------|
|accountDomain|String|Домен учетной записи пользователя, используемое для входа в систему.|
|Имя учетной записи|String|Имя учетной записи учетная запись пользователя, используемая для входа в систему.|
|accountType|String|Тип учетной записи пользователя, для определения Windows. Возможные значения: `unknown`, `standard`, `power`, `administrator`.|
|firstSeenDateTime|DateTimeOffset|DateTime, в которой произошло раннюю вход в систему с этой учетной записи пользователя (определяются поставщика период). Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|lastSeenDateTime|DateTimeOffset|DateTime, в которой произошло последнего входа в систему с этой учетной записи пользователя. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|logonId|String|Идентификатор входа пользователя.|
|logonTypes|Коллекция String|Коллекция типов входа в систему, наблюдаемая для пользователя, выполнившего вход из при до последнего Заметим. Возможные значения: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.|

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