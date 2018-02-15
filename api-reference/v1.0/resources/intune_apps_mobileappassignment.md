# <a name="mobileappassignment-resource-type"></a>Тип ресурса mobileAppAssignment

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Класс, содержащий свойства, которые используются для назначения групп в мобильном приложении.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов mobileAppAssignment](../api/intune_apps_mobileappassignment_list.md)|Коллекция [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)|Список свойств и связей объектов [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md).|
|[Получение объекта mobileAppAssignment](../api/intune_apps_mobileappassignment_get.md)|[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)|Чтение свойств и связей объекта [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md).|
|[Создание объекта mobileAppAssignment](../api/intune_apps_mobileappassignment_create.md)|[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)|Создание объекта [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md).|
|[Удаление объекта mobileAppAssignment](../api/intune_apps_mobileappassignment_delete.md)|Нет|Удаляет объект [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md).|
|[Обновление объекта mobileAppAssignment](../api/intune_apps_mobileappassignment_update.md)|[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md)|Обновление свойств объекта [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|intent|String|Цель установки, определенная администратором. Возможные значения: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune_apps_deviceandappmanagementassignmenttarget.md)|Целевое назначение группы, определенное администратором.|
|settings|[mobileAppAssignmentSettings](../resources/intune_apps_mobileappassignmentsettings.md)|Параметры целевого назначения, определенные администратором.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppAssignment",
  "id": "String (identifier)",
  "intent": "String",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "settings": {
    "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
  }
}
```



