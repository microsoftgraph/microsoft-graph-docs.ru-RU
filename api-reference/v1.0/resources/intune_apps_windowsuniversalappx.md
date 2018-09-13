# <a name="windowsuniversalappx-resource-type"></a>Тип ресурса windowsUniversalAppX

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Содержит свойства, в том числе унаследованные, для универсальных бизнес-приложений AppX Windows.

Наследуется от [mobileLobApp](../resources/intune_apps_mobilelobapp.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление windowsUniversalAppXs](../api/intune_apps_windowsuniversalappx_list.md)|Коллекция [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md)|Список свойств и связей объектов [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md).|
|[Получение windowsUniversalAppX](../api/intune_apps_windowsuniversalappx_get.md)|[windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md)|Считывание свойств и связей объекта [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md).|
|[Создание windowsUniversalAppX](../api/intune_apps_windowsuniversalappx_create.md)|[windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md)|Создание нового объекта [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md).|
|[Удаление windowsUniversalAppX](../api/intune_apps_windowsuniversalappx_delete.md)|Нет|Удаление экземпляра [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md).|
|[Обновление windowsUniversalAppX](../api/intune_apps_windowsuniversalappx_update.md)|[windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md)|Обновление свойств объекта [windowsUniversalAppX](../resources/intune_apps_windowsuniversalappx.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).|
|displayName|Строка|Название приложения, которое предоставил или импортировал администратор. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).|
|description|Строка|Описание приложения. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).|
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
|committedContentVersion|Строка|Внутренняя версия подтвержденного содержимого. Наследуется от объекта [mobileLobApp](../resources/intune_apps_mobilelobapp.md).|
|fileName|Строка|Имя основного файла бизнес-приложения. Наследуется от объекта [mobileLobApp](../resources/intune_apps_mobilelobapp.md).|
|size|Int64|Общий размер, включая все отправленные файлы. Наследуется от объекта [mobileLobApp](../resources/intune_apps_mobilelobapp.md).|
|applicableArchitectures|[windowsArchitecture](../resources/intune_apps_windowsarchitecture.md)|Архитектура Windows, которая поддерживается этим приложением. Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`.|
|applicableDeviceTypes|[windowsDeviceType](../resources/intune_apps_windowsdevicetype.md)|Типы устройств с Windows, которые поддерживаются этим приложением. Возможные значения: `none`, `desktop`, `mobile`, `holographic`, `team`.|
|identityName|String (строка)|Имя удостоверения.|
|identityPublisherHash|String (строка)|Хэш издателей удостоверений.|
|identityResourceIdentifier|String (строка)|Идентификатор ресурса Identity.|
|isBundle|Boolean (логический)|Указывает, является ли приложение пакетом.|
|minimumSupportedOperatingSystem|[windowsMinimumOperatingSystem](../resources/intune_apps_windowsminimumoperatingsystem.md)|Значение, указывающее минимальную применимую версию операционной системы.|
|identityVersion|String (строка)|Версия удостоверения.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|categories|Коллекция объектов [mobileAppCategory](../resources/intune_apps_mobileappcategory.md)|Список категорий для этого приложения. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).|
|assignments|Коллекция [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)|Список назначений группы для этого мобильного приложения. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).|
|contentVersions|Коллекция объектов [mobileAppContent](../resources/intune_apps_mobileappcontent.md)|Список версий содержимого для этого приложения. Наследуется от [mobileLobApp](../resources/intune_apps_mobilelobapp.md).|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.mobileLobApp",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUniversalAppX"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
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
  "applicableArchitectures": "String",
  "applicableDeviceTypes": "String",
  "identityName": "String",
  "identityPublisherHash": "String",
  "identityResourceIdentifier": "String",
  "isBundle": true,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true
  },
  "identityVersion": "String"
}
```








