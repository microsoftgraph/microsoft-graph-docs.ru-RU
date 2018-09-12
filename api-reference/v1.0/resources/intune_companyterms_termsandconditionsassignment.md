# <a name="termsandconditionsassignment-resource-type"></a>Тип ресурса termsAndConditionsAssignment

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Объект termsAndConditionsAssignment представляет назначение определенной политики условий заданной группе. Чтобы зарегистрировать устройства в Intune, пользователям в группе необходимо принять условия.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список termsAndConditionsAssignments](../api/intune_companyterms_termsandconditionsassignment_list.md)|Коллекция [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md)|Список свойств и связей объектов [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md).|
|[Получение объекта termsAndConditionsAssignment](../api/intune_companyterms_termsandconditionsassignment_get.md)|[termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md)|Чтение свойств и связей объекта [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md).|
|[Создание объекта termsAndConditionsAssignment](../api/intune_companyterms_termsandconditionsassignment_create.md)|[termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md)|Создание объекта [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md).|
|[Удаление объекта termsAndConditionsAssignment](../api/intune_companyterms_termsandconditionsassignment_delete.md)|Нет|Удаляет объект [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md).|
|[Обновление объекта termsAndConditionsAssignment](../api/intune_companyterms_termsandconditionsassignment_update.md)|[termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md)|Удаление свойств объекта [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String (строка)|Уникальный идентификатор объекта.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|Объект, для которого назначается политика соблюдения условий.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditionsAssignment"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```








