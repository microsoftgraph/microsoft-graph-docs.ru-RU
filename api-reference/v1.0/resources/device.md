# <a name="device-resource-type"></a>Тип ресурса device

Представляет устройство, зарегистрированное в организации. Экземпляры device могут создаваться в облаке с помощью службы Device Registration Service или Intune. Их используют политики условного доступа для многофакторной проверки подлинности. Представленными устройствами могут быть компьютеры и ноутбуки, смартфоны и планшеты. Наследуется из [directoryObject](directoryobject.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Создание устройства](../api/device_post_devices.md) | [device](device.md) |Регистрация нового устройства в каталоге.|
|[Получение device](../api/device_get.md) | [device](device.md) |Считывание свойств и отношений объекта device.|
|[Список объектов device](../api/device_list.md) | Коллекция [device](device.md)| Получение списка устройств, зарегистрированных в каталоге. |
|[Обновление device](../api/device_update.md) | [device](device.md) |Обновление свойств, принадлежащих объекту device. |
|[Удаление device](../api/device_delete.md) | Нет |Удаление объекта device. |
|[Создание registeredOwner](../api/device_post_registeredowners.md) |[directoryObject](directoryobject.md)| Добавление пользователя в качестве нового владельца устройства путем записи данных в свойство навигации registeredOwners.|
|[Список экземпляров registeredOwner](../api/device_list_registeredowners.md) |Коллекция [directoryObject](directoryobject.md)| Получение пользователей, которые относятся к зарегистрированным владельцам устройства, из свойства навигации registeredOwners.|
|[Создание экземпляра registeredUser](../api/device_post_registeredusers.md) |[directoryObject](directoryobject.md)| Добавление зарегистрированного пользователя устройства путем записи данных в свойство навигации registeredUsers.|
|[Список экземпляров registeredUser](../api/device_list_registeredusers.md) |Коллекция [directoryObject](directoryobject.md)| Получение зарегистрированных пользователей устройства из свойства навигации registeredUsers.|

## <a name="properties"></a>Свойства
| Свойство       | Тип    |Описание|
|:---------------|:--------|:----------|
|accountEnabled|Логическое| Если учетная запись обеспечена — значение **true**, в противном случае — **false**. Обязательный параметр.|
|alternativeSecurityIds|Коллекция [alternativeSecurityId](alternativesecurityid.md)| Для выражений фильтра для свойств с несколькими значениями требуется оператор **any**. Значение null не допускается. Обязательный параметр. |
|approximateLastSignInDateTime|DateTimeOffset| Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|deviceId|Guid| Уникальный идентификатор GUID клиента, представляющий устройство. Обязательный параметр. |
|deviceMetadata|String|    |
|deviceVersion|Int32|            |
|displayName|String|Отображаемое имя устройства. Обязательный параметр. |
|id|Строка|Уникальный идентификатор устройства. Наследуется из [directoryObject](directoryobject.md). Ключ, значение null не допускается. Только для чтения.|
|isCompliant|Boolean|Используется значение **true**, если устройство соответствует требованиям политик управления мобильными устройствами (MDM). В противном случае используется значение **false**.|
|isManaged|Boolean|Используется значение **true**, если устройство контролируется приложением для управления мобильными устройствами (MDM), например Intune. В противном случае используется значение **false**.|
|onPremisesLastSyncDateTime|DateTimeOffset|Время последней синхронизации объекта с локальным каталогом. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (время всегда в формате UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|onPremisesSyncEnabled|Boolean|Используется значение **true**, если этот объект синхронизируется из локального каталога. Используется значение **false**, если этот объект ранее синхронизировался из локального каталога, но синхронизация больше не выполняется. Используется значение **null**, если этот объект никогда не синхронизировался из локального каталога (значение по умолчанию).|
|operatingSystem|String|Тип операционной системы на устройстве. Обязательный параметр. |
|operatingSystemVersion|Строка|Версия операционной системы на устройстве. Обязательный параметр. |
|physicalIds|Коллекция String| Значение null не допускается.            |
|trustType|String|    ||

## <a name="relationships"></a>Отношения
| Связь | Тип    |Описание|
|:---------------|:--------|:----------|
|registeredOwners|Коллекция [directoryObject](directoryobject.md)|Пользователи, относящиеся к зарегистрированным владельцам устройства. Только для чтения. Допускается значение null.|
|registeredUsers|Коллекция [directoryObject](directoryobject.md)|Зарегистрированные пользователи устройства. Только для чтения. Допускается значение null.|



## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "registeredOwners",
    "registeredUsers"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.device"
}-->

```json
{
  "accountEnabled": true,
  "alternativeSecurityIds": [{"@odata.type": "microsoft.graph.alternativeSecurityId"}],
  "approximateLastSignInDateTime": "String (timestamp)",
  "deviceId": "string",
  "deviceMetadata": "string",
  "deviceVersion": 1024,
  "displayName": "string",
  "id": "string (identifier)",
  "isCompliant": true,
  "isManaged": true,
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesSyncEnabled": true,
  "operatingSystem": "string",
  "operatingSystemVersion": "string",
  "physicalIds": ["string"],
  "trustType": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "device resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
