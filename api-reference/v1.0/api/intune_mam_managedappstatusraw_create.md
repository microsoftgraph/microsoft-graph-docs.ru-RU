# <a name="create-managedappstatusraw"></a>Создание объекта managedAppStatusRaw

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Создание объекта [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md).
## <a name="prerequisites"></a>Предварительные условия
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementApps.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppStatuses
```

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Тело запроса
В теле запроса добавьте представление объекта managedAppStatusRaw в формате JSON.

В приведенной ниже таблице указаны свойства, необходимые при создании объекта managedAppStatusRaw.

|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Понятное имя отчета о состоянии. Наследуется от объекта [managedAppStatus](../resources/intune_mam_managedappstatus.md).|
|id|String|Ключ объекта. Наследуется от объекта [managedAppStatus](../resources/intune_mam_managedappstatus.md).|
|version|String|Версия объекта. Наследуется от объекта [managedAppStatus](../resources/intune_mam_managedappstatus.md).|
|content|[Json](../resources/intune_mam_json.md)|Содержимое отчета о состоянии.|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) в теле отклика.

## <a name="example"></a>Пример
### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppStatuses
Content-type: application/json
Content-length: 197

{
  "@odata.type": "#microsoft.graph.managedAppStatusRaw",
  "displayName": "Display Name value",
  "version": "Version value",
  "content": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

### <a name="response"></a>Ответ
Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 246

{
  "@odata.type": "#microsoft.graph.managedAppStatusRaw",
  "displayName": "Display Name value",
  "id": "80847581-7581-8084-8175-848081758480",
  "version": "Version value",
  "content": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```



