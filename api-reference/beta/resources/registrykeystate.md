---
title: тип ресурса registryKeyState
description: Содержит сведения об изменениях ключей реестра, связанных с оповещением, и о процессе изменения ключей реестра.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 6bf8c232548a70603fc6c38d3228b3a08b11e47c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59074607"
---
# <a name="registrykeystate-resource-type"></a>тип ресурса registryKeyState

Пространство имен: microsoft.graph

Содержит сведения об изменениях ключей реестра, связанных с оповещением, и о процессе изменения ключей реестра.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|hive|registryHive|[Ульй Windows реестра:](/windows/desktop/sysinfo/registry-hives) <ul><li>HKEY_CURRENT_CONFIG</li> <li>HKEY_CURRENT_USER</li> <li>HKEY_LOCAL_MACHINE\SAM</li> <li>HKEY_LOCAL_MACHINE\Security</li> <li>HKEY_LOCAL_MACHINE\Software</li> <li>HKEY_LOCAL_MACHINE\System</li> <li>HKEY_USERS \\ . По умолчанию.</li></ul> Возможные значения: `unknown`, `currentConfig`, `currentUser`, `localMachineSam`, `localMachineSecurity`, `localMachineSoftware`, `localMachineSystem`, `usersDefault`.|
|ключа|String|Ключ текущего (то есть измененного) реестра (исключает HIVE).|
|oldKey|String|Предыдущий (то есть перед измененным) ключом реестра (исключает HIVE).|
|oldValueData|String|Предыдущие (то есть до изменения) данные ключевого значения реестра (содержимое).|
|oldValueName|String|Предыдущее (то есть перед измененным) имя ключевого значения реестра.|
|операция|registryOperation|Операция, изменивла имя и/или значение ключа реестра. Возможные значения: `unknown`, `create`, `modify`, `delete`.|
|processId|Int32|Процесс ID (PID) процесса, который изменил ключ реестра (сведения о процессе будут отображаться в коллекции процессов оповещения).|
|valueData|String|Текущие (то есть измененные) данные о ключевом значении реестра (содержимое).|
|valueName|String|Имя ключевого значения текущего (то есть измененного) реестра|
|valueType|registryValueType|[Тип ключевого значения реестра](/windows/desktop/sysinfo/registry-value-types) <ul><li>REG_BINARY</li> <li>REG_DWORD</li> <li>REG_DWORD_LITTLE_ENDIAN</li> <li>REG_DWORD_BIG_ENDIAN</li><li>REG_EXPAND_SZ</li> <li>REG_LINK</li> <li>REG_MULTI_SZ</li> <li>REG_NONE</li> <li>REG_QWORD</li> <li>REG_QWORD_LITTLE_ENDIAN</li> <li>REG_SZ</li></ul> Возможные значения: `unknown`, `binary`, `dword`, `dwordLittleEndian`, `dwordBigEndian`, `expandSz`, `link`, `multiSz`, `none`, `qword`, `qwordlittleEndian`, `sz`.|

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


