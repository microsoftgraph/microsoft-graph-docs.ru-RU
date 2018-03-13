# <a name="update-mobilethreatdefenseconnector"></a>Обновление mobileThreatDefenseConnector

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Обновление свойств объекта [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md).
## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementServiceConfig.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Тело запроса
В теле запроса добавьте представление объекта [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) в формате JSON.

В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Пока не задокументировано|
|lastHeartbeatDateTime|DateTimeOffset|Метка времени последнего полученного пакета пульса после того, как администратор включил параметр "Подключиться к MTP"|
|partnerState|String|Состояние партнера этого клиента. Возможные значения: `unavailable`, `available`, `enabled`, `unresponsive`.|
|androidEnabled|Boolean|Включение или отключение Android|
|androidDeviceBlockedOnMissingPartnerData|Boolean|Для Android. Позволяет администратору настроить получение обязательных данных от партнера по синхронизации перед подтверждением соответствия требованиям|
|iosDeviceBlockedOnMissingPartnerData|Boolean|Для IOS. Позволяет администратору настроить получение обязательных данных от партнера по синхронизации перед подтверждением соответствия требованиям|
|partnerUnsupportedOsVersionBlocked|Boolean|Позволяет администратору блокировать на включенных платформах устройства, несоответствующие минимальным требованиям для версии|
|iosEnabled|Boolean|Включение и отключение IOS|
|partnerUnresponsivenessThresholdInDays|Int32|Получает или задает количество дней устойчивости к отсутствию отклика для клиента в случае интеграции партнера|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) в теле отклика.

## <a name="example"></a>Пример
### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
Content-type: application/json
Content-length: 347

{
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "iosEnabled": true,
  "partnerUnresponsivenessThresholdInDays": 6
}
```

### <a name="response"></a>Ответ
Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 463

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "id": "e4bede14-de14-e4be-14de-bee414debee4",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "iosEnabled": true,
  "partnerUnresponsivenessThresholdInDays": 6
}
```



