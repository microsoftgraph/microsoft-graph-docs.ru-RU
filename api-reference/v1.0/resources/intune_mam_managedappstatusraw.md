# <a name="managedappstatusraw-resource-type"></a>Тип ресурса managedAppStatusRaw

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Представляет нетипизированный отчет о состоянии, касающийся конфигурации и защиты приложений организации.

Наследуется от [managedAppStatus](../resources/intune_mam_managedappstatus.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление managedAppStatusRaws](../api/intune_mam_managedappstatusraw_list.md)|Коллекция [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md)|Перечисление свойств и связей объектов [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md).|
|[Получение managedAppStatusRaw](../api/intune_mam_managedappstatusraw_get.md)|[managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md)|Считывание свойств и связей объекта [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Понятное имя отчета о состоянии. Наследуется от объекта [managedAppStatus](../resources/intune_mam_managedappstatus.md).|
|id|String|Ключ объекта. Наследуется от объекта [managedAppStatus](../resources/intune_mam_managedappstatus.md).|
|version|String|Версия объекта. Наследуется от объекта [managedAppStatus](../resources/intune_mam_managedappstatus.md).|
|content|[Json](../resources/intune_mam_json.md)|Содержимое отчета о состоянии.|

## <a name="relationships"></a>Связи
None
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppStatusRaw"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppStatusRaw",
  "displayName": "String",
  "id": "String (identifier)",
  "version": "String",
  "content": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```



