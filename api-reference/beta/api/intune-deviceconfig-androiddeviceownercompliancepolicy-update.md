---
title: Обновление androidDeviceOwnerCompliancePolicy
description: Обновление свойств объекта AndroidDeviceOwnerCompliancePolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4c9663d65c30e7518b619271b1d6f5439f218197
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58789462"
---
# <a name="update-androiddeviceownercompliancepolicy"></a>Обновление androidDeviceOwnerCompliancePolicy

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [AndroidDeviceOwnerCompliancePolicy.](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Application|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для [объекта AndroidDeviceOwnerCompliancePolicy.](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md)

В следующей таблице показаны свойства, необходимые при создании [androidDeviceOwnerCompliancePolicy.](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|roleScopeTagIds|Коллекция String|Список тегов области для этого экземпляра Entity. Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).|
|id|String|Ключ объекта. Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).|
|description|Строка|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md).|
|deviceThreatProtectionEnabled|Boolean|Указывает, что защита от угроз для устройств должна быть включена.|
|deviceThreatProtectionRequiredSecurityLevel|[deviceThreatProtectionLevel](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|Указывает на то, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям. Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.|
|advancedThreatProtectionRequiredSecurityLevel|[deviceThreatProtectionLevel](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|MDATP требует минимального уровня риска для защиты от мобильных угроз, чтобы сообщить о несоблюдении. Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.|
|securityRequireSafetyNetAttestationBasicIntegrity|Boolean|Указывает, что устройству требуется пройти базовую проверку целостности SafetyNet.|
|securityRequireSafetyNetAttestationCertifiedDevice|Boolean|Указывает, что устройству требуется пройти проверку сертификата SafetyNet.|
|osMinimumVersion|String|Минимальная версия Android.|
|osMaximumVersion|String|Максимальная версия Android.|
|minAndroidSecurityPatchLevel|String|Минимальный уровень обновления для системы безопасности Android.|
|passwordRequired|Boolean|Указывает, что для разблокировки устройства требуется указывать пароль.|
|passwordMinimumLength|Int32|Минимальная длина пароля. Допустимые значения: от 4 до 16.|
|passwordMinimumLetterCharacters|Int32|Указывает минимальное количество букв, необходимых для пароля устройства. Допустимые значения от 1 до 16|
|passwordMinimumLowerCaseCharacters|Int32|Указывает минимальное число символов более низкого уровня, необходимых для пароля устройства. Допустимые значения от 1 до 16|
|passwordMinimumNonLetterCharacters|Int32|Указывает минимальное количество символов без букв, необходимых для пароля устройства. Допустимые значения от 1 до 16|
|passwordMinimumNumericCharacters|Int32|Указывает минимальное число числимые символы, необходимые для пароля устройства. Допустимые значения от 1 до 16|
|passwordMinimumSymbolCharacters|Int32|Указывает минимальное количество символов, необходимых для пароля устройства. Допустимые значения от 1 до 16|
|passwordMinimumUpperCaseCharacters|Int32|Указывает минимальное количество символов верхней буквы, необходимых для пароля устройства. Допустимые значения от 1 до 16|
|passwordRequiredType|[AndroidDeviceOwnerRequiredPasswordType](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|Тип символов в пароле. Возможные значения: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `customPassword`.|
|passwordMinutesOfInactivityBeforeLock|Int32|Период бездействия (в минутах), по истечении которого будет запрашиваться ввод пароля.|
|passwordExpirationDays|Int32|Количество дней до окончания срока действия пароля. Допустимые значения: от 1 до 365.|
|passwordPreviousPasswordCountToBlock|Int32|Количество предыдущих паролей, которые требуется блокировать. Допустимые значения: от 1 до 24.|
|storageRequireEncryption|Boolean|Указывает, что шифрование на устройствах с Android должно быть обязательным.|
|securityRequireIntuneAppIntegrity|Логический|Если задаваем параметр true, проверяет, что приложение Intune, установленное на полностью управляемых, выделенных или корпоративных устройствах, зарегистрированных в Android Enterprise, — это приложение, предоставленное Корпорацией Майкрософт из управляемого магазина Google Playstore. Если проверка не выполняется, устройство будет отчитаться о несоблюдении.|



## <a name="response"></a>Отклик
В случае успешного использования этот метод возвращает код отклика и обновленный `200 OK` [объект androidDeviceOwnerCompliancePolicy](../resources/intune-deviceconfig-androiddeviceownercompliancepolicy.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 1269

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "advancedThreatProtectionRequiredSecurityLevel": "secured",
  "securityRequireSafetyNetAttestationBasicIntegrity": true,
  "securityRequireSafetyNetAttestationCertifiedDevice": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordMinimumLetterCharacters": 15,
  "passwordMinimumLowerCaseCharacters": 2,
  "passwordMinimumNonLetterCharacters": 2,
  "passwordMinimumNumericCharacters": 0,
  "passwordMinimumSymbolCharacters": 15,
  "passwordMinimumUpperCaseCharacters": 2,
  "passwordRequiredType": "required",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordCountToBlock": 4,
  "storageRequireEncryption": true,
  "securityRequireIntuneAppIntegrity": true
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1441

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "be2464b4-64b4-be24-b464-24beb46424be",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "advancedThreatProtectionRequiredSecurityLevel": "secured",
  "securityRequireSafetyNetAttestationBasicIntegrity": true,
  "securityRequireSafetyNetAttestationCertifiedDevice": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordMinimumLetterCharacters": 15,
  "passwordMinimumLowerCaseCharacters": 2,
  "passwordMinimumNonLetterCharacters": 2,
  "passwordMinimumNumericCharacters": 0,
  "passwordMinimumSymbolCharacters": 15,
  "passwordMinimumUpperCaseCharacters": 2,
  "passwordRequiredType": "required",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordCountToBlock": 4,
  "storageRequireEncryption": true,
  "securityRequireIntuneAppIntegrity": true
}
```



