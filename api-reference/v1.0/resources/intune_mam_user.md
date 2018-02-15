# <a name="user-resource-type"></a>Тип ресурса user

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Представляет объект пользователя Azure Active Directory.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление пользователей](../api/intune_mam_user_list.md)|Коллекция объектов [user](../resources/intune_mam_user.md)|Список свойств и связей объектов [user](../resources/intune_mam_user.md).|
|[Получение пользователя](../api/intune_mam_user_get.md)|[user](../resources/intune_mam_user.md)|Чтение свойств и связей объекта [user](../resources/intune_mam_user.md).|
|[Создание пользователя](../api/intune_mam_user_create.md)|[user](../resources/intune_mam_user.md)|Создание объекта [user](../resources/intune_mam_user.md).|
|[Удаление пользователя](../api/intune_mam_user_delete.md)|Нет|Удаляет объект [user](../resources/intune_mam_user.md).|
|[Обновление пользователя](../api/intune_mam_user_update.md)|[user](../resources/intune_mam_user.md)|Обновление свойств объекта [user](../resources/intune_mam_user.md).|
|[Функция getManagedAppDiagnosticStatuses](../api/intune_mam_user_getmanagedappdiagnosticstatuses.md)|Коллекция [managedAppDiagnosticStatus](../resources/intune_mam_managedappdiagnosticstatus.md)|Получает состояние диагностической проверки определенного пользователя.|
|[Функция getManagedAppPolicies](../api/intune_mam_user_getmanagedapppolicies.md)|Коллекция [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|Получает ограничения приложений для определенного пользователя.|
|[Действие wipeManagedAppRegistrationsByDeviceTag](../api/intune_mam_user_wipemanagedappregistrationsbydevicetag.md)|Нет|Стирает данные о регистрации приложений с указанным тегом приложения.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор пользователя.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|managedAppRegistrations|Коллекция [managedAppRegistration](../resources/intune_mam_managedappregistration.md)|Любое количество объектов регистрации управляемых приложений, принадлежащих пользователю.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.user"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.user",
  "id": "String (identifier)"
}
```



