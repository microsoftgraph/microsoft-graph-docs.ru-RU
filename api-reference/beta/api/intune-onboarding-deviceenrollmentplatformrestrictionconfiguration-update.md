---
title: Обновление устройстваEnrollmentPlatformRestrictionConfiguration
description: Обновление свойств объекта deviceEnrollmentPlatformRestrictionConfiguration.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3f422e2492f785fb42b687d9d0be831b68a1eb4c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59121195"
---
# <a name="update-deviceenrollmentplatformrestrictionconfiguration"></a>Обновление устройстваEnrollmentPlatformRestrictionConfiguration

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [deviceEnrollmentPlatformRestrictionConfiguration.](../resources/intune-onboarding-deviceenrollmentplatformrestrictionconfiguration.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementServiceConfig.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementServiceConfig.ReadWrite.All|

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
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса предоставляем представление JSON для [объекта deviceEnrollmentPlatformRestrictionConfiguration.](../resources/intune-onboarding-deviceenrollmentplatformrestrictionconfiguration.md)

В следующей таблице показаны свойства, необходимые при создании [устройстваEnrollmentPlatformRestrictionConfiguration.](../resources/intune-onboarding-deviceenrollmentplatformrestrictionconfiguration.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор учетной записи, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|displayName|String|Отображающее имя конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|description|String|Описание конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|priority|Int32|Приоритет используется, когда пользователь существует в нескольких группах, которые назначены конфигурации регистрации. Пользователи подчиняются только конфигурации с наименьшим значением приоритета. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|createdDateTime|DateTimeOffset|Создано время даты в UTC конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|Последнее измененное время даты в UTC конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|version|Int32|Версия конфигурации регистрации устройства, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|roleScopeTagIds|Коллекция объектов string|Необязательные теги области ролей для ограничений регистрации. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|platformRestriction|[deviceEnrollmentPlatformRestriction](../resources/intune-onboarding-deviceenrollmentplatformrestriction.md)|Ограничения на основе платформы, версии операционной системы платформы и владения устройствами|
|platformType|[enrollmentRestrictionPlatformType](../resources/intune-onboarding-enrollmentrestrictionplatformtype.md)|Тип платформы, для которой применяется это ограничение. Возможные значения: `allPlatforms`, `ios`, `windows`, `windowsPhone`, `android`, `androidForWork`, `androidAosp`, `mac`.|



## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает код отклика и обновленный объект `200 OK` [deviceEnrollmentPlatformRestrictionConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionconfiguration.md) в теле отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 716

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestrictionConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "platformRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ],
    "blockedSkus": [
      "Blocked Skus value"
    ]
  },
  "platformType": "ios"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 888

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestrictionConfiguration",
  "id": "dedce9f4-e9f4-dedc-f4e9-dcdef4e9dcde",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "platformRestriction": {
    "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
    "platformBlocked": true,
    "personalDeviceEnrollmentBlocked": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "blockedManufacturers": [
      "Blocked Manufacturers value"
    ],
    "blockedSkus": [
      "Blocked Skus value"
    ]
  },
  "platformType": "ios"
}
```



