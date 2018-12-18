---
title: Тип ресурса depEnrollmentProfile
description: Ресурс depEnrollmentProfile представляет профиля регистрации программы регистрации устройства Apple (DEP). Этот тип профиля должен быть назначен Apple DEP представленные числами, прежде чем соответствующих устройств можно зарегистрировать с помощью функции.
author: tfitzmac
ms.openlocfilehash: 5079a109e2c1aa236c69fff8d114e4a37d82367c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316970"
---
# <a name="depenrollmentprofile-resource-type"></a>Тип ресурса depEnrollmentProfile

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

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
|id|Строка|Идентификатор GUID для объекта унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|displayName|Строка|Имя профиля, унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|описание|Строка|Описание профиля унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requiresUserAuthentication|Boolean.|Указывает, если профиль требует проверки подлинности пользователя унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|configurationEndpointUrl|String.|Конфигурация конечную точку URL-адрес для регистрации наследуется от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|enableAuthenticationViaCompanyPortal|Boolean.|Указывает на проверку подлинности с Apple помощник по настройке вместо портала компании. Наследуется от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|isDefault|Boolean|Указывает, является ли профиля по умолчанию|
|supervisedModeEnabled|Boolean.|Режим контролируемом значение True для включения значение false в противном случае. Просмотреть https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune для получения дополнительных сведений.|
|supportDepartment|String.|Сведения о поддержке отдела|
|passCodeDisabled|Boolean.|Указывает, если область настройки секретный код отключен|
|isMandatory|Boolean.|Указывает, является ли обязательных профилей|
|locationDisabled|Boolean.|Указывает, если область настройки расположения службы отключен|
|supportPhoneNumber|String.|Номер телефона службы поддержки|
|iTunesPairingMode.|[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md).|Указывает iTunes, режим связывания. Возможные значения: `disallow`, `allow`, `requiresCertificate`.|
|profileRemovalDisabled|Boolean.|Указывает, если параметр удаления профиль отключен|
|managementCertificates|[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) коллекции|Управление сертификатами для конфигуратора Apple|
|restoreBlocked|Boolean.|Указывает, если область настройки восстановления блокируется|
|restoreFromAndroidDisabled|Boolean.|Указывает, если отключено восстановление из Android (en)|
|appleIdDisabled|Boolean.|Указывает, если область настройки идентификатор Apple отключен|
|termsAndConditionsDisabled|Boolean.|Указывает, если отключено «Сроками и условиями» область настройки|
|touchIdDisabled|Boolean.|Указывает, если область настройки идентификатор сенсорного ввода отключен|
|applePayDisabled|Boolean.|Указывает, если область настройки оплаты Apple отключен|
|zoomDisabled|Boolean.|Указывает, если область настройки масштаба отключен|
|siriDisabled|Boolean.|Указывает, если область настроек siri отключен|
|diagnosticsDisabled|Boolean.|Указывает, если область настройки диагностики отключен|
|macOSRegistrationDisabled|Boolean.|Указывает, отключена при регистрации Mac OS|
|macOSFileVaultDisabled|Boolean.|Указывает, если отключено хранилище файлов Mac OS|
|awaitDeviceConfiguredConfirmation|Boolean.|Указывает, если устройство необходимо подождать настроенного подтверждения|
|sharedIPadMaximumUserCount|Int32|Это указывает максимальное количество пользователей, которые могут использовать общие iPad. Применим только в режиме общего iPad.|
|enableSharedIPad|Boolean.|Это указывает, является ли устройство для участвуют в режиме, которое позволяет несколькими пользовательские сценарии. Применим только в общих iPads.|

## <a name="relationships"></a>Связи
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





