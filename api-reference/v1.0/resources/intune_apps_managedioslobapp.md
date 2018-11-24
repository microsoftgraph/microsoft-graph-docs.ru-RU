# <a name="managedioslobapp-resource-type"></a>Тип ресурса managedIOSLobApp

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Содержит свойства, в том числе унаследованные, для управляемых бизнес-приложений iOS.

Наследуется от [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление managedIOSLobApps](../api/intune_apps_managedioslobapp_list.md)|Коллекция [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md)|Список свойств и связей объектов [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md).|
|[Получение managedIOSLobApp](../api/intune_apps_managedioslobapp_get.md)|[managedIOSLobApp](../resources/intune_apps_managedioslobapp.md)|Считывание свойств и связей объекта [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md).|
|[Создание managedIOSLobApp](../api/intune_apps_managedioslobapp_create.md)|[managedIOSLobApp](../resources/intune_apps_managedioslobapp.md)|Создание объекта [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md).|
|[Удаление managedIOSLobApp](../api/intune_apps_managedioslobapp_delete.md)|None|Удаление экземпляра [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md).|
|[Обновление managedIOSLobApp](../api/intune_apps_managedioslobapp_update.md)|[managedIOSLobApp](../resources/intune_apps_managedioslobapp.md)|Обновление свойств объекта [managedIOSLobApp](../resources/intune_apps_managedioslobapp.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).|
|displayName|String|Название приложения, которое предоставил или импортировал администратор. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).|
|description|String|Описание приложения. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).|
|publisher|String|Издатель приложения. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).|
|largeIcon|[mimeContent](../resources/intune_shared_mimecontent.md)|Большой значок, который отображается в сведениях о приложении и используется для отправки значка. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).|
|createdDateTime|DateTimeOffset|Дата и время создания приложения. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения приложения. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).|
|isFeatured|Boolean|Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).|
|privacyInformationUrl|String|URL-адрес заявления о конфиденциальности. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).|
|informationUrl|String|URL-адрес страницы с дополнительными сведениями. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).|
|owner|String|Владелец приложения. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).|
|developer|String|Разработчик приложения. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).|
|notes|String|Примечания к приложению. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).|
|publishingState|[mobileAppPublishingState](../resources/intune_apps_mobileapppublishingstate.md)|Состояние публикации приложения. Приложение невозможно назначить, если оно не опубликовано. Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md). Возможные значения: `notPublished`, `processing`, `published`.|
|appAvailability|[managedAppAvailability](../resources/intune_apps_managedappavailability.md)|Доступность приложения. Наследуется от [managedApp](../resources/intune_apps_managedapp.md). Возможные значения: `global`, `lineOfBusiness`.|
|version|String|Версия приложения. Наследуется от объекта [managedApp](../resources/intune_apps_managedapp.md).|
|committedContentVersion|String|Внутренняя версия подтвержденного содержимого. Наследуется от объекта [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md).|
|fileName|String|Имя основного файла бизнес-приложения. Наследуется от объекта [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md).|
|size|Int64|Общий размер, включая все отправленные файлы. Наследуется от объекта [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md).|
|bundleId|String|Имя удостоверения.|
|applicableDeviceType|[iosDeviceType](../resources/intune_apps_iosdevicetype.md)|Архитектура iOS, поддерживаемая этим приложением.|
|minimumSupportedOperatingSystem|[iosMinimumOperatingSystem](../resources/intune_apps_iosminimumoperatingsystem.md)|Значение, указывающее минимальную применимую версию операционной системы.|
|expirationDateTime|DateTimeOffset|Время окончания срока действия.|
|versionNumber|String|Номер версии управляемого бизнес-приложения для iOS.|
|buildNumber|String|Номер сборки управляемого бизнес-приложения для iOS.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|categories|Коллекция объектов [mobileAppCategory](../resources/intune_apps_mobileappcategory.md)|Список категорий для этого приложения. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).|
|assignments|Коллекция [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)|Список назначений группы для этого мобильного приложения. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).|
|contentVersions|Коллекция объектов [mobileAppContent](../resources/intune_apps_mobileappcontent.md)|Список версий содержимого для этого приложения. Наследуется от [managedMobileLobApp](../resources/intune_apps_managedmobilelobapp.md).|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedIOSLobApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
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
  "committedContentVersion": "String",
  "fileName": "String",
  "size": 1024,
  "bundleId": "String",
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
    "v11_0": true,
    "v12_0": true
  },
  "expirationDateTime": "String (timestamp)",
  "versionNumber": "String",
  "buildNumber": "String"
}
```



