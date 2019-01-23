---
title: Тип ресурса depIOSEnrollmentProfile
description: Ресурс DepIOSEnrollmentProfile представляет определенного профиля регистрации программы регистрации устройства Apple (DEP) в конфигурации операций ввода-вывода. Этот тип профиля должен быть назначен Apple DEP представленные числами, прежде чем соответствующих устройств можно зарегистрировать с помощью функции.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0068921c65085417712efbe41e9145ac0b122cab
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400895"
---
# <a name="depiosenrollmentprofile-resource-type"></a>Тип ресурса depIOSEnrollmentProfile

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс DepIOSEnrollmentProfile представляет определенного профиля регистрации программы регистрации устройства Apple (DEP) в конфигурации операций ввода-вывода. Этот тип профиля должен быть назначен Apple DEP представленные числами, прежде чем соответствующих устройств можно зарегистрировать с помощью функции.


Наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список depIOSEnrollmentProfiles](../api/intune-enrollment-depiosenrollmentprofile-list.md)|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) коллекции|Свойства списка и связей объектов [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) .|
|[Получение depIOSEnrollmentProfile](../api/intune-enrollment-depiosenrollmentprofile-get.md)|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)|Чтение свойства и связи объекта [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) .|
|[Создание depIOSEnrollmentProfile](../api/intune-enrollment-depiosenrollmentprofile-create.md)|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)|Создание нового объекта [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) .|
|[Удаление depIOSEnrollmentProfile](../api/intune-enrollment-depiosenrollmentprofile-delete.md)|Нет|Удаляет [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md).|
|[Обновление depIOSEnrollmentProfile](../api/intune-enrollment-depiosenrollmentprofile-update.md)|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)|Обновление свойства объекта [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) .|

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
|isDefault|Логический|Указывает, является ли профилем по умолчанию унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|supervisedModeEnabled|Логический|Режим контролируемом значение True для включения значение false в противном случае. Просмотреть https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune для получения дополнительных сведений. Наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|supportDepartment|String|Отдел сведения о поддержке унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|passCodeDisabled|Логический|Указывает, если код связи, — это область настройки запрещено унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|isMandatory|Логический|Указывает, является ли профиль обязательные унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|locationDisabled|Логический|Указывает, если расположение Панель настроек службы запрещено унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|supportPhoneNumber|String|Номер телефона службы поддержки унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|profileRemovalDisabled|Логический|Указывает, если параметр удаления профиль отключен наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|restoreBlocked|Логический|Указывает, если область настройки восстановления блокируется наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|appleIdDisabled|Логический|Указывает, если панель настроек идентификатор Apple запрещено Inherited из [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|termsAndConditionsDisabled|Логический|Указывает, если отключено «Сроками и условиями» область настройки наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|touchIdDisabled|Логический|Указывает, если область настройки идентификатор сенсорного ввода отключен наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|applePayDisabled|Логический|Указывает, если область настройки оплаты Apple отключен наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|zoomDisabled|Логический|Указывает, если область настройки масштаба отключен наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|siriDisabled|Логический|Указывает, если область настроек siri отключен наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|diagnosticsDisabled|Логический|Указывает, если диагностики, Панель настроек запрещено унаследованные от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|displayToneSetupDisabled|Логический|Указывает, если экран установки displaytone отключен наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|privacyPaneDisabled|Логический|Указывает, если отключено экрана конфиденциальности наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|iTunesPairingMode.|[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md).|Указывает iTunes, режим связывания. Возможные значения: `disallow`, `allow`, `requiresCertificate`.|
|managementCertificates|[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) коллекции|Управление сертификатами для конфигуратора Apple|
|restoreFromAndroidDisabled|Логический|Указывает, если отключено восстановление из Android (en)|
|awaitDeviceConfiguredConfirmation|Логический|Указывает, если устройство необходимо подождать настроенного подтверждения|
|sharedIPadMaximumUserCount|Int32|Это указывает максимальное количество пользователей, которые могут использовать общие iPad. Применим только в режиме общего iPad.|
|enableSharedIPad|Логический|Это указывает, является ли устройство для участвуют в режиме, которое позволяет несколькими пользовательские сценарии. Применим только в общих iPads.|
|companyPortalVppTokenId|String|Если значение, указывает, какие Vpp маркер следует использовать для развертывания портала компании с устройства лицензирования. «enableAuthenticationViaCompanyPortal» необходимо задать для этого свойства должно быть задано.|
|enableSingleAppEnrollmentMode|Логический|Указывает устройство, чтобы включить режим одного приложения и применение блокировки приложения во время регистрации. Значение по умолчанию — false. «enableAuthenticationViaCompanyPortal» и «companyPortalVppTokenId» необходимо задать для этого свойства должно быть задано.|
|homeButtonScreenDisabled|Логический|Указывает, если уровень конфиденциальности сообщения окна кнопки Домой отключено|
|iMessageAndFaceTimeScreenDisabled|Логический|Указывает, если iMessage отключена FaceTime экрана|
|onBoardingScreenDisabled|Логический|Указывает, если экран установки входящая отключен|
|screenTimeScreenDisabled|Логический|Указывает, если экран установки времени ожидания отключен|
|simSetupScreenDisabled|Логический|Указывает, если на экране SIMSetup отключен|
|softwareUpdateScreenDisabled|Логический|Указывает, если на экране обязательные программа обновления отключен|
|watchMigrationScreenDisabled|Логический|Указывает, если на экране миграции Контрольное значение отключено|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.depIOSEnrollmentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.depIOSEnrollmentProfile",
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
  "profileRemovalDisabled": true,
  "restoreBlocked": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "displayToneSetupDisabled": true,
  "privacyPaneDisabled": true,
  "iTunesPairingMode": "String",
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "String",
      "certificate": "String"
    }
  ],
  "restoreFromAndroidDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 1024,
  "enableSharedIPad": true,
  "companyPortalVppTokenId": "String",
  "enableSingleAppEnrollmentMode": true,
  "homeButtonScreenDisabled": true,
  "iMessageAndFaceTimeScreenDisabled": true,
  "onBoardingScreenDisabled": true,
  "screenTimeScreenDisabled": true,
  "simSetupScreenDisabled": true,
  "softwareUpdateScreenDisabled": true,
  "watchMigrationScreenDisabled": true
}
```




