# <a name="devicemanagementpartner-resource-type"></a>Тип ресурса deviceManagementPartner

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Объект, представляющий подключение к партнеру по управлению устройствами.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов deviceManagementPartner](../api/intune_onboarding_devicemanagementpartner_list.md)|Коллекция [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md)|Список свойств и связей объектов [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md).|
|[Получение объекта deviceManagementPartner](../api/intune_onboarding_devicemanagementpartner_get.md)|[deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md)|Чтение свойств и связей объекта [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md).|
|[Создание объекта deviceManagementPartner](../api/intune_onboarding_devicemanagementpartner_create.md)|[deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md)|Создание объекта [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md).|
|[Удаление объекта deviceManagementPartner](../api/intune_onboarding_devicemanagementpartner_delete.md)|Нет|Удаляет объект [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md).|
|[Обновление объекта deviceManagementPartner](../api/intune_onboarding_devicemanagementpartner_update.md)|[deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md)|Обновление свойств объекта [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Н/Д|
|lastHeartbeatDateTime|DateTimeOffset|Метка времени последнего пульса после того, как администратор включил параметр "Подключиться к партнеру по управлению устройствами".|
|partnerState|[deviceManagementPartnerTenantState](../resources/intune_onboarding_devicemanagementpartnertenantstate.md)|Состояние партнера этого клиента. Возможные значения: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.|
|partnerAppType|[deviceManagementPartnerAppType](../resources/intune_onboarding_devicemanagementpartnerapptype.md)|Тип приложения партнера. Возможные значения: `unknown`, `singleTenantApp`, `multiTenantApp`.|
|singleTenantAppId|Строка|Идентификатор одноклиентского приложения партнера|
|displayName|Строка|Отображаемое имя партнера|
|isConfigured|Логическое|Указывает, настроен ли партнер по управлению устройствами|
|whenPartnerDevicesWillBeRemovedDateTime|DateTimeOffset|Дата и время в формате UTC, указывающие, когда будут удалены партнерские устройства.|
|whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime|DateTimeOffset|Дата и время в формате UTC, указывающие, когда партнерские устройства будут отмечены как несоответствующие требованиям|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementPartner"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "id": "String (identifier)",
  "lastHeartbeatDateTime": "String (timestamp)",
  "partnerState": "String",
  "partnerAppType": "String",
  "singleTenantAppId": "String",
  "displayName": "String",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemovedDateTime": "String (timestamp)",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "String (timestamp)"
}
```








