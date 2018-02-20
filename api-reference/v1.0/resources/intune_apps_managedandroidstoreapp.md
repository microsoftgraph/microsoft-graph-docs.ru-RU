# <a name="managedandroidstoreapp-resource-type"></a>Тип ресурса managedAndroidStoreApp

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Содержит свойства, в том числе унаследованные, для приложений из магазина Android, которыми вы можете управлять с помощью политики защиты приложений Intune.

Наследуется от [managedApp](../resources/intune_apps_managedapp.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление managedAndroidStoreApps](../api/intune_apps_managedandroidstoreapp_list.md)|Коллекция [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md)|Список свойств и связей объектов [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md).|
|[Получение managedAndroidStoreApp](../api/intune_apps_managedandroidstoreapp_get.md)|[managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md)|Считывание свойств и связей объекта [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md).|
|[Создание managedAndroidStoreApp](../api/intune_apps_managedandroidstoreapp_create.md)|[managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md)|Создание нового объекта [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md).|
|[Удаление managedAndroidStoreApp](../api/intune_apps_managedandroidstoreapp_delete.md)|None|Удаляет экземпляр [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md).|
|[Обновление managedAndroidStoreApp](../api/intune_apps_managedandroidstoreapp_update.md)|[managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md)|Обновление свойств объекта [managedAndroidStoreApp](../resources/intune_apps_managedandroidstoreapp.md).|

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
|appAvailability|String|Доступность приложения. Наследуется от [managedApp](../resources/intune_apps_managedapp.md). Допустимые значения: `global`, `lineOfBusiness`.|
|version|String|Версия приложения. Наследуется от [managedApp](../resources/intune_apps_managedapp.md).|
|packageId|String|ИД пакета приложения.|
|appStoreUrl|String|AppStoreUrl для Android.|
|minimumSupportedOperatingSystem|[androidMinimumOperatingSystem](../resources/intune_apps_androidminimumoperatingsystem.md)|Значение, которое представляет минимальную поддерживаемую версию операционной системы.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|categories|Коллекция [mobileAppCategory](../resources/intune_apps_mobileappcategory.md)|Список категорий для этого приложения. Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).|
|assignments|Коллекция [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)|Список назначений группы для этого мобильного приложения. Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAndroidStoreApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
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
  "packageId": "String",
  "appStoreUrl": "String",
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
  }
}
```



