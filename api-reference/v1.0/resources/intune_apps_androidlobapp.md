# <a name="androidlobapp-resource-type"></a>Тип ресурса androidLobApp

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Содержит свойства, в том числе унаследованные, для бизнес-приложений Android.

Наследуется от [mobileLobApp](../resources/intune_apps_mobilelobapp.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление androidLobApps](../api/intune_apps_androidlobapp_list.md)|Коллекция [androidLobApp](../resources/intune_apps_androidlobapp.md)|Список свойств и связей объектов [androidLobApp](../resources/intune_apps_androidlobapp.md).|
|[Получение androidLobApp](../api/intune_apps_androidlobapp_get.md)|[androidLobApp](../resources/intune_apps_androidlobapp.md)|Считывание свойств и связей объекта [androidLobApp](../resources/intune_apps_androidlobapp.md).|
|[Создание androidLobApp](../api/intune_apps_androidlobapp_create.md)|[androidLobApp](../resources/intune_apps_androidlobapp.md)|Создание нового объекта [androidLobApp](../resources/intune_apps_androidlobapp.md).|
|[Удаление androidLobApp](../api/intune_apps_androidlobapp_delete.md)|None|Удаление экземпляра [androidLobApp](../resources/intune_apps_androidlobapp.md).|
|[Обновление androidLobApp](../api/intune_apps_androidlobapp_update.md)|[androidLobApp](../resources/intune_apps_androidlobapp.md)|Обновление свойств объекта [androidLobApp](../resources/intune_apps_androidlobapp.md).|

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
|packageId|String|Идентификатор пакета.|
|minimumSupportedOperatingSystem|[androidMinimumOperatingSystem](../resources/intune_apps_androidminimumoperatingsystem.md)|Значение, которое представляет минимальную применимую версию операционной системы.|
|versionName|String|Имя версии бизнес-приложения для Android.|
|versionCode|String|Код версии бизнес-приложения.|

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
  "@odata.type": "microsoft.graph.androidLobApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidLobApp",
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
  "packageId": "String",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  },
  "versionName": "String",
  "versionCode": "String"
}
```



