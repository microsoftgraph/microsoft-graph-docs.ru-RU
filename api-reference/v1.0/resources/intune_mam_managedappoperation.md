# <a name="managedappoperation-resource-type"></a>Тип ресурса managedAppOperation

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Представляет операцию, примененную к регистрации приложения.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов List managedAppOperation](../api/intune_mam_managedappoperation_list.md)|Коллекция [managedAppOperation](../resources/intune_mam_managedappoperation.md)|Список свойств и связей объектов [managedAppOperation](../resources/intune_mam_managedappoperation.md).|
|[Получение объекта managedAppOperation](../api/intune_mam_managedappoperation_get.md)|[managedAppOperation](../resources/intune_mam_managedappoperation.md)|Чтение свойств и связей объекта [managedAppOperation](../resources/intune_mam_managedappoperation.md).|
|[Создание объекта managedAppOperation](../api/intune_mam_managedappoperation_create.md)|[managedAppOperation](../resources/intune_mam_managedappoperation.md)|Создание объекта [managedAppOperation](../resources/intune_mam_managedappoperation.md).|
|[Удаление объекта managedAppOperation](../api/intune_mam_managedappoperation_delete.md)|Нет|Удаляет объекта [managedAppOperation](../resources/intune_mam_managedappoperation.md).|
|[Обновление объекта managedAppOperation](../api/intune_mam_managedappoperation_update.md)|[managedAppOperation](../resources/intune_mam_managedappoperation.md)|Обновление свойств объекта [managedAppOperation](../resources/intune_mam_managedappoperation.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String (строка)|Имя операции.|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения операции для приложения.|
|state|String (строка)|Текущее состояние операции|
|id|String (строка)|Ключ объекта.|
|version|String (строка)|Версия объекта.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.managedAppOperation"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "state": "String",
  "id": "String (identifier)",
  "version": "String"
}
```



