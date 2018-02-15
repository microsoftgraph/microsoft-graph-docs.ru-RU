# <a name="mobileappcategory-resource-type"></a>Тип ресурса mobileAppCategory

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Содержит свойства для одной категории приложений Intune.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов mobileAppCategory](../api/intune_apps_mobileappcategory_list.md)|Коллекция [mobileAppCategory](../resources/intune_apps_mobileappcategory.md)|Список свойств и связей объектов [mobileAppCategory](../resources/intune_apps_mobileappcategory.md).|
|[Получение объекта mobileAppCategory](../api/intune_apps_mobileappcategory_get.md)|[mobileAppCategory](../resources/intune_apps_mobileappcategory.md)|Чтение свойств и связей объекта [mobileAppCategory](../resources/intune_apps_mobileappcategory.md).|
|[Создание объекта mobileAppCategory](../api/intune_apps_mobileappcategory_create.md)|[mobileAppCategory](../resources/intune_apps_mobileappcategory.md)|Создание объекта [mobileAppCategory](../resources/intune_apps_mobileappcategory.md).|
|[Удаление объекта mobileAppCategory](../api/intune_apps_mobileappcategory_delete.md)|Нет|Удаляет объект [mobileAppCategory](../resources/intune_apps_mobileappcategory.md).|
|[Обновление объекта mobileAppCategory](../api/intune_apps_mobileappcategory_update.md)|[mobileAppCategory](../resources/intune_apps_mobileappcategory.md)|Обновление свойств объекта [mobileAppCategory](../resources/intune_apps_mobileappcategory.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|displayName|String|Имя категории приложений.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения mobileAppCategory.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```



