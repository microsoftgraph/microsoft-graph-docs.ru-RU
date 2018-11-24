# <a name="managedapppolicy-resource-type"></a>Тип ресурса managedAppPolicy

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Ресурс ManagedAppPolicy представляет базовый тип политик для определенных платформ.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов managedAppPolicy](../api/intune_mam_managedapppolicy_list.md)|Коллекция [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|Список свойств и связей объектов [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|[Получение объекта managedAppPolicy](../api/intune_mam_managedapppolicy_get.md)|[managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|Чтение свойств и связей объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|[Действие targetApps](../api/intune_mam_managedapppolicy_targetapps.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Отображаемое имя политики.|
|description|String|Описание политики.|
|createdDateTime|DateTimeOffset|Дата и время создания политики.|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения политики.|
|id|String|Ключ объекта.|
|version|String|Версия объекта.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppPolicy",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "version": "String"
}
```



