# <a name="managedappconfiguration-resource-type"></a>Тип ресурса managedAppConfiguration

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Конфигурация, используемая для доставки набора пользовательских настроек (без изменений) в приложение тех пользователей, для которых задана конфигурация

Наследуется от [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список managedAppConfigurations](../api/intune_mam_managedappconfiguration_list.md)|Коллекция [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md)|Список свойств и связей объектов [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md).|
|[Получение объекта managedAppConfiguration](../api/intune_mam_managedappconfiguration_get.md)|[managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md)|Чтение свойств и связей объекта [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Отображаемое имя политики. Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|description|String|Описание политики. Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|createdDateTime|DateTimeOffset|Дата и время создания политики. Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения политики. Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|id|Строка|Ключ объекта. Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|version|String|Версия объекта. Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|customSettings|Коллекция [keyValuePair](../resources/intune_mam_keyvaluepair.md)|Набор, состоящий из пар ключа и значения строки, которые отправляются в приложение для пользователей с заданной конфигурацией и не меняются этой службой|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "abstract": true,
  "keyProperty": "id",
  "baseType": "microsoft.graph.managedAppPolicy",
  "@odata.type": "microsoft.graph.managedAppConfiguration"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppConfiguration",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "version": "String",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ]
}
```



