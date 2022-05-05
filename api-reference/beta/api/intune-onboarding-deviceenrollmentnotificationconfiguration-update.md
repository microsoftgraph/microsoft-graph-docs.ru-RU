---
title: Обновление объекта deviceEnrollmentNotificationConfiguration
description: Обновление свойств объекта deviceEnrollmentNotificationConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0127d0d837814dd699a2cd10e06c28e712532517
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65213263"
---
# <a name="update-deviceenrollmentnotificationconfiguration"></a>Обновление объекта deviceEnrollmentNotificationConfiguration

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [deviceEnrollmentNotificationConfiguration](../resources/intune-onboarding-deviceenrollmentnotificationconfiguration.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [deviceEnrollmentNotificationConfiguration](../resources/intune-onboarding-deviceenrollmentnotificationconfiguration.md) в формате JSON.

В следующей таблице показаны свойства, необходимые при создании [объекта deviceEnrollmentNotificationConfiguration](../resources/intune-onboarding-deviceenrollmentnotificationconfiguration.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор учетной записи, унаследованного от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|displayName|Строка|Отображаемое имя конфигурации регистрации устройства, унаследованного от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|description|Строка|Описание конфигурации регистрации устройства, унаследованного от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|priority|Int32|Приоритет используется, когда пользователь существует в нескольких группах, для которых назначена конфигурация регистрации. На пользователей распространяется только конфигурация с наименьшим значением приоритета. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|createdDateTime|DateTimeOffset|Дата создания в формате UTC конфигурации регистрации устройства, унаследованного от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|Дата последнего изменения в формате UTC конфигурации регистрации устройства, унаследованного от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|version|Int32|Версия конфигурации регистрации устройства, унаследованного от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|Идентификаторы roleScopeTagId|Коллекция объектов string|Необязательные теги области роли для ограничений регистрации. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|DeviceEnrollmentConfigurationType|[DeviceEnrollmentConfigurationType](../resources/intune-onboarding-deviceenrollmentconfigurationtype.md)|Поддержка типа конфигурации регистрации, унаследованного [от deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md). Возможные значения: `unknown`, `limit`, `platformRestrictions`, `windowsHelloForBusiness`, `defaultLimit`, `defaultPlatformRestrictions`, `defaultWindowsHelloForBusiness`, `defaultWindows10EnrollmentCompletionPageConfiguration`, `windows10EnrollmentCompletionPageConfiguration`, `deviceComanagementAuthorityConfiguration`, `singlePlatformRestriction`, `unknownFutureValue`, `enrollmentNotificationsConfiguration`.|
|platformType|[enrollmentRestrictionPlatformType](../resources/intune-onboarding-enrollmentrestrictionplatformtype.md)|Тип платформы уведомления о регистрации. Возможные значения: `allPlatforms`, `ios`, `windows`, `windowsPhone`, `android`, `androidForWork`, `mac`.|
|templateType|[enrollmentNotificationTemplateType](../resources/intune-onboarding-enrollmentnotificationtemplatetype.md)|Тип шаблона уведомления о регистрации. Возможные значения: `email`, `push`, `unknownFutureValue`.|
|NotificationMessageTemplateId|Guid|Идентификатор шаблона сообщения уведомления|
|brandingOptions|[enrollmentNotificationBrandingOptions](../resources/intune-onboarding-enrollmentnotificationbrandingoptions.md)|Параметры фирменной символики для уведомления о регистрации. Возможные значения: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`, `includeCompanyPortalLink`, `includeDeviceDetails`.|
|defaultLocale|String|DefaultLocale для уведомления о регистрации|



## <a name="response"></a>Ответ
В случае успешного выполнения `200 OK` этот метод возвращает код отклика и обновленный объект [deviceEnrollmentNotificationConfiguration](../resources/intune-onboarding-deviceenrollmentnotificationconfiguration.md) в теле отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 525

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentNotificationConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "deviceEnrollmentConfigurationType": "limit",
  "platformType": "ios",
  "templateType": "push",
  "notificationMessageTemplateId": "eba3ed57-ed57-eba3-57ed-a3eb57eda3eb",
  "brandingOptions": "includeCompanyLogo",
  "defaultLocale": "Default Locale value"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 697

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentNotificationConfiguration",
  "id": "bdd0743a-743a-bdd0-3a74-d0bd3a74d0bd",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "deviceEnrollmentConfigurationType": "limit",
  "platformType": "ios",
  "templateType": "push",
  "notificationMessageTemplateId": "eba3ed57-ed57-eba3-57ed-a3eb57eda3eb",
  "brandingOptions": "includeCompanyLogo",
  "defaultLocale": "Default Locale value"
}
```




