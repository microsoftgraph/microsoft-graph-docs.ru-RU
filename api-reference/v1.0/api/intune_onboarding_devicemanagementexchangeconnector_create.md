# <a name="create-devicemanagementexchangeconnector"></a>Создание объекта deviceManagementExchangeConnector

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Создание объекта [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md).
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
POST /deviceManagement/exchangeConnectors
```

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Авторизация|&lt;Токен&gt; носителя. Обязательный.|
|Принять|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса добавьте представление объекта deviceManagementExchangeConnector в формате JSON.

Ниже показаны свойства, которые необходимо указывать при создании объекта deviceManagementExchangeConnector.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Н/Д|
|lastSyncDateTime|DateTimeOffset|Время последней синхронизации соединителя Exchange|
|status|String|Состояние соединителя Exchange. Возможные значения: `none`, `connectionPending`, `connected`, `disconnected`.|
|primarySmtpAddress|String|Электронный адрес, используемый для настройки соединителя Exchange между службами.|
|serverName|String|Имя сервера, на котором размещается соединитель Exchange.|
|exchangeConnectorType|String|Тип настраиваемого соединителя Exchange. Возможные значения: `onPremises`, `hosted`, `serviceToService`, `dedicated`.|
|version|String|Версия объекта ExchangeConnectorAgent|
|exchangeAlias|String|Псевдоним, назначенный серверу Exchange Server|
|exchangeOrganization|String|Организация Exchange, соответствующая серверу Exchange Server|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md) в теле ответа.

## <a name="example"></a>Пример
### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/exchangeConnectors
Content-type: application/json
Content-length: 433

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "status": "connectionPending",
  "primarySmtpAddress": "Primary Smtp Address value",
  "serverName": "Server Name value",
  "exchangeConnectorType": "hosted",
  "version": "Version value",
  "exchangeAlias": "Exchange Alias value",
  "exchangeOrganization": "Exchange Organization value"
}
```

### <a name="response"></a>Ответ
Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 482

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
  "id": "e11c1de8-1de8-e11c-e81d-1ce1e81d1ce1",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "status": "connectionPending",
  "primarySmtpAddress": "Primary Smtp Address value",
  "serverName": "Server Name value",
  "exchangeConnectorType": "hosted",
  "version": "Version value",
  "exchangeAlias": "Exchange Alias value",
  "exchangeOrganization": "Exchange Organization value"
}
```



