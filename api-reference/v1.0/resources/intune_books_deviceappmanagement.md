# <a name="deviceappmanagement-resource-type"></a>Тип ресурса deviceAppManagement

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Одноэлементный объект, служащий контейнером для всех функций управления приложениями на устройствах.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение объекта deviceAppManagement](../api/intune_books_deviceappmanagement_get.md)|[deviceAppManagement](../resources/intune_books_deviceappmanagement.md)|Чтение свойств и связей объекта [deviceAppManagement](../resources/intune_books_deviceappmanagement.md).|
|[Обновление объекта deviceAppManagement](../api/intune_books_deviceappmanagement_update.md)|[deviceAppManagement](../resources/intune_books_deviceappmanagement.md)|Обновление свойств объекта [deviceAppManagement](../resources/intune_books_deviceappmanagement.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|managedEBooks|Коллекция [managedEBook](../resources/intune_books_managedebook.md)|Управляемая электронная книга.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAppManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "String (identifier)"
}
```



