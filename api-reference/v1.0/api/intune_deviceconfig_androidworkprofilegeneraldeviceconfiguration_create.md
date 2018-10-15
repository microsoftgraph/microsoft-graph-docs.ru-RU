# <a name="create-androidworkprofilegeneraldeviceconfiguration"></a>Создание androidWorkProfileGeneralDeviceConfiguration

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Создание нового объекта [androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md).
## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Авторизация|Требуется Bearer &lt;маркер&gt;|
|Принять|приложение/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса укажите представление объекта androidWorkProfileGeneralDeviceConfiguration в формате JSON.

В приведенной ниже таблице указаны свойства, необходимые при создании объекта androidWorkProfileGeneralDeviceConfiguration.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|описание|Строка|Указанное администратором описание конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|displayName|Строка|Указанное администратором имя конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md).|
|passwordBlockFingerprintUnlock|Логический|Указывает, следует ли запретить разблокировку с помощью отпечатка пальца.|
|passwordBlockTrustAgents|Логический|Указывает, следует ли блокировать Smart Lock и другие агенты безопасности.|
|passwordExpirationDays|Int32|Количество дней до окончания срока действия пароля. Допустимые значения: от 1 до 365.|
|passwordMinimumLength|Int32|Минимальная длина паролей. Допустимые значения: от 4 до 16.|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Время бездействия до отключения экрана (в минутах).|
|passwordPreviousPasswordBlockCount|Int32|Количество предыдущих паролей, которые требуется блокировать. Допустимые значения: от 0 до 24|
|passwordSignInFailureCountBeforeFactoryReset|Int32|Количество неудачных попыток входа до восстановления заводских настроек. Допустимые значения: от 4 до 11|
|passwordRequiredType|[androidWorkProfileRequiredPasswordType](../resources/intune_deviceconfig_androidworkprofilerequiredpasswordtype.md)|Требуемый тип пароля. Возможные значения: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.|
|workProfileDataSharingType|[androidWorkProfileCrossProfileDataSharingType](../resources/intune_deviceconfig_androidworkprofilecrossprofiledatasharingtype.md)|Разрешенный тип общего доступа к данным. Возможные значения: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.|
|workProfileBlockNotificationsWhileDeviceLocked|Логическое|Указывает, следует ли блокировать уведомления, когда устройство заблокировано.|
|workProfileBlockAddingAccounts|Логическое|Установка запрета для пользователей на добавление или удаление учетных записей в рабочем профиле.|
|workProfileBluetoothEnableContactSharing|Логическое|Разрешение устройствам bluetooth получать доступ к контактам предприятия.|
|workProfileBlockScreenCapture|Логическое|Установка запрета на снимок экрана в рабочем профиле.|
|workProfileBlockCrossProfileCallerId|Логическое|Установка запрета на отображение в личном профиле идентификатора вызывающего абонента рабочего профиля.|
|workProfileBlockCamera|Логическое|Блокировка камеры рабочего профиля.|
|workProfileBlockCrossProfileContactsSearch|Логическое|Блокировка доступности контактов рабочего профиля в личном профиле.|
|workProfileBlockCrossProfileCopyPaste|Логическое|Логическое значение, которое указывает, включена ли настройка запрета копирования или вставки между профилями.|
|workProfileDefaultAppPermissionPolicy|[androidWorkProfileDefaultAppPermissionPolicyType](../resources/intune_deviceconfig_androidworkprofiledefaultapppermissionpolicytype.md)|Требуемый тип пароля. Возможные значения: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.|
|workProfilePasswordBlockFingerprintUnlock|Логическое|Указывает, следует ли запретить разблокировку с помощью отпечатка пальца для рабочего профиля.|
|workProfilePasswordBlockTrustAgents|Логическое|Указывает, следует ли блокировать Smart Lock и другие агенты безопасности для рабочего профиля.|
|workProfilePasswordExpirationDays|Int32|Количество дней до окончания срока действия пароля рабочего профиля. Допустимые значения: от 1 до 365.|
|workProfilePasswordMinimumLength|Int32|Минимальная длина пароля рабочего профиля. Допустимые значения: от 4 до 16.|
|workProfilePasswordMinNumericCharacters|Int32|Требуемое минимальное количество цифровых символов в пароле рабочего профиля. Допустимые значения: от 1 до 10.|
|workProfilePasswordMinNonLetterCharacters|Int32|Требуемое минимальное количество небуквенных символов в пароле рабочего профиля. Допустимые значения: от 1 до 10.|
|workProfilePasswordMinLetterCharacters|Int32|Требуемое минимальное количество буквенных символов в пароле рабочего профиля. Допустимые значения: от 1 до 10.|
|workProfilePasswordMinLowerCaseCharacters|Int32|Требуемое минимальное количество строчных букв в пароле рабочего профиля. Допустимые значения: от 1 до 10.|
|workProfilePasswordMinUpperCaseCharacters|Int32|Требуемое минимальное количество прописных букв в пароле рабочего профиля. Допустимые значения: от 1 до 10.|
|workProfilePasswordMinSymbolCharacters|Int32|Требуемое минимальное количество символов в пароле рабочего профиля. Допустимые значения: от 1 до 10.|
|workProfilePasswordMinutesOfInactivityBeforeScreenTimeout|Int32|Время бездействия до отключения экрана (в минутах).|
|workProfilePasswordPreviousPasswordBlockCount|Int32|Количество предыдущих паролей рабочего профиля, которые требуется блокировать. Допустимые значения: от 0 до 24.|
|workProfilePasswordSignInFailureCountBeforeFactoryReset|Int32|Количество неудачных попыток входа до удаления рабочего профиля и всех корпоративных данных. Допустимые значения: от 4 до 11|
|workProfilePasswordRequiredType|[androidWorkProfileRequiredPasswordType](../resources/intune_deviceconfig_androidworkprofilerequiredpasswordtype.md)|Требуемый тип пароля рабочего профиля. Возможные значения: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.|
|workProfileRequirePassword|Логическое|Требуется ли пароль для рабочего профиля|
|securityRequireVerifyApps|Логический|Указывает, что требуется включить функцию проверки приложений для Android.|



## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает `201 Created` код ответа и объект [androidWorkProfileGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidworkprofilegeneraldeviceconfiguration.md) в тексте ответа.

## <a name="example"></a>Пример
### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1895

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "lowSecurityBiometric",
  "workProfileDataSharingType": "preventAny",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "prompt",
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinNumericCharacters": 7,
  "workProfilePasswordMinNonLetterCharacters": 9,
  "workProfilePasswordMinLetterCharacters": 6,
  "workProfilePasswordMinLowerCaseCharacters": 9,
  "workProfilePasswordMinUpperCaseCharacters": 9,
  "workProfilePasswordMinSymbolCharacters": 6,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
  "workProfilePasswordPreviousPasswordBlockCount": 13,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "lowSecurityBiometric",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true
}
```

### <a name="response"></a>Ответ
Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2003

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
  "id": "6decda7e-da7e-6dec-7eda-ec6d7edaec6d",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "lowSecurityBiometric",
  "workProfileDataSharingType": "preventAny",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "prompt",
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinNumericCharacters": 7,
  "workProfilePasswordMinNonLetterCharacters": 9,
  "workProfilePasswordMinLetterCharacters": 6,
  "workProfilePasswordMinLowerCaseCharacters": 9,
  "workProfilePasswordMinUpperCaseCharacters": 9,
  "workProfilePasswordMinSymbolCharacters": 6,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
  "workProfilePasswordPreviousPasswordBlockCount": 13,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "lowSecurityBiometric",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true
}
```








