# <a name="list-devicecompliancepolicystates"></a>Перечисление объектов deviceCompliancePolicyState

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Список свойств и связей объектов [deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md).
## <a name="prerequisites"></a>Предварительные условия
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /managedDevices/{managedDevicesId}/deviceCompliancePolicyStates
```

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
Не указывайте тело запроса для этого метода.

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [deviceCompliancePolicyState](../resources/intune_deviceconfig_devicecompliancepolicystate.md) в тексте отклика.

## <a name="example"></a>Пример
### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
GET https://graph.microsoft.com/v1.0/managedDevices/{managedDevicesId}/deviceCompliancePolicyStates
```

### <a name="response"></a>Ответ
Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1175

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceCompliancePolicyState",
      "id": "2999e387-e387-2999-87e3-992987e39929",
      "settingStates": [
        {
          "@odata.type": "microsoft.graph.deviceCompliancePolicySettingState",
          "setting": "Setting value",
          "settingName": "Setting Name value",
          "instanceDisplayName": "Instance Display Name value",
          "state": "notApplicable",
          "errorCode": 9,
          "errorDescription": "Error Description value",
          "userId": "User Id value",
          "userName": "User Name value",
          "userEmail": "User Email value",
          "userPrincipalName": "User Principal Name value",
          "sources": [
            {
              "@odata.type": "microsoft.graph.settingSource",
              "id": "Id value",
              "displayName": "Display Name value"
            }
          ],
          "currentValue": "Current Value value"
        }
      ],
      "displayName": "Display Name value",
      "version": 7,
      "platformType": "iOS",
      "state": "notApplicable",
      "settingCount": 12
    }
  ]
}
```



