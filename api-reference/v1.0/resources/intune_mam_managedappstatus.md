# <a name="managedappstatus-resource-type"></a>Тип ресурса managedAppStatus

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Представляет состояние защиты и конфигурации приложений для организации.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов managedAppStatus](../api/intune_mam_managedappstatus_list.md)|Коллекция [managedAppStatus](../resources/intune_mam_managedappstatus.md)|Список свойств и связей объектов [managedAppStatus](../resources/intune_mam_managedappstatus.md).|
|[Получение объекта managedAppStatus](../api/intune_mam_managedappstatus_get.md)|[managedAppStatus](../resources/intune_mam_managedappstatus.md)|Чтение свойств и связей объекта [managedAppStatus](../resources/intune_mam_managedappstatus.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Понятное имя отчета о состоянии.|
|id|String|Ключ объекта.|
|version|String|Версия объекта.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppStatus",
  "displayName": "String",
  "id": "String (identifier)",
  "version": "String"
}
```



