---
title: тип ресурса процесса
description: Содержит сведения о процессе, связанном с оповещением.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d29a09b2d593fcf1c4a3cb5bee4230e57e9836d2
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720732"
---
# <a name="process-resource-type"></a>тип ресурса процесса

Пространство имен: microsoft.graph

Содержит сведения о процессе, связанном с оповещением.

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|accountName|String|Идентификатор учетной записи пользователя (контекст учетной записи пользователя, в котором был указан процесс), например, Имя учетной записи, SID и так далее.|
|commandLine|String|Командная линия полного призыва процесса, включая все параметры.|
|createdDateTime|DateTimeOffset|Время начала процесса. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|fileHash|[fileHash](filehash.md)|Сложный тип, содержащий хеши файлов (криптографические и чувствительные к расположению).|
|integrityLevel|processIntegrityLevel|Уровень целостности процесса. Возможные значения: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.|
|isElevated|Логический|True, если процесс повышен.|
|name|String|Имя файла Image процесса.|
|parentProcessCreatedDateTime|DateTimeOffset|DateTime, на котором был запущен родительский процесс. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|parentProcessId|Int32|ID процесса (PID) родительского процесса.|
|parentProcessName|String|Имя файла изображений родительского процесса.|
|path|String|Полный путь, включая имя файла.|
|processId|Int32|ID процесса (PID) процесса.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.process"
}-->

```json
{
  "accountName": "String",
  "commandLine": "String",
  "createdDateTime": "String (timestamp)",
  "fileHash": {"@odata.type": "microsoft.graph.fileHash"},
  "integrityLevel": "@odata.type: microsoft.graph.processIntegrityLevel",
  "isElevated": true,
  "name": "String",
  "parentProcessCreatedDateTime": "String (timestamp)",
  "parentProcessId": 1024,
  "parentProcessName": "String",
  "path": "String",
  "processId": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "process resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

