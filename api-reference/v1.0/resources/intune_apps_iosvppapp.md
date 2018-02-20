# <a name="iosvppapp-resource-type"></a>Тип ресурса iosVppApp

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Содержит свойства, в том числе унаследованные, для приложений iOS, на которые распространяется программа VPP (Volume Purchase Program).

Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление iosVppApps](../api/intune_apps_iosvppapp_list.md)|Коллекция [iosVppApp](../resources/intune_apps_iosvppapp.md)|Список свойств и связей объектов [iosVppApp](../resources/intune_apps_iosvppapp.md).|
|[Получение iosVppApp](../api/intune_apps_iosvppapp_get.md)|[iosVppApp](../resources/intune_apps_iosvppapp.md)|Считывание свойств и связей объекта [iosVppApp](../resources/intune_apps_iosvppapp.md).|
|[Создание iosVppApp](../api/intune_apps_iosvppapp_create.md)|[iosVppApp](../resources/intune_apps_iosvppapp.md)|Создание нового объекта [iosVppApp](../resources/intune_apps_iosvppapp.md).|
|[Удаление iosVppApp](../api/intune_apps_iosvppapp_delete.md)|None|Удаление экземпляра [iosVppApp](../resources/intune_apps_iosvppapp.md).|
|[Обновление iosVppApp](../api/intune_apps_iosvppapp_update.md)|[iosVppApp](../resources/intune_apps_iosvppapp.md)|Обновление свойств объекта [iosVppApp](../resources/intune_apps_iosvppapp.md).|

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
|usedLicenseCount|Int32|Количество используемых лицензий VPP.|
|totalLicenseCount|Int32|Общее количество лицензий VPP.|
|releaseDateTime|DateTimeOffset|Дата и время выпуска приложения, на которое распространяется программа VPP.|
|appStoreUrl|String|URL-адрес магазина.|
|licensingType|[vppLicensingType](../resources/intune_apps_vpplicensingtype.md)|Поддерживаемый тип лицензии.|
|applicableDeviceType|[iosDeviceType](../resources/intune_apps_iosdevicetype.md)|Применимый тип устройства с iOS.|
|vppTokenOrganizationName|String|Организация, связанная с токеном Apple Volume Purchase Program.|
|vppTokenAccountType|String|Тип программы оптовых покупок, с которой связан заданный токен Apple Volume Purchase Program. Возможные значения: `business`, `education`. Возможные значения: `business`, `education`.|
|vppTokenAppleId|String|Идентификатор Apple ID, связанный с заданным токеном Apple Volume Purchase Program.|
|bundleId|String|Имя удостоверения.|

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
  "@odata.type": "microsoft.graph.iosVppApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppApp",
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
  "usedLicenseCount": 1024,
  "totalLicenseCount": 1024,
  "releaseDateTime": "String (timestamp)",
  "appStoreUrl": "String",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "String",
  "vppTokenAccountType": "String",
  "vppTokenAppleId": "String",
  "bundleId": "String"
}
```



