# <a name="mobileapp-resource-type"></a>Тип ресурса mobileApp

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Абстрактный класс, содержащий базовые свойства мобильных приложений Intune.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список mobileApps](../api/intune_apps_mobileapp_list.md)|Коллекция [mobileApp](../resources/intune_apps_mobileapp.md)|Список свойств и связей объектов [mobileApp](../resources/intune_apps_mobileapp.md).|
|[Получение объекта mobileApp](../api/intune_apps_mobileapp_get.md)|[mobileApp](../resources/intune_apps_mobileapp.md)|Чтение свойств и связей объекта [mobileApp](../resources/intune_apps_mobileapp.md).|
|[assign action](../api/intune_apps_mobileapp_assign.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|displayName|Строка|Администратор предоставил или импортировал название приложения.|
|description|Строка|Описание приложения.|
|publisher|Строка|Издатель приложения.|
|largeIcon|[mimeContent](../resources/intune_shared_mimecontent.md)|Большой значок, отображается в сведениях о приложении и используется для отправки значка.|
|createdDateTime|DateTimeOffset|Дата и время создания приложения.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения приложения.|
|isFeatured|Логический|Значение, которое показывает, отмечено ли приложение как подобранное администратором.|
|privacyInformationUrl|Строка|URL-адрес заявления о конфиденциальности.|
|informationUrl|Строка|URL-адрес с дополнительными сведениями.|
|owner|Строка|Владелец приложения.|
|developer|Строка|Разработчик приложения.|
|notes|Строка|Заметки для приложения.|
|publishingState|[mobileAppPublishingState](../resources/intune_apps_mobileapppublishingstate.md)|Состояние публикации приложения. Приложение невозможно назначить, если оно не опубликовано. Возможные значения: `notPublished`, `processing`, `published`.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|categories|Коллекция объектов [mobileAppCategory](../resources/intune_apps_mobileappcategory.md)|Список категорий для этого приложения.|
|assignments|Коллекция [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)|Список назначений группы для этого мобильного приложения.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "abstract": true,
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.mobileApp"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileApp",
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
  "publishingState": "String"
}
```



