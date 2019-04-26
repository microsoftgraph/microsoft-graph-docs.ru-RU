---
title: Тип ресурса Регистрикэйстате
description: Содержит сведения об изменениях в реестре, связанных с предупреждением, и процесс, который изменил разделы реестра.
localization_priority: Normal
ms.openlocfilehash: d07b0b6f502794154b400444eaf3854535e04547
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563002"
---
# <a name="registrykeystate-resource-type"></a>Тип ресурса Регистрикэйстате

Содержит сведения об изменениях в реестре, связанных с предупреждением, и процесс, который изменил разделы реестра.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|семейства|registryHive|[Куст реестра Windows](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-hives) : <ul><li>ХКЭЙ_КУРРЕНТ_КОНФИГ</li> <li>HKEY_CURRENT_USER</li> <li>ХКЭЙ_ЛОКАЛ_МАЧИНЕ\САМ</li> <li>Хкэй_локал_мачине\секурити</li> <li>Хкэй_локал_мачине\софтваре</li> <li>Хкэй_локал_мачине\систем</li> <li>HKEY_USERS\\. Умолчани.</li></ul> Возможные значения: `unknown`, `currentConfig`, `currentUser`, `localMachineSam`, `localMachineSecurity`, `localMachineSoftware`, `localMachineSystem`, `usersDefault`.|
|ключа|String|Текущий (то есть измененный) раздел реестра (исключая КУСТ).|
|Олдкэй|String|Предыдущий (то есть перед изменением) раздел реестра (исключает КУСТ).|
|Олдвалуедата|String|Previous (то есть перед изменением) значение раздела реестра (Content).|
|Олдвалуенаме|String|Previous (то есть перед изменением) имя значения раздела реестра.|
|восстановление|registryOperation|Операция, в которой изменилось имя и/или значение раздела реестра. Возможные значения: `unknown`, `create`, `modify`, `delete`.|
|processId|Int32|Идентификатор процесса (PID), который изменил раздел реестра (сведения о процессе будут отображаться в коллекции предупреждений "процессы").|
|Валуедата|String|Текущие (то есть измененные) данные значения раздела реестра (содержимое).|
|valueName|String|Current (то есть изменено) имя значения раздела реестра|
|Типом|registryValueType|[Тип значения раздела реестра](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-value-types) <ul><li>REG_BINARY</li> <li>REG_DWORD</li> <li>РЕГ_ДВОРД_ЛИТТЛЕ_ЕНДИАН</li> <li>РЕГ_ДВОРД_БИГ_ЕНДИАН</li><li>REG_EXPAND_SZ</li> <li>РЕГ_ЛИНК</li> <li>REG_MULTI_SZ</li> <li>РЕГ_НОНЕ</li> <li>РЕГ_КВОРД</li> <li>РЕГ_КВОРД_ЛИТТЛЕ_ЕНДИАН</li> <li>REG_SZ</li></ul> Возможные значения: `unknown`, `binary`, `dword`, `dwordLittleEndian`, `dwordBigEndian`, `expandSz`, `link`, `multiSz`, `none`, `qword`, `qwordlittleEndian`, `sz`.|

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
