# <a name="targetedmanagedapppolicyassignment-resource-type"></a>Тип ресурса targetedManagedAppPolicyAssignment

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Тип развертывания групп или приложений.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов targetedManagedAppPolicyAssignment](../api/intune_mam_targetedmanagedapppolicyassignment_list.md)|Коллекция [targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md)|Список свойств и связей объектов [targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md).|
|[Получение объекта targetedManagedAppPolicyAssignment](../api/intune_mam_targetedmanagedapppolicyassignment_get.md)|[targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md)|Чтение свойств и связей объекта [targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md).|
|[Удаление объекта targetedManagedAppPolicyAssignment](../api/intune_mam_targetedmanagedapppolicyassignment_delete.md)|Нет|Удаляет объект [targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md).|
|[Обновление объекта targetedManagedAppPolicyAssignment](../api/intune_mam_targetedmanagedapppolicyassignment_update.md)|[targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md)|Обновление свойств объекта [targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|string|ИД|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|Идентификатор для развертывания группы или приложения|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.targetedManagedAppPolicyAssignment"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```
