# <a name="targetedmanagedappconfiguration-resource-type"></a>Тип ресурса targetedManagedAppConfiguration

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Конфигурация, используемая для предоставления набора настраиваемых параметров в исходном виде для всех пользователей в целевой группе безопасности.

Наследуется от объекта [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов targetedManagedAppConfiguration](../api/intune_mam_targetedmanagedappconfiguration_list.md)|Коллекция объектов [targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md)|Список свойств и связей объектов [targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md).|
|[Получение объекта targetedManagedAppConfiguration](../api/intune_mam_targetedmanagedappconfiguration_get.md)|[targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md)|Чтение свойств и связей объекта [targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md).|
|[Создание объекта targetedManagedAppConfiguration](../api/intune_mam_targetedmanagedappconfiguration_create.md)|[targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md)|Создание объекта [targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md).|
|[Удаление объекта targetedManagedAppConfiguration](../api/intune_mam_targetedmanagedappconfiguration_delete.md)|Нет|Удаление объекта [targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md).|
|[Обновление объекта targetedManagedAppConfiguration](../api/intune_mam_targetedmanagedappconfiguration_update.md)|[targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md)|Обновление свойств объекта [targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md).|
|[Действие assign](../api/intune_mam_targetedmanagedappconfiguration_assign.md)|Нет|Н/Д|
|[Действие targetApps](../api/intune_mam_targetedmanagedappconfiguration_targetapps.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Отображаемое имя политики. Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|description|Строка|Описание политики. Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|createdDateTime|DateTimeOffset|Дата и время создания политики. Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения политики. Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|id|Строка|Ключ объекта. Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|version|Строка|Версия объекта. Наследуется от объекта [managedAppPolicy](../resources/intune_mam_managedapppolicy.md).|
|customSettings|Коллекция [keyValuePair](../resources/intune_mam_keyvaluepair.md)|Набор строковых пар "ключ-значение", которые отправляются в приложения для пользователей с заданной конфигурацией и не меняются этой службой. Наследуется от объекта [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md).|
|deployedAppCount|Int32|Количество приложений, для которых развернута текущая политика.|
|isAssigned|Логический|Указывает, применена ли политика к группам включения.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|apps|Коллекция [managedMobileApp](../resources/intune_mam_managedmobileapp.md)|Список приложений, к которым применена политика.|
|deploymentSummary|[managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md)|Свойства навигации к сводке по развертыванию конфигурации.|
|assignments|Коллекция [targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md)|Список групп включения и исключения, к которым применяется политика.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.managedAppConfiguration",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.targetedManagedAppConfiguration"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
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
  ],
  "deployedAppCount": 1024,
  "isAssigned": true
}
```








