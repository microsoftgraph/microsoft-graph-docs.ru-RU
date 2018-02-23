# <a name="devicecategory-resource-type"></a>Тип ресурса deviceCategory

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Категории устройств используются для упорядочивания устройств. Используя категории устройств, администраторы могут определить собственные категории, применимые к их организации. Эти категории затем можно применить к устройству в консоли Azure Intune или выбрать во время регистрации устройства пользователем. На основе категорий устройств вы можете фильтровать отчеты и создавать динамические группы устройств Azure Active Directory.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов deviceCategory](../api/intune_onboarding_devicecategory_list.md)|Коллекция объектов [deviceCategory](../resources/intune_onboarding_devicecategory.md)|Список свойств и связей объектов [deviceCategory](../resources/intune_onboarding_devicecategory.md).|
|[Получение объекта deviceCategory](../api/intune_onboarding_devicecategory_get.md)|[deviceCategory](../resources/intune_onboarding_devicecategory.md)|Чтение свойств и связей объекта [deviceCategory](../resources/intune_onboarding_devicecategory.md).|
|[Создание объекта deviceCategory](../api/intune_onboarding_devicecategory_create.md)|[deviceCategory](../resources/intune_onboarding_devicecategory.md)|Создание объекта [deviceCategory](../resources/intune_onboarding_devicecategory.md).|
|[Удаление объекта deviceCategory](../api/intune_onboarding_devicecategory_delete.md)|Нет|Удаление объекта [deviceCategory](../resources/intune_onboarding_devicecategory.md).|
|[Обновление объекта deviceCategory](../api/intune_onboarding_devicecategory_update.md)|[deviceCategory](../resources/intune_onboarding_devicecategory.md)|Обновление свойств объекта [deviceCategory](../resources/intune_onboarding_devicecategory.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор категории устройства. Только для чтения.|
|displayName|String|Отображаемое имя категории устройств.|
|description|String|Необязательное описание категории устройств.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```



