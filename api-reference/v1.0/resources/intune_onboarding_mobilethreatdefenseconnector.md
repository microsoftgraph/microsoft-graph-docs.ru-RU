# <a name="mobilethreatdefenseconnector-resource-type"></a>Тип ресурса mobileThreatDefenseConnector

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Объект, представляющий подключение к партнеру по Mobile Threat Defense.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список mobileThreatDefenseConnectors](../api/intune_onboarding_mobilethreatdefenseconnector_list.md)|Коллекция [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md)|Список свойств и связей объектов [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md).|
|[Получение объекта mobileThreatDefenseConnector](../api/intune_onboarding_mobilethreatdefenseconnector_get.md)|[mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md)|Чтение свойств и связей объекта [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md).|
|[Создание объекта mobileThreatDefenseConnector](../api/intune_onboarding_mobilethreatdefenseconnector_create.md)|[mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md)|Создание объекта [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md).|
|[Удаление объекта mobileThreatDefenseConnector](../api/intune_onboarding_mobilethreatdefenseconnector_delete.md)|Нет|Удаляет объект [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md).|
|[Обновление объекта mobileThreatDefenseConnector](../api/intune_onboarding_mobilethreatdefenseconnector_update.md)|[mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md)|Обновление свойств объекта [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Н/Д|
|lastHeartbeatDateTime|DateTimeOffset|Метка времени последнего полученного пакета пульса после того, как администратор включил параметр "Подключиться к MTP"|
|partnerState|String|Состояние партнера этого клиента. Возможные значения: `unavailable`, `available`, `enabled`, `unresponsive`.|
|androidEnabled|Boolean|Включение или отключение Android|
|androidDeviceBlockedOnMissingPartnerData|Boolean|Для Android. Позволяет администратору настроить получение обязательных данных от партнера по синхронизации перед предоставлением соответствия требованиям|
|iosDeviceBlockedOnMissingPartnerData|Boolean|Для IOS. Позволяет администратору настроить получение обязательных данных от партнера по синхронизации перед предоставлением соответствия требованиям|
|partnerUnsupportedOsVersionBlocked|Boolean|Позволяет администратору блокировать на включенных платформах устройства, несоответствующие минимальным требованиям версии|
|iosEnabled|Boolean|Включение и отключение IOS|
|partnerUnresponsivenessThresholdInDays|Int32|Получает или задает количество дней, в течение которых клиент устойчив к отсутствию ответа для интеграции партнера|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileThreatDefenseConnector"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "id": "String (identifier)",
  "lastHeartbeatDateTime": "String (timestamp)",
  "partnerState": "String",
  "androidEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "iosEnabled": true,
  "partnerUnresponsivenessThresholdInDays": 1024
}
```



