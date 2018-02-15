# <a name="user-resource-type"></a>Тип ресурса user

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Н/Д
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление пользователей](../api/intune_devices_user_list.md)|Коллекция объектов [user](../resources/intune_devices_user.md)|Список свойств и связей объектов [user](../resources/intune_devices_user.md).|
|[Получение пользователя](../api/intune_devices_user_get.md)|[user](../resources/intune_devices_user.md)|Чтение свойств и связей объекта [user](../resources/intune_devices_user.md).|
|[Создание пользователя](../api/intune_devices_user_create.md)|[user](../resources/intune_devices_user.md)|Создание объекта [user](../resources/intune_devices_user.md).|
|[Удаление пользователя](../api/intune_devices_user_delete.md)|Нет|Удаляет объект [user](../resources/intune_devices_user.md).|
|[Обновление пользователя](../api/intune_devices_user_update.md)|[user](../resources/intune_devices_user.md)|Обновление свойств объекта [user](../resources/intune_devices_user.md).|
|[Действие removeAllDevicesFromManagement](../api/intune_devices_user_removealldevicesfrommanagement.md)|Нет|Прекращение управления всеми устройствами для этого пользователя|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор пользователя.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|managedDevices|Коллекция [managedDevice](../resources/intune_devices_manageddevice.md)|Управляемые устройства, связанные с пользователем.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.user"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.user",
  "id": "String (identifier)"
}
```



