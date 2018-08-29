# <a name="managedmobileapp-resource-type"></a>Тип ресурса managedMobileApp

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Идентификатор для развертывания приложения.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов managedMobileApp](../api/intune_mam_managedmobileapp_list.md)|Коллекция [managedMobileApp](../resources/intune_mam_managedmobileapp.md)|Список свойств и связей объектов [managedMobileApp](../resources/intune_mam_managedmobileapp.md).|
|[Получение объекта managedMobileApp](../api/intune_mam_managedmobileapp_get.md)|[managedMobileApp](../resources/intune_mam_managedmobileapp.md)|Чтение свойств и связей объекта [managedMobileApp](../resources/intune_mam_managedmobileapp.md).|
|[Создание объекта managedMobileApp](../api/intune_mam_managedmobileapp_create.md)|[managedMobileApp](../resources/intune_mam_managedmobileapp.md)|Создание объекта [managedMobileApp](../resources/intune_mam_managedmobileapp.md).|
|[Удаление объекта managedMobileApp](../api/intune_mam_managedmobileapp_delete.md)|Нет|Удаляет объект [managedMobileApp](../resources/intune_mam_managedmobileapp.md).|
|[Обновление объекта managedMobileApp](../api/intune_mam_managedmobileapp_update.md)|[managedMobileApp](../resources/intune_mam_managedmobileapp.md)|Обновление свойств объекта [managedMobileApp](../resources/intune_mam_managedmobileapp.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|mobileAppIdentifier|[mobileAppIdentifier](../resources/intune_mam_mobileappidentifier.md)|Идентификатор приложения с типом его операционной системы.|
|id|Строка|Ключ объекта.|
|version|Строка​|Версия объекта.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.managedMobileApp"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "id": "String (identifier)",
  "version": "String"
}
```



