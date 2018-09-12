# <a name="iosstoreapp-resource-type"></a>Тип ресурса iosStoreApp

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Содержит свойства, в том числе унаследованные, для приложений из магазина iOS.

Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление iosStoreApps](../api/intune_apps_iosstoreapp_list.md)|Коллекция [iosStoreApp](../resources/intune_apps_iosstoreapp.md)|Список свойств и связей объектов [iosStoreApp](../resources/intune_apps_iosstoreapp.md).|
|[Получение iosStoreApp](../api/intune_apps_iosstoreapp_get.md)|[iosStoreApp](../resources/intune_apps_iosstoreapp.md)|Считывание свойств и связей объекта [iosStoreApp](../resources/intune_apps_iosstoreapp.md).|
|[Создание iosStoreApp](../api/intune_apps_iosstoreapp_create.md)|[iosStoreApp](../resources/intune_apps_iosstoreapp.md)|Создание объекта [iosStoreApp](../resources/intune_apps_iosstoreapp.md).|
|[Удаление iosStoreApp](../api/intune_apps_iosstoreapp_delete.md)|None|Удаление экземпляра [iosStoreApp](../resources/intune_apps_iosstoreapp.md).|
|[Обновление iosStoreApp](../api/intune_apps_iosstoreapp_update.md)|[iosStoreApp](../resources/intune_apps_iosstoreapp.md)|Обновление свойств объекта [iosStoreApp](../resources/intune_apps_iosstoreapp.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).|
|displayName|Строка|Название приложения, которое предоставил или импортировал администратор. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).|
|описание|Строка|Описание приложения. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).|
|publisher|Строка|Издатель приложения. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).|
|largeIcon|[mimeContent](../resources/intune_shared_mimecontent.md)|Большой значок, который отображается в сведениях о приложении и используется для отправки значка. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).|
|createdDateTime|DateTimeOffset|Дата и время создания приложения. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения приложения. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).|
|isFeatured|Логический|Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).|
|privacyInformationUrl|Строка|URL-адрес заявления о конфиденциальности. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).|
|informationUrl|Строка|URL-адрес страницы с дополнительными сведениями. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).|
|owner|Строка|Владелец приложения. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).|
|developer|Строка|Разработчик приложения. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).|
|notes|Строка|Примечания к приложению. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).|
|publishingState|[mobileAppPublishingState](../resources/intune_apps_mobileapppublishingstate.md)|Состояние публикации приложения. Приложение невозможно назначить, если оно не опубликовано. Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md). Возможные значения: `notPublished`, `processing`, `published`.|
|bundleId|Строка|Имя удостоверения.|
|appStoreUrl|Строка|URL-адрес в Apple App Store|
|applicableDeviceType|[iosDeviceType](../resources/intune_apps_iosdevicetype.md)|Архитектура iOS, поддерживаемая этим приложением.|
|minimumSupportedOperatingSystem|[iosMinimumOperatingSystem](../resources/intune_apps_iosminimumoperatingsystem.md)|Значение, которое представляет минимальную применимую версию операционной системы.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|categories|Коллекция объектов [mobileAppCategory](../resources/intune_apps_mobileappcategory.md)|Список категорий для этого приложения. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).|
|assignments|Коллекция [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)|Список назначений группы для этого мобильного приложения. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.mobileApp",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosStoreApp"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.iosStoreApp",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "isFeatured": true,
  "privacyInformationUrl": "String",
  "informationUrl": "String",
  "owner": "String",
  "developer": "String",
  "notes": "String",
  "publishingState": "String",
  "bundleId": "String",
  "appStoreUrl": "String",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true
  }
}
```








