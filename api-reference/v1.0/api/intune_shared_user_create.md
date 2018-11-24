# <a name="create-user"></a>Создание пользователя

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Создание объекта [user](../resources/intune_shared_user.md).
## <a name="prerequisites"></a>Предварительные условия
Чтобы вызвать этот интерфейс API необходимо одно из следующих разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).  Необходимые разрешения определенного зависит от контекста.

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)| _изменяется в соответствии с контекста_ |
| &nbsp;&nbsp; Управление устройствами | DeviceManagementManagedDevices.ReadWrite.All |
| &nbsp;&nbsp; MAM | DeviceManagementApps.ReadWrite.All |
| &nbsp;&nbsp; Адаптация новых сотрудников | DeviceManagementServiceConfig.ReadWrite.All |
| &nbsp;&nbsp; Устранение неполадок | DeviceManagementManagedDevices.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Authorization|Требуется Bearer &lt;маркер&gt;
|
|Accept|application/json|

## <a name="request-body"></a>Тело запроса
В теле запроса добавьте представление объекта user в формате JSON.

В приведенной ниже таблице указаны свойства, необходимые при создании объекта user.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор пользователя.|
|**Адаптация новых сотрудников**|
|deviceEnrollmentLimit|Int32|Максимальное количество устройств, которые разрешено зарегистрировать пользователю. Допустимые значения: 5 или 1000.|

Поддержка свойств текст запроса изменяется в зависимости от контекста.

## <a name="response"></a>Отклик
При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [user](../resources/intune_shared_user.md) в теле отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.

``` http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a>Ответ
Ниже приведен пример отклика. Примечание. Представленный здесь объект отклика может быть усечен для краткости. Свойства, возвращенные фактический вызов различаться в зависимости от контекста.

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



