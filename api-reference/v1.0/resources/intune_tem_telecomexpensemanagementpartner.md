# <a name="telecomexpensemanagementpartner-resource-type"></a>Тип ресурса telecomExpenseManagementPartner

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Ресурсы telecomExpenseManagementPartner представляют метаданные и сведения о состоянии определенной службы TEM. После подключения партнера к вашей организации вы можете разрешить или запретить ему включать и отключать функции TEM.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов telecomExpenseManagementPartners](../api/intune_tem_telecomexpensemanagementpartner_list.md)|Коллекция [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md)|Список свойств и связей объектов [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md).|
|[Получение объекта telecomExpenseManagementPartner](../api/intune_tem_telecomexpensemanagementpartner_get.md)|[telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md)|Чтение свойств и связей объекта [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md).|
|[Создание объекта telecomExpenseManagementPartner](../api/intune_tem_telecomexpensemanagementpartner_create.md)|[telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md)|Создание объекта [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md).|
|[Удаление объекта telecomExpenseManagementPartner](../api/intune_tem_telecomexpensemanagementpartner_delete.md)|Нет|Удаляет объект [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md).|
|[Обновление объекта telecomExpenseManagementPartner](../api/intune_tem_telecomexpensemanagementpartner_update.md)|[telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md)|Обновление свойств объекта [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор партнера TEM.|
|displayName|String|Отображаемое имя партнера TEM.|
|url|String|URL-адрес административной панели управления партнера TEM, где можно настроить службу TEM.|
|appAuthorized|Boolean|Определяет, авторизозвано ли партнерское приложение AAD на доступ к Intune.|
|enabled|Boolean|Определяет, включено или отключено подключение Intune к службе TEM в настоящее время.|
|lastConnectionDateTime|DateTimeOffset|Метка времени последнего запроса, отправленного службе Intune партнером TEM.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.telecomExpenseManagementPartner"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
  "id": "String (identifier)",
  "displayName": "String",
  "url": "String",
  "appAuthorized": true,
  "enabled": true,
  "lastConnectionDateTime": "String (timestamp)"
}
```



