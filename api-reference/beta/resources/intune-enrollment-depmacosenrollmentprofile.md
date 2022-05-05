---
title: Тип ресурса depMacOSEnrollmentProfile
description: Ресурс DepMacOSEnrollmentProfile представляет профиль регистрации программы регистрации устройств Apple (DEP), относщийся к конфигурации macOS. Этот тип профиля необходимо назначить серийным номерам Apple DEP, прежде чем соответствующие устройства могут зарегистрироваться через DEP.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bb9661733bb33c66b011cf3186801f7a2d698473
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211396"
---
# <a name="depmacosenrollmentprofile-resource-type"></a>Тип ресурса depMacOSEnrollmentProfile

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс DepMacOSEnrollmentProfile представляет профиль регистрации программы регистрации устройств Apple (DEP), относщийся к конфигурации macOS. Этот тип профиля необходимо назначить серийным номерам Apple DEP, прежде чем соответствующие устройства могут зарегистрироваться через DEP.


Наследуется [от depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление depMacOSEnrollmentProfiles](../api/intune-enrollment-depmacosenrollmentprofile-list.md)|[Коллекция depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)|Список свойств и связей объектов [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) .|
|[Получение depMacOSEnrollmentProfile](../api/intune-enrollment-depmacosenrollmentprofile-get.md)|[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)|Чтение свойств и связей объекта [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) .|
|[Создание depMacOSEnrollmentProfile](../api/intune-enrollment-depmacosenrollmentprofile-create.md)|[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)|Создайте объект [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) .|
|[Удаление depMacOSEnrollmentProfile](../api/intune-enrollment-depmacosenrollmentprofile-delete.md)|Нет|Удаляет [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md).|
|[Обновление depMacOSEnrollmentProfile](../api/intune-enrollment-depmacosenrollmentprofile-update.md)|[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)|Обновление свойств объекта [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|GUID объекта, унаследованного от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|displayName|Строка|Имя профиля, унаследованного от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|description|Строка|Описание профиля, унаследованного от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requiresUserAuthentication|Логическое|Указывает, требуется ли для профиля проверка подлинности пользователя, унаследованного от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|configurationEndpointUrl|String|URL-адрес конечной точки конфигурации для регистрации, унаследованного от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|enableAuthenticationViaCompanyPortal|Логическое|Указывает на проверку подлинности с помощью помощника по настройке Apple вместо Корпоративный портал. Наследуется [от enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Логический|Указывает, что Корпоративный портал на зарегистрированных устройствах помощника по настройке, унаследованных от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|isDefault|Boolean|Указывает, является ли этот профиль профилем по умолчанию, унаследованным от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|supervisedModeEnabled|Логическое|Защищенный режим, значение True для включения, значение false в противном случае. Дополнительные https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune сведения см. в этой статье. Наследуется [от depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|supportDepartment|String|Сведения о отделе поддержки, унаследованные [от depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|isMandatory|Логическое|Указывает, является ли профиль обязательным наследованием [от depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|locationDisabled|Логическое|Указывает, отключена ли область установки службы location Inherited от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|supportPhoneNumber|Строка|Номер телефона службы поддержки, унаследованный от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|profileRemovalDisabled|Логическое|Указывает, отключен ли параметр удаления профиля Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md).|
|restoreBlocked|Логическое|Указывает, заблокирована ли область установки восстановления. Наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|appleIdDisabled|Логическое|Указывает, отключена ли область установки идентификатора Apple Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md).|
|termsAndConditionsDisabled|Логический|Указывает, отключена ли область установки "Условия". Наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|touchIdDisabled|Логический|Указывает, отключена ли панель установки touch id Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|applePayDisabled|Логический|Указывает, отключена ли область настройки apple Pay Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|siriDisabled|Логический|Указывает, отключена ли область установки siri Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|diagnosticsDisabled|Логический|Указывает, отключена ли область настройки диагностики Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|displayToneSetupDisabled|Логическое|Указывает, отключен ли экран установки displaytone inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|privacyPaneDisabled|Логическое|Указывает, отключен ли экран конфиденциальности Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|screenTimeScreenDisabled|Логический|Указывает, отключена ли настройка времени ожидания экрана . Наследуется от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|deviceNameTemplate|Строка|Задает литерал или шаблон имени. Наследуется [от depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|configurationWebUrl|Логическое|URL-адрес для входа помощника по настройке, унаследованный от [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|registrationDisabled|Логическое|Указывает, отключена ли регистрация|
|fileVaultDisabled|Логическое|Указывает, отключено ли хранилище файлов|
|iCloudDiagnosticsDisabled|Логическое|Указывает, отключен ли экран iCloud Analytics|
|passCodeDisabled|Логическое|Указывает, отключена ли область установки секретного кода|
|zoomDisabled|Логическое|Указывает, отключена ли область настройки масштабирования|
|iCloudStorageDisabled|Логическое|Указывает, отключен ли экран документов iCloud и рабочего стола|
|chooseYourLockScreenDisabled|Логическое|Указывает, отключен ли экран документов iCloud и рабочего стола|
|accessibilityScreenDisabled|Логическое|Указывает, отключен ли экран специальных возможностей|
|autoUnlockWithWatchDisabled|Логическое|Указывает, отключен ли экран UnlockWithWatch|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.depMacOSEnrollmentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.depMacOSEnrollmentProfile",
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
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "String",
  "profileRemovalDisabled": true,
  "restoreBlocked": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "displayToneSetupDisabled": true,
  "privacyPaneDisabled": true,
  "screenTimeScreenDisabled": true,
  "deviceNameTemplate": "String",
  "configurationWebUrl": true,
  "registrationDisabled": true,
  "fileVaultDisabled": true,
  "iCloudDiagnosticsDisabled": true,
  "passCodeDisabled": true,
  "zoomDisabled": true,
  "iCloudStorageDisabled": true,
  "chooseYourLockScreenDisabled": true,
  "accessibilityScreenDisabled": true,
  "autoUnlockWithWatchDisabled": true
}
```




