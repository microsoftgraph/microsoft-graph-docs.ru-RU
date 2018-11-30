---
title: Тип ресурса registryKeyState
description: Содержит сведения об изменениях ключа реестра, связанные с оповещение и процесс, изменений в реестр.
ms.openlocfilehash: 37654aab2bf8f0afae0f7ec6ed544aed8634dacc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026286"
---
# <a name="registrykeystate-resource-type"></a>Тип ресурса registryKeyState

Содержит сведения об изменениях ключа реестра, связанные с оповещение и процесс, изменений в реестр.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Description |
|:-------------|:------------|:------------|
|куст|registryHive|[Куст реестра Windows](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-hives) : <ul><li>HKEY_CURRENT_CONFIG</li> <li>HKEY_CURRENT_USER</li> <li>HKEY_LOCAL_MACHINE\SAM</li> <li>HKEY_LOCAL_MACHINE\Security</li> <li>HKEY_LOCAL_MACHINE\Software</li> <li>HKEY_LOCAL_MACHINE\System</li> <li>HKEY_USERS\\. По умолчанию.</li></ul> Возможные значения: `unknown`, `currentConfig`, `currentUser`, `localMachineSam`, `localMachineSamSoftware`, `localMachineSystem`, `usersDefault`.|
|key|String|Текущий (то есть измененные) системного реестра (исключает КУСТ).|
|oldKey|String|Предыдущий (то есть перед изменением) раздел реестра (исключает КУСТ).|
|oldValueData|String|Предыдущий (то есть до изменения) данных значение ключа реестра (содержимое).|
|oldValueName|String|Предыдущий (то есть перед изменением) имя раздела реестра.|
|операция|registryOperation|Операция, изменено имя раздела реестра и/или значение. Возможные значения: `unknown`, `create`, `modify`, `delete`.|
|processId|Int32|Обработать Идентификатором процесса изменения раздела реестра (процесс отображения сведений в коллекции оповещения «процессы»).|
|valueData|String|Текущий (то есть измененные) значение ключа реестра (содержимое).|
|Имени|String|Текущее имя значение ключа реестра (то есть измененные)|
|Тип значения|registryValueType|[Тип значения ключа реестра](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-value-types) <ul><li>REG_BINARY</li> <li>REG_DWORD</li> <li>REG_DWORD_LITTLE_ENDIAN</li> <li>REG_DWORD_BIG_ENDIAN</li><li>REG_EXPAND_SZ</li> <li>REG_LINK</li> <li>REG_MULTI_SZ</li> <li>REG_NONE</li> <li>REG_QWORD ИНТЕРФЕЙСА</li> <li>REG_QWORD_LITTLE_ENDIAN</li> <li>REG_SZ</li></ul> Возможные значения: `unknown`, `binary`, `dword`, `dwordLittleEndian`, `dwordBigEndian`, `expandSz`, `link`, `multiSz`, `none`, `qword`, `qwordlittleEndian`, `sz`.|

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