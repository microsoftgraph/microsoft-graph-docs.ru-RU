---
title: Тип ресурса registryKeyState
description: Содержит сведения об изменениях раздела реестра, связанных с оповещением, и о процессе изменения разделов реестра.
ms.localizationpriority: medium
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: a3bdf345c5c34721563dd69c9f3df18695a333a3
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900109"
---
# <a name="registrykeystate-resource-type"></a>Тип ресурса registryKeyState

Пространство имен: microsoft.graph

Содержит сведения об изменениях раздела реестра, связанных с оповещением, и о процессе изменения разделов реестра.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|Куст|registryHive|Куст [реестра Windows](/windows/desktop/sysinfo/registry-hives) : <ul><li>HKEY_CURRENT_CONFIG</li> <li>HKEY_CURRENT_USER</li> <li>HKEY_LOCAL_MACHINE\SAM</li> <li>HKEY_LOCAL_MACHINE\Security</li> <li>HKEY_LOCAL_MACHINE\Software</li> <li>HKEY_LOCAL_MACHINE\System</li> <li>\\HKEY_USERS. По умолчанию.</li></ul> Возможные значения: `unknown`, `currentConfig`, `currentUser`, `localMachineSam`, `localMachineSecurity`, `localMachineSoftware`, `localMachineSystem`, `usersDefault`.|
|ключа|Строка|Текущий (то есть измененный) раздел реестра (не включает HIVE).|
|oldKey|Строка|Предыдущий (то есть до изменения) раздел реестра (исключая HIVE).|
|oldValueData|Строка|Предыдущие (то есть до изменения) данные о значении ключа реестра (содержимое).|
|oldValueName|Строка|Предыдущее (то есть перед изменением) имя значения раздела реестра.|
|Операции|registryOperation|Операция, которая изменила имя и (или) значение раздела реестра. Возможные значения: `unknown`, `create`, `modify`, `delete`.|
|processId|Int32|Идентификатор процесса, который изменил раздел реестра (сведения о процессе будут отображаться в коллекции оповещений "processes").|
|valueData|Строка|Текущие (то есть измененные) данные о значении ключа реестра (содержимое).|
|valueName|Строка|Текущее (то есть измененное) имя ключа реестра|
|Valuetype|registryValueType|[Тип значения раздела реестра](/windows/desktop/sysinfo/registry-value-types) <ul><li>REG_BINARY</li> <li>REG_DWORD</li> <li>REG_DWORD_LITTLE_ENDIAN</li> <li>REG_DWORD_BIG_ENDIAN</li><li>REG_EXPAND_SZ</li> <li>REG_LINK</li> <li>REG_MULTI_SZ</li> <li>REG_NONE</li> <li>REG_QWORD</li> <li>REG_QWORD_LITTLE_ENDIAN</li> <li>REG_SZ</li></ul> Возможные значения: `unknown`, `binary`, `dword`, `dwordLittleEndian`, `dwordBigEndian`, `expandSz`, `link`, `multiSz`, `none`, `qword`, `qwordlittleEndian`, `sz`.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.registryKeyState"
}-->

```json
{
  "hive": "@odata.type: microsoft.graph.registryHive",
  "key": "String",
  "oldKey": "String",
  "oldValueData": "String",
  "oldValueName": "String",
  "operation": "@odata.type: microsoft.graph.registryOperation",
  "processId": 1024,
  "valueData": "String",
  "valueName": "String",
  "valueType": "@odata.type: microsoft.graph.registryValueType"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "registryKeyState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

