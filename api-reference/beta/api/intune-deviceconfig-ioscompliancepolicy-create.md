---
title: Create iosCompliancePolicy
description: Создание объекта iosCompliancePolicy.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e1fdebc75bfa98d2da83889c0e0e4cbc2ed76a23
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423057"
---
# <a name="create-ioscompliancepolicy"></a>Create iosCompliancePolicy

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание объекта [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md).

## <a name="prerequisites"></a>Необходимые разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).

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
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Авторизация|Требуется Bearer &lt;маркер&gt;
|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта iosCompliancePolicy в формате JSON.

В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта iosCompliancePolicy.

|Свойство|Тип|Описание|
|:---|:---|:---|
|roleScopeTagIds|Коллекция String|Список областей теги для данного экземпляра сущности. Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|id|String|Ключ объекта. Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|description|String|Указанное администратором описание конфигурации устройства. Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|displayName|String|Указанное администратором имя конфигурации устройства. Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|version|Int32|Версия конфигурации устройства. Наследуется от объекта [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).|
|passcodeBlockSimple|Логический|Указывает, следует ли блокировать простые секретные коды.|
|passcodeExpirationDays|Int32|Количество дней до окончания срока действия секретного кода. Допустимые значения: от 1 до 65 535.|
|passcodeMinimumLength|Int32|Минимальная длина секретного кода. Допустимые значения: от 4 до 14.|
|passcodeMinutesOfInactivityBeforeLock|Int32|Период бездействия (в минутах) до запроса пароля.|
|passcodeMinutesOfInactivityBeforeScreenTimeout|Int32|Время бездействия до отключения экрана (в минутах).|
|passcodePreviousPasscodeBlockCount|Int32|Количество предыдущих секретных кодов, которые следует блокировать. Допустимые значения: от 1 до 24.|
|passcodeMinimumCharacterSetCount|Int32|Количество наборов символов, которые требуются для пароля.|
|passcodeRequiredType|[requiredPasswordType](../resources/intune-deviceconfig-requiredpasswordtype.md)|Требуемый тип секретного кода. Возможные значения: `deviceDefault`, `alphanumeric`, `numeric`.|
|passcodeRequired|Логический|Указывает, требуется ли запрашивать секретный код.|
|osMinimumVersion|String|Минимальная версия iOS.|
|osMaximumVersion|String|Максимальная версия iOS.|
|osMinimumBuildVersion|String|Версия сборки минимальные операций ввода-ВЫВОДА.|
|osMaximumBuildVersion|String|Версия сборки максимальное операций ввода-ВЫВОДА.|
|securityBlockJailbrokenDevices|Boolean|Устройства запрещено взламывать и рутовать.|
|deviceThreatProtectionEnabled|Boolean|Указывает, что защита от угроз для устройств должна быть включена.|
|deviceThreatProtectionRequiredSecurityLevel|[deviceThreatProtectionLevel](../resources/intune-deviceconfig-devicethreatprotectionlevel.md)|Указывает, что на уровне минимального риска, определенного в Mobile Threat Protection, нужно сообщать о несоответствии требованиям. Возможные значения: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.|
|managedEmailProfileRequired|Boolean|Указывает, обязательно ли использовать управляемый профиль электронной почты.|
|restrictedApps|Коллекция [appListItem](../resources/intune-deviceconfig-applistitem.md)|Требуется устройство, чтобы отказаться от указанного приложения, установленные. Эта коллекция может содержать не более 100 элементов.|



## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1241

{
  "@odata.type": "#microsoft.graph.iosCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "osMinimumBuildVersion": "Os Minimum Build Version value",
  "osMaximumBuildVersion": "Os Maximum Build Version value",
  "securityBlockJailbrokenDevices": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "managedEmailProfileRequired": true,
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ]
}
```

### <a name="response"></a>Отклик
Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1413

{
  "@odata.type": "#microsoft.graph.iosCompliancePolicy",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "4f501351-1351-4f50-5113-504f5113504f",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "osMinimumBuildVersion": "Os Minimum Build Version value",
  "osMaximumBuildVersion": "Os Maximum Build Version value",
  "securityBlockJailbrokenDevices": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "managedEmailProfileRequired": true,
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ]
}
```




