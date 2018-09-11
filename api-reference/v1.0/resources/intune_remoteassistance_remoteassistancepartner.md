# <a name="remoteassistancepartner-resource-type"></a>Тип ресурса remoteAssistancePartner

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Ресурсы remoteAssistPartner представляются метаданные и состояние определенной партнерской службы удаленного помощника.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов remoteAssistancePartner](../api/intune_remoteassistance_remoteassistancepartner_list.md)|Коллекция [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md)|Список свойств и связей объектов [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md).|
|[Получение объекта remoteAssistancePartner](../api/intune_remoteassistance_remoteassistancepartner_get.md)|[remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md)|Чтение свойств и связей объекта [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md).|
|[Создание объекта remoteAssistancePartner](../api/intune_remoteassistance_remoteassistancepartner_create.md)|[remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md)|Создание объекта [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md).|
|[Удаление объекта remoteAssistancePartner](../api/intune_remoteassistance_remoteassistancepartner_delete.md)|Нет|Удаляет объект [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md).|
|[Обновление объекта remoteAssistancePartner](../api/intune_remoteassistance_remoteassistancepartner_update.md)|[remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md)|Обновление свойств объекта [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md).|
|[Действие beginOnboarding](../api/intune_remoteassistance_remoteassistancepartner_beginonboarding.md)|Нет|Н/Д|
|[Действие disconnect](../api/intune_remoteassistance_remoteassistancepartner_disconnect.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор партнера.|
|displayName|String|Отображаемое имя партнера.|
|onboardingUrl|String|URL-адрес портала подключения партнера, где администратор может настроить свою службу удаленного помощника.|
|onboardingStatus|[remoteAssistanceOnboardingStatus](../resources/intune_remoteassistance_remoteassistanceonboardingstatus.md)|Подлежит определению. Возможные значения: `notOnboarded`, `onboarding`, `onboarded`.|
|lastConnectionDateTime|DateTimeOffset|Метка времени последнего запроса, отправленного службе Intune партнером TEM.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.remoteAssistancePartner"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "id": "String (identifier)",
  "displayName": "String",
  "onboardingUrl": "String",
  "onboardingStatus": "String",
  "lastConnectionDateTime": "String (timestamp)"
}
```








