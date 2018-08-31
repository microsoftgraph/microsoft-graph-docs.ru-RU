# <a name="managediosstoreapp-resource-type"></a>Тип ресурса managedIOSStoreApp

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Содержит свойства, в том числе унаследованные, для приложения из магазина iOS, которым вы можете управлять с помощью политики защиты приложений Intune.

Наследуется от [managedApp](../resources/intune_apps_managedapp.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление managedIOSStoreApps](../api/intune_apps_managediosstoreapp_list.md)|Коллекция [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md)|Список свойств и связей объектов [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md).|
|[Получение managedIOSStoreApp](../api/intune_apps_managediosstoreapp_get.md)|[managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md)|Считывание свойств и связей объекта [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md).|
|[Создание managedIOSStoreApp](../api/intune_apps_managediosstoreapp_create.md)|[managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md)|Создание объекта [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md).|
|[Удаление managedIOSStoreApp](../api/intune_apps_managediosstoreapp_delete.md)|Нет|Удаление экземпляра [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md).|
|[Обновление managedIOSStoreApp](../api/intune_apps_managediosstoreapp_update.md)|[managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md)|Обновление свойств объекта [managedIOSStoreApp](../resources/intune_apps_managediosstoreapp.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String (строка)|Ключ объекта. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).|
|displayName|String (строка)|Название приложения, которое предоставил или импортировал администратор. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).|
|description|String (строка)|Описание приложения. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).|
|publisher|String (строка)|Издатель приложения. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).|
|largeIcon|[mimeContent](../resources/intune_shared_mimecontent.md)|Большой значок, который отображается в сведениях о приложении и используется для отправки значка. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).|
|createdDateTime|DateTimeOffset|Дата и время создания приложения. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения приложения. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).|
|isFeatured|Boolean (логический)|Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).|
|privacyInformationUrl|String (строка)|URL-адрес заявления о конфиденциальности. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).|
|informationUrl|String (строка)|URL-адрес страницы с дополнительными сведениями. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).|
|owner|String (строка)|Владелец приложения. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).|
|developer|String (строка)|Разработчик приложения. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).|
|notes|String (строка)|Примечания к приложению. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).|
|publishingState|[mobileAppPublishingState](../resources/intune_apps_mobileapppublishingstate.md)|Состояние публикации приложения. Приложение невозможно назначить, если оно не опубликовано. Унаследовано от [mobileApp](../resources/intune_apps_mobileapp.md). Возможные значения: `notPublished`, `processing`, `published`.|
|appAvailability|[managedAppAvailability](../resources/intune_apps_managedappavailability.md)|Доступность приложения. Унаследовано от [managedApp](../resources/intune_apps_managedapp.md). Возможные значения: `global`, `lineOfBusiness`.|
|version|String (строка)|Версия приложения. Наследуется от [managedApp](../resources/intune_apps_managedapp.md)|
|bundleId|String (строка)|Идентификатор пакета приложения.|
|appStoreUrl|String (строка)|AppStoreUrl для Apple.|
|applicableDeviceType|[iosDeviceType](../resources/intune_apps_iosdevicetype.md)|Архитектура iOS, поддерживаемая этим приложением.|
|minimumSupportedOperatingSystem|[iosMinimumOperatingSystem](../resources/intune_apps_iosminimumoperatingsystem.md)|Значение, которое представляет минимальную поддерживаемую версию операционной системы.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|categories|Коллекция объектов [mobileAppCategory](../resources/intune_apps_mobileappcategory.md)|Список категорий для этого приложения. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).|
|assignments|Коллекция [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)|Список назначений группы для этого мобильного приложения. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.managedApp",
  "@odata.type": "microsoft.graph.managedIOSStoreApp"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedIOSStoreApp",
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
  "appAvailability": "String",
  "version": "String",
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



