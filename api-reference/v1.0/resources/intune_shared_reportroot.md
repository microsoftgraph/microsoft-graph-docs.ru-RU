# <a name="reportroot-resource-type"></a>Тип ресурса reportRoot

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Ресурс, представляющий экземпляр отчетов журнала.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение объекта reportRoot](../api/intune_shared_reportroot_get.md)|[reportRoot](../resources/intune_shared_reportroot.md)|Чтение свойств и связей объекта [reportRoot](../resources/intune_shared_reportroot.md).|
|[Обновление объекта reportRoot](../api/intune_shared_reportroot_update.md)|[reportRoot](../resources/intune_shared_reportroot.md)|Обновление свойств объекта [reportRoot](../resources/intune_shared_reportroot.md).|
|**Конфигурация устройства**|
|[Функция deviceConfigurationDeviceActivity](../api/intune_shared_reportroot_deviceconfigurationdeviceactivity.md)|[report](../resources/intune_shared_report.md)|Метаданные для отчета о действиях устройств с конфигурацией устройств|
|[Функция deviceConfigurationUserActivity](../api/intune_shared_reportroot_deviceconfigurationuseractivity.md)|[report](../resources/intune_shared_report.md)|Метаданные для отчета о действиях пользователей с конфигурацией устройств|
|**Устранение неполадок**|
|[Функция managedDeviceEnrollmentFailureDetails](../api/intune_shared_reportroot_manageddeviceenrollmentfailuredetails.md)|[report](../resources/intune_shared_report.md)|Еще не задокументировано|
|[Функция managedDeviceEnrollmentTopFailures](../api/intune_shared_reportroot_manageddeviceenrollmenttopfailures.md)|[report](../resources/intune_shared_report.md)|Еще не задокументировано|


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для этого объекта.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.reportRoot"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "String (identifier)"
}
```

## <a name="example"></a>Пример

<!--{"blockType": "request"}-->
```http
GET https://graph.microsoft.com/v1.0/reports
```

<!--{"blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.reportRoot"}-->
```json
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```