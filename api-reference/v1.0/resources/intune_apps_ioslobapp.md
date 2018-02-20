# <a name="ioslobapp-resource-type"></a>Тип ресурса iosLobApp

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Содержит свойства, в том числе унаследованные, для бизнес-приложений iOS.

Наследуется от [mobileLobApp](../resources/intune_apps_mobilelobapp.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список iosLobApps](../api/intune_apps_ioslobapp_list.md)|Коллекция [iosLobApp](../resources/intune_apps_ioslobapp.md)|Список свойств и связей объектов [iosLobApp](../resources/intune_apps_ioslobapp.md).|
|[Получение iosLobApp](../api/intune_apps_ioslobapp_get.md)|[iosLobApp](../resources/intune_apps_ioslobapp.md)|Считывание свойств и связей объекта [iosLobApp](../resources/intune_apps_ioslobapp.md).|
|[Создание iosLobApp](../api/intune_apps_ioslobapp_create.md)|[iosLobApp](../resources/intune_apps_ioslobapp.md)|Создание нового объекта [iosLobApp](../resources/intune_apps_ioslobapp.md).|
|[Удаление iosLobApp](../api/intune_apps_ioslobapp_delete.md)|None|Удаление экземпляра [iosLobApp](../resources/intune_apps_ioslobapp.md).|
|[Обновление iosLobApp](../api/intune_apps_ioslobapp_update.md)|[iosLobApp](../resources/intune_apps_ioslobapp.md)|Обновление свойств объекта [iosLobApp](../resources/intune_apps_ioslobapp.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).|
|displayName|String|Администратор предоставил или импортировал название приложения. Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).|
|description|String|Описание приложения. Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).|
|publisher|String|Издатель приложения. Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).|
|largeIcon|[mimeContent](../resources/intune_apps_mimecontent.md)|Большой значок, отображается в сведениях о приложении и используется для отправки значка. Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).|
|createdDateTime|DateTimeOffset|Дата и время создания приложения. Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения приложения. Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).|
|isFeatured|Boolean|Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).|
|privacyInformationUrl|String|URL-адрес заявления о конфиденциальности. Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).|
|informationUrl|String|URL-адрес страницы с дополнительными сведениями. Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).|
|owner|String|Владелец приложения. Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).|
|developer|String|Разработчик приложения. Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).|
|notes|String|Заметки для приложения. Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).|
|publishingState|String|Состояние публикации для приложения. Приложение не может быть назначено, если оно не опубликовано. Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md). Допустимые значения: `notPublished`, `processing`, `published`.|
|committedContentVersion|String|Внутренняя версия подтвержденного содержимого. Наследуется от [mobileLobApp](../resources/intune_apps_mobilelobapp.md).|
|fileName|String|Имя основного файла бизнес-приложения. Наследуется от [mobileLobApp](../resources/intune_apps_mobilelobapp.md).|
|size|Int64|Общий размер, включая все отправленные файлы. Наследуется от [mobileLobApp](../resources/intune_apps_mobilelobapp.md).|
|bundleId|String|Имя удостоверения.|
|applicableDeviceType|[iosDeviceType](../resources/intune_apps_iosdevicetype.md)|Архитектура iOS, которая поддерживается этим приложением.|
|minimumSupportedOperatingSystem|[iosMinimumOperatingSystem](../resources/intune_apps_iosminimumoperatingsystem.md)|Значение, которое представляет минимальную применимую версию операционной системы.|
|expirationDateTime|DateTimeOffset|Срок действия.|
|versionNumber|String|Номер версии бизнес-приложения для iOS.|
|buildNumber|String|Номер сборки бизнес-приложения для iOS.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|categories|Коллекция [mobileAppCategory](../resources/intune_apps_mobileappcategory.md)|Список категорий для этого приложения. Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).|
|assignments|Коллекция [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)|Список назначений группы для этого мобильного приложения. Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).|
|contentVersions|Коллекция [mobileAppContent](../resources/intune_apps_mobileappcontent.md)|Список версий содержимого для этого приложения. Наследуется от [mobileLobApp](../resources/intune_apps_mobilelobapp.md).|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosLobApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosLobApp",
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
    "v11_0": true
  },
  "expirationDateTime": "String (timestamp)",
  "versionNumber": "String",
  "buildNumber": "String"
}
```



