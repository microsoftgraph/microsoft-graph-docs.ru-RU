# <a name="exclusiongroupassignmenttarget-resource-type"></a>Тип ресурса exclusionGroupAssignmentTarget

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Представляет группу, которую следует исключить из назначения.

Наследуется от [groupAssignmentTarget](../resources/intune_shared_groupassignmenttarget.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|groupId|Строка|ИД группы, являющейся объектом назначения. Наследуется от [groupAssignmentTarget](../resources/intune_shared_groupassignmenttarget.md)|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.groupAssignmentTarget",
  "@odata.type": "microsoft.graph.exclusionGroupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.exclusionGroupAssignmentTarget",
  "groupId": "String"
}
```



