---
title: Тип ресурса Регистрикэйстате
description: Содержит сведения об изменениях в реестре, связанных с предупреждением, и процесс, который изменил разделы реестра.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: b07f031fed393c4de41a55b55e8009ca9c8d8259
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806795"
---
# <a name="registrykeystate-resource-type"></a>Тип ресурса Регистрикэйстате

Пространство имен: microsoft.graph

Содержит сведения об изменениях в реестре, связанных с предупреждением, и процесс, который изменил разделы реестра.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|семейства|registryHive|[Куст реестра Windows](/windows/desktop/sysinfo/registry-hives) : <ul><li>HKEY_CURRENT_CONFIG</li> <li>HKEY_CURRENT_USER</li> <li>HKEY_LOCAL_MACHINE \САМ</li> <li>HKEY_LOCAL_MACHINE \Секурити</li> <li>HKEY_LOCAL_MACHINE \Софтваре</li> <li>HKEY_LOCAL_MACHINE \Систем</li> <li>HKEY_USERS \\ . Умолчани.</li></ul> Возможные значения: `unknown`, `currentConfig`, `currentUser`, `localMachineSam`, `localMachineSecurity`, `localMachineSoftware`, `localMachineSystem`, `usersDefault`.|
|ключа|String|Текущий (то есть измененный) раздел реестра (исключая КУСТ).|
|олдкэй|String|Предыдущий (то есть перед изменением) раздел реестра (исключает КУСТ).|
|олдвалуедата|String|Previous (то есть перед изменением) значение раздела реестра (Content).|
|олдвалуенаме|String|Previous (то есть перед изменением) имя значения раздела реестра.|
|восстановление|registryOperation|Операция, в которой изменилось имя и/или значение раздела реестра. Возможные значения: `unknown`, `create`, `modify`, `delete`.|
|processId|Int32|Идентификатор процесса (PID), который изменил раздел реестра (сведения о процессе будут отображаться в коллекции предупреждений "процессы").|
|валуедата|String|Текущие (то есть измененные) данные значения раздела реестра (содержимое).|
|valueName|String|Current (то есть изменено) имя значения раздела реестра|
|Типом|registryValueType|[Тип значения раздела реестра](/windows/desktop/sysinfo/registry-value-types) <ul><li>REG_BINARY</li> <li>REG_DWORD</li> <li>REG_DWORD_LITTLE_ENDIAN</li> <li>REG_DWORD_BIG_ENDIAN</li><li>REG_EXPAND_SZ</li> <li>REG_LINK</li> <li>REG_MULTI_SZ</li> <li>REG_NONE</li> <li>REG_QWORD</li> <li>REG_QWORD_LITTLE_ENDIAN</li> <li>REG_SZ</li></ul> Возможные значения: `unknown`, `binary`, `dword`, `dwordLittleEndian`, `dwordBigEndian`, `expandSz`, `link`, `multiSz`, `none`, `qword`, `qwordlittleEndian`, `sz`.|

## <a name="json-representation"></a>Представление в формате JSON

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
