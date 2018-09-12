# <a name="vpptoken-resource-type"></a>Тип ресурса vppToken

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Вы приобрели несколько лицензий для приложений для iOS по программе корпоративных покупок Apple Volume Purchase Program для бизнеса или образовательных учреждений. Это включает настройку учетной записи Apple VPP с веб-сайта Apple и передачу токена Apple VPP для бизнеса или образовательных учреждений в Intune. Затем вы можете синхронизировать данные корпоративных покупок с помощью Intune и отслеживать использование приложения, приобретенного по программе корпоративных покупок. Вы можете передать несколько токенов Apple VPP для бизнеса или образовательных учреждений.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список VPP токенов](../api/intune_onboarding_vpptoken_list.md)|Коллекция [VPP токенов](../resources/intune_onboarding_vpptoken.md)|Список свойств и связей объектов [VPP токен](../resources/intune_onboarding_vpptoken.md).|
|[Получить VPP токен](../api/intune_onboarding_vpptoken_get.md)|[VPP токен](../resources/intune_onboarding_vpptoken.md)|Чтение свойств и связей объекта [VPP токен](../resources/intune_onboarding_vpptoken.md).|
|[Создать VPP токен](../api/intune_onboarding_vpptoken_create.md)|[VPP токен](../resources/intune_onboarding_vpptoken.md)|Создайте новый объект [VPP токен](../resources/intune_onboarding_vpptoken.md).|
|[Удалить VPP токен](../api/intune_onboarding_vpptoken_delete.md)|Отсутствует|Удаляет [VPP токен](../resources/intune_onboarding_vpptoken.md).|
|[Обновить VPP токен](../api/intune_onboarding_vpptoken_update.md)|[VPP токен](../resources/intune_onboarding_vpptoken.md)|Обновление свойств объекта [VPP токен](../resources/intune_onboarding_vpptoken.md).|
|[Действие syncLicenses](../api/intune_onboarding_vpptoken_synclicenses.md)|[VPP токен](../resources/intune_onboarding_vpptoken.md)|Синхронизирует лицензии, связанные с конкретным appleVolumePurchaseProgramToken|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Автоматически генерируется при создании appleVolumePurchaseProgramToken. Это ключ объекта.|
|organizationName|Строка|Организация, связанная с токеном Apple Volume Purchase Program.|
|vppTokenAccountType|[vppTokenAccountType](../resources/intune_shared_vpptokenaccounttype.md)|Тип программы корпоративных закупок, с которой связан заданный маркер Программы корпоративных закупок Apple. Возможные значения: `business`, `education`. Возможные значения: `business`, `education`.|
|appleId|Строка|Идентификатор Apple ID, связанный с заданным маркером Apple Volume Purchase Program.|
|expirationDateTime|DateTimeOffset|Дата и время завершения срока действия маркера Apple Volume Purchase Program.|
|lastSyncDateTime|DateTimeOffset|Последнее выполнение синхронизации приложения при помощи службы Apple Volume Purchase Program с использованием токена Apple Volume Purchase Program.|
|токен|Строка|Строка токена Apple Volume Purchase Program; загрузка выполнена из Apple Volume Purchase Program.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения, связанного с токеном Apple Volume Purchase Program.|
|state|[vppTokenState](../resources/intune_onboarding_vpptokenstate.md)|Текущее состояние маркера Программы корпоративных закупок Apple. Возможные значения: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`. Возможные значения: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.|
|lastSyncStatus|[vppTokenSyncStatus](../resources/intune_onboarding_vpptokensyncstatus.md)|Текущее состояние последней синхронизации приложения, инициированной с помощью маркера Программы корпоративных закупок Apple. Возможные значения: `none`, `inProgress`, `completed`, `failed`. Возможные значения: `none`, `inProgress`, `completed`, `failed`.|
|automaticallyUpdateApps|Логическое|Автоматически обновятся все приложения, не только для токена VPP.|
|countryOrRegion|Строка|Автоматически обновятся все приложения, не только для токена VPP.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.vppToken"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.vppToken",
  "id": "String (identifier)",
  "organizationName": "String",
  "vppTokenAccountType": "String",
  "appleId": "String",
  "expirationDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "token": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "state": "String",
  "lastSyncStatus": "String",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "String"
}
```








