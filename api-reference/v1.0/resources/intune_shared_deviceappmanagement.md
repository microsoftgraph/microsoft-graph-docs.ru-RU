# <a name="deviceappmanagement-resource-type"></a>Тип ресурса deviceAppManagement

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Одноэлементный объект, служащий контейнером для всех функций управления приложениями на устройствах.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение объекта deviceAppManagement](../api/intune_shared_deviceappmanagement_get.md)|Чтение свойств и связей объекта [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md).|
|[Обновление объекта deviceAppManagement](../api/intune_shared_deviceappmanagement_update.md)|Обновление свойств объекта [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md).|
|**Адаптация**|
|[Действие syncMicrosoftStoreForBusinessApps](../api/intune_shared_deviceappmanagement_syncmicrosoftstoreforbusinessapps.md)|Нет|Синхронизирует учетную запись Intune с Microsoft Store для бизнеса|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|**Адаптация**|
|isEnabledForMicrosoftStoreForBusiness|Boolean (логический)|Указывает, включена ли для учетной запись синхронизация приложений из Microsoft Store для бизнеса.|
|microsoftStoreForBusinessLanguage|string|Сведения о языковом стандарте, используемом для синхронизации приложений из Microsoft Store для бизнеса. Региональные параметры, относящиеся к стране или региону. Названия этих региональных параметров соответствуют стандарту RFC 4646 (для Windows Vista и более поздних версий). Используется формат <languagecode2>-<страна/код_региона2>, где <languagecode2> — это двухбуквенный код в нижнем регистре, полученный из стандарта ISO 639-1, а <страна/код_регион2> — код из двух прописных букв по стандарту ISO 3166. Например, en-US для английского (США) — это определенный региональный стандарт.|
|microsoftStoreForBusinessLastCompletedApplicationSyncTime|DateTimeOffset|Время последней завершенной синхронизации приложений из Microsoft Store для бизнеса.|
|microsoftStoreForBusinessLastSuccessfulSyncDateTime|DateTimeOffset|Время последней успешной синхронизации приложений из Microsoft Store для бизнеса с учетной записью.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|**Apps**|
|mobileAppCategories|Коллекция [mobileAppCategory](../resources/intune_apps_mobileappcategory.md)|Категории мобильных приложений|
|mobileAppConfigurations|Коллекция [managedDeviceMobileAppConfiguration](../resources/intune_apps_manageddevicemobileappconfiguration.md)|Конфигурации мобильных приложений для управляемых устройств.|
|mobileApps|Коллекция [mobileApp](../resources/intune_apps_mobileapp.md)|Мобильные приложения.|
|**Books**|
|managedEBooks|Коллекция [managedEBook](../resources/intune_books_managedebook.md)|Управляемая электронная книга.|
|**Мобильное приложение управления (MAM)**|
|androidManagedAppProtections|Коллекция [androidManagedAppProtection](../resources/intune_mam_androidmanagedappprotection.md)|Политики управляемых приложений для Android.|
|defaultManagedAppProtections|Коллекция [defaultManagedAppProtection](../resources/intune_mam_defaultmanagedappprotection.md)|Политики управляемых приложений по умолчанию.|
|iosManagedAppProtections|Коллекция [iosManagedAppProtection](../resources/intune_mam_iosmanagedappprotection.md)|Политики управляемых приложений для iOS.|
|managedAppPolicies|Коллекция [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|Политики управляемых приложений.|
|managedAppRegistrations|Коллекция [managedAppRegistration](../resources/intune_mam_managedappregistration.md)|Регистрации управляемых приложений.|
|managedAppStatuses|Коллекция [managedAppStatus](../resources/intune_mam_managedappstatus.md)|Состояния управляемых приложений.|
|mdmWindowsInformationProtectionPolicies|Коллекция [mdmWindowsInformationProtectionPolicy](../resources/intune_mam_mdmwindowsinformationprotectionpolicy.md)|Windows Information Protection для приложений на устройствах, зарегистрированных с использованием MDM.|
|targetedManagedAppConfigurations|Коллекция [targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md)|Целевые конфигурации управляемых приложений.|
|windowsInformationProtectionPolicies|Коллекция [windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md)|Windows Information Protection для приложений на устройствах, не зарегистрированных с использованием MDM.|
|**Адаптация**|
|vppTokens|[vpp Токен](../resources/intune_onboarding_vpptoken.md) коллекция|Список Vpp маркеров для данной организации.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.  Обратите внимание, что это — пример. Ответы на фактические запросы будут содержать свойства, соответствующие контексту.  
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.deviceAppManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "String (identifier)",
  "microsoftStoreForBusinessLastSuccessfulSyncDateTime": "String (timestamp)",
  "isEnabledForMicrosoftStoreForBusiness": true,
  "microsoftStoreForBusinessLanguage": "String",
  "microsoftStoreForBusinessLastCompletedApplicationSyncTime": "String (timestamp)"
}
```



