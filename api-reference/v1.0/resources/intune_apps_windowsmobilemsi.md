# <a name="windowsmobilemsi-resource-type"></a>Тип ресурса windowsMobileMSI

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Содержит свойства, в том числе унаследованные, для бизнес-приложений, к которым применяется MSI Windows Mobile.

Наследуется от [mobileLobApp](../resources/intune_apps_mobilelobapp.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление windowsMobileMSIs](../api/intune_apps_windowsmobilemsi_list.md)|Коллекция [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md)|Список свойств и связей объектов [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md).|
|[Получение windowsMobileMSI](../api/intune_apps_windowsmobilemsi_get.md)|[windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md)|Считывание свойств и связей объекта [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md).|
|[Создание windowsMobileMSI](../api/intune_apps_windowsmobilemsi_create.md)|[windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md)|Создание объекта [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md).|
|[Удаление windowsMobileMSI](../api/intune_apps_windowsmobilemsi_delete.md)|Нет|Удаление экземпляра [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md).|
|[Обновление windowsMobileMSI](../api/intune_apps_windowsmobilemsi_update.md)|[windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md)|Обновление свойств объекта [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md).|

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
|publishingState|[mobileAppPublishingState](../resources/intune_apps_mobileapppublishingstate.md)|Состояние публикации для приложения. Приложение невозможно назначить, если оно не опубликовано. Наследуется от [mobileApp](../resources/intune_apps_mobileapp.md). Возможные значения: `notPublished`, `processing`, `published`.|
|committedContentVersion|String (строка)|Внутренняя версия подтвержденного содержимого. Наследуется от объекта [mobileLobApp](../resources/intune_apps_mobilelobapp.md).|
|fileName|String (строка)|Имя основного файла бизнес-приложения. Наследуется от объекта [mobileLobApp](../resources/intune_apps_mobilelobapp.md).|
|size|Int64|Общий размер, включая все отправленные файлы. Наследуется от объекта [mobileLobApp](../resources/intune_apps_mobilelobapp.md).|
|commandLine|String (строка)|Командная строка.|
|productCode|String (строка)|Код продукта.|
|productVersion|String (строка)|Версия бизнес-приложения MSI Windows Mobile.|
|ignoreVersionDetection|Boolean (логический)|Логическое значение, позволяющее разрешить или запретить поиск приложения по его версии после установки на устройстве. Задайте значение true для бизнес-приложений, к которым применяется MSI Windows Mobile и функция самостоятельного обновления.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|категории|Коллекция объектов [mobileAppCategory](../resources/intune_apps_mobileappcategory.md)|Список категорий для этого приложения. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).|
|назначения|Коллекция [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)|Список назначений группы для этого мобильного приложения. Наследуется от объекта [mobileApp](../resources/intune_apps_mobileapp.md).|
|contentVersions|Коллекция объектов [mobileAppContent](../resources/intune_apps_mobileappcontent.md)|Список версий содержимого для этого приложения. Наследуется от [mobileLobApp](../resources/intune_apps_mobilelobapp.md).|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.mobileLobApp",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsMobileMSI"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
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
  "commandLine": "String",
  "productCode": "String",
  "productVersion": "String",
  "ignoreVersionDetection": true
}
```








