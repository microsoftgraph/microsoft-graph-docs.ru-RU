---
title: Тип ресурса depEnrollmentProfile
description: Ресурс depEnrollmentProfile представляет профиля регистрации программы регистрации устройства Apple (DEP). Этот тип профиля должен быть назначен Apple DEP представленные числами, прежде чем соответствующих устройств можно зарегистрировать с помощью функции.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 61119a97deb41807e6eee66f0ef3376035500190
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395904"
---
# <a name="depenrollmentprofile-resource-type"></a>Тип ресурса depEnrollmentProfile

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс depEnrollmentProfile представляет профиля регистрации программы регистрации устройства Apple (DEP). Этот тип профиля должен быть назначен Apple DEP представленные числами, прежде чем соответствующих устройств можно зарегистрировать с помощью функции.


Наследуется от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список depEnrollmentProfiles](../api/intune-enrollment-depenrollmentprofile-list.md)|[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) коллекции|Свойства списка и связей объектов [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) .|
|[Получение depEnrollmentProfile](../api/intune-enrollment-depenrollmentprofile-get.md)|[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md);|Чтение свойства и связи объекта [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) .|
|[Создание depEnrollmentProfile](../api/intune-enrollment-depenrollmentprofile-create.md)|[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md);|Создание нового объекта [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) .|
|[Удаление depEnrollmentProfile](../api/intune-enrollment-depenrollmentprofile-delete.md)|Нет|Удаляет [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md).|
|[Обновление depEnrollmentProfile](../api/intune-enrollment-depenrollmentprofile-update.md)|[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md);|Обновление свойства объекта [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор GUID для объекта унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|displayName|String|Имя профиля, унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|description|String|Описание профиля унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requiresUserAuthentication|Логический|Указывает, если профиль требует проверки подлинности пользователя унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|configurationEndpointUrl|String|Конфигурация конечную точку URL-адрес для регистрации наследуется от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|enableAuthenticationViaCompanyPortal|Логический|Указывает на проверку подлинности с Apple помощник по настройке вместо портала компании. Наследуется от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Логический|Указывает, что требуется портала компании на устройствах помощник по регистрации программы установки унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|isDefault|Логический|Указывает, является ли профиля по умолчанию|
|supervisedModeEnabled|Логический|Режим контролируемом значение True для включения значение false в противном случае. Просмотреть https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune для получения дополнительных сведений.|
|supportDepartment|String|Сведения о поддержке отдела|
|passCodeDisabled|Логический|Указывает, если область настройки секретный код отключен|
|isMandatory|Логический|Указывает, является ли обязательных профилей|
|locationDisabled|Логический|Указывает, если область настройки расположения службы отключен|
|supportPhoneNumber|String|Номер телефона службы поддержки|
|iTunesPairingMode.|[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md).|Указывает iTunes, режим связывания. Возможные значения: `disallow`, `allow`, `requiresCertificate`.|
|profileRemovalDisabled|Логический|Указывает, если параметр удаления профиль отключен|
|managementCertificates|[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) коллекции|Управление сертификатами для конфигуратора Apple|
|restoreBlocked|Логический|Указывает, если область настройки восстановления блокируется|
|restoreFromAndroidDisabled|Логический|Указывает, если отключено восстановление из Android (en)|
|appleIdDisabled|Логический|Указывает, если область настройки идентификатор Apple отключен|
|termsAndConditionsDisabled|Логический|Указывает, если отключено «Сроками и условиями» область настройки|
|touchIdDisabled|Логический|Указывает, если область настройки идентификатор сенсорного ввода отключен|
|applePayDisabled|Логический|Указывает, если область настройки оплаты Apple отключен|
|zoomDisabled|Логический|Указывает, если область настройки масштаба отключен|
|siriDisabled|Логический|Указывает, если область настроек siri отключен|
|diagnosticsDisabled|Логический|Указывает, если область настройки диагностики отключен|
|macOSRegistrationDisabled|Логический|Указывает, отключена при регистрации Mac OS|
|macOSFileVaultDisabled|Логический|Указывает, если отключено хранилище файлов Mac OS|
|awaitDeviceConfiguredConfirmation|Логический|Указывает, если устройство необходимо подождать настроенного подтверждения|
|sharedIPadMaximumUserCount|Int32|Это указывает максимальное количество пользователей, которые могут использовать общие iPad. Применим только в режиме общего iPad.|
|enableSharedIPad|Логический|Это указывает, является ли устройство для участвуют в режиме, которое позволяет несколькими пользовательские сценарии. Применим только в общих iPads.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.depEnrollmentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.depEnrollmentProfile",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "String",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true,
  "isDefault": true,
  "supervisedModeEnabled": true,
  "supportDepartment": "String",
  "passCodeDisabled": true,
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "String",
  "iTunesPairingMode": "String",
  "profileRemovalDisabled": true,
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "String",
      "certificate": "String"
    }
  ],
  "restoreBlocked": true,
  "restoreFromAndroidDisabled": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "macOSRegistrationDisabled": true,
  "macOSFileVaultDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 1024,
  "enableSharedIPad": true
}
```




