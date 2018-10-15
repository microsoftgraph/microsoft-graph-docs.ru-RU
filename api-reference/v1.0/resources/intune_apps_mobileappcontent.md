# <a name="mobileappcontent-resource-type"></a>Тип ресурса mobileAppContent

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Содержит свойства контента для определенной версии приложения. Каждому объекту mobileAppContent может соответствовать несколько объектов mobileAppContentFile.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов mobileAppContents](../api/intune_apps_mobileappcontent_list.md)|Коллекция [mobileAppContent](../resources/intune_apps_mobileappcontent.md)|Список свойств и связей объектов [mobileAppContent](../resources/intune_apps_mobileappcontent.md).|
|[Получение объекта mobileAppContent](../api/intune_apps_mobileappcontent_get.md)|[mobileAppContent](../resources/intune_apps_mobileappcontent.md)|Чтение свойств и связей объекта [mobileAppContent](../resources/intune_apps_mobileappcontent.md).|
|[Создание объекта mobileAppContent](../api/intune_apps_mobileappcontent_create.md)|[mobileAppContent](../resources/intune_apps_mobileappcontent.md)|Создание объекта [mobileAppContent](../resources/intune_apps_mobileappcontent.md).|
|[Удаление объекта mobileAppContent](../api/intune_apps_mobileappcontent_delete.md)|Нет|Удаляет объект [mobileAppContent](../resources/intune_apps_mobileappcontent.md).|
|[Обновление объекта mobileAppContent](../api/intune_apps_mobileappcontent_update.md)|[mobileAppContent](../resources/intune_apps_mobileappcontent.md)|Обновление свойств объекта [mobileAppContent](../resources/intune_apps_mobileappcontent.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Версия контента приложения.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|files|Коллекция [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md)|Список файлов для этой версии контента приложения.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppContent"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "String (identifier)"
}
```








