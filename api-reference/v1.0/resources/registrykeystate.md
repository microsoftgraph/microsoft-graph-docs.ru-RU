# <a name="registrykeystate-resource-type"></a>Тип ресурса registryKeyState

Содержит сведения об изменениях раздела реестра, связанные с оповещением, и процесс, изменивший разделы реестра.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|hive|registryHive| [Куст реестра Windows](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-hives): <ul><li>HKEY_CURRENT_CONFIG</li> <li>HKEY_CURRENT_USER</li> <li>HKEY_LOCAL_MACHINE\SAM</li> <li>HKEY_LOCAL_MACHINE\Security</li> <li>HKEY_LOCAL_MACHINE\Software</li> <li>HKEY_LOCAL_MACHINE\System</li> <li>HKEY_USERS\\. Ветвь по умолчанию.</li></ul> Возможные значения: `unknown`, `currentConfig`, `currentUser`, `localMachineSam`, `localMachineSamSoftware`, `localMachineSystem`, `usersDefault`.|
|key|String|Текущий (то есть измененный) раздел реестра (исключая HIVE).|
|oldkey|String|Предыдущий (т.е. до изменения) раздел реестра (исключая HIVE).|
|oldValueData|String|Предыдущее (то есть до изменения) значение данных раздела реестра (содержимое).|
|oldValueName|String|Предыдущее (то есть перед изменением) имя значения раздела реестра.|
|operation|registryOperation|Операция, которая изменила имя и/или значение раздела реестра. Возможные значения: `unknown`, `create`, `modify`, `delete`.|
|processId|Int32|Идентификатор процесса (PID), изменивший раздел реестра (подробности процесса отобразятся в коллекции оповещения "процессы").|
|valueData|String|Текущие (то есть измененные) данные значения раздела реестра (содержимое).|
|valueName|String|Текущее (то есть измененное) имя значения раздела регистра|
|valueType|registryValueType|[Тип значения ключа реестра](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-value-types) <ul><li>REG_BINARY</li> <li>REG_DWORD</li> <li>REG_DWORD_LITTLE_ENDIAN</li> <li>REG_DWORD_BIG_ENDIAN</li><li>REG_EXPAND_SZ</li> <li>REG_LINK</li> <li>REG_MULTI_SZ</li> <li>REG_NONE</li> <li>REG_QWORD</li> <li>REG_QWORD_LITTLE_ENDIAN</li> <li>REG_SZ</li></ul> Возможные значения: `unknown`, `binary`, `dword`, `dwordLittleEndian`, `dwordBigEndian`, `expandSz`, `link`, `multiSz`, `none`, `qword`, `qwordlittleEndian`, `sz`.|

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