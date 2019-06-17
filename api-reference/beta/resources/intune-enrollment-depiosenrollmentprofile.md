---
title: Тип ресурса Депиосенроллментпрофиле
description: Ресурс Депиосенроллментпрофиле представляет профиль регистрации программы регистрации устройств Apple (DEP), характерный для конфигурации iOS. Этот тип профиля должен быть назначен серийным номерам Apple DEP, прежде чем соответствующие устройства смогут регистрироваться с помощью функции DEP.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: adc271f461d83278dbb6007ce871424b3799bb4e
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993559"
---
# <a name="depiosenrollmentprofile-resource-type"></a>Тип ресурса Депиосенроллментпрофиле

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс Депиосенроллментпрофиле представляет профиль регистрации программы регистрации устройств Apple (DEP), характерный для конфигурации iOS. Этот тип профиля должен быть назначен серийным номерам Apple DEP, прежде чем соответствующие устройства смогут регистрироваться с помощью функции DEP.


Наследуется от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Депиосенроллментпрофилес](../api/intune-enrollment-depiosenrollmentprofile-list.md)|Коллекция [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md)|Список свойств и связей объектов [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md) .|
|[Получение Депиосенроллментпрофиле](../api/intune-enrollment-depiosenrollmentprofile-get.md)|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)|Чтение свойств и связей объекта [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md) .|
|[Создание Депиосенроллментпрофиле](../api/intune-enrollment-depiosenrollmentprofile-create.md)|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)|Создание нового объекта [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md) .|
|[Удаление Депиосенроллментпрофиле](../api/intune-enrollment-depiosenrollmentprofile-delete.md)|Нет|Удаляет объект [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md).|
|[Обновление Депиосенроллментпрофиле](../api/intune-enrollment-depiosenrollmentprofile-update.md)|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)|Обновление свойств объекта [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|GUID объекта, наследуемого от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)|
|displayName|Строка|Имя профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)|
|description|String|Описание профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)|
|Рекуиресусераусентикатион|Boolean|Указывает, требуется ли для профиля проверка подлинности пользователей, унаследованных от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)|
|Конфигуратионендпоинтурл|String|URL-адрес конечной точки конфигурации, используемый для регистрации, унаследованный от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)|
|enableAuthenticationViaCompanyPortal|Boolean|Указывает на проверку подлинности с помощью помощника по настройке Apple, а не корпоративного портала. Наследуется от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)|
|Рекуирекомпанипорталонсетупассистантенролледдевицес|Boolean|Указывает, что корпоративный портал необходим на зарегистрированных устройствах помощника по настройке, наследуемых от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)|
|isDefault|Boolean|Указывает, является ли этот профиль профилем по умолчанию, унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|Супервиседмодинаблед|Boolean|Защищенный режим, true для включения, false в противном случае. Дополнительную https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune информацию можно узнать в статье. Наследуется от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|Суппортдепартмент|String|Сведения о отделе поддержки, унаследованные от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|Пасскодедисаблед|Boolean|Указывает, является ли область настройки секретного кода наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|Обязательный|Boolean|Указывает, является ли профиль обязательно унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|Локатиондисаблед|Boolean|Указывает, является ли область настроек службы расположений наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|Суппортфоненумбер|String|Номер телефона поддержки, наследуемый от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|Профилеремовалдисаблед|Boolean|Указывает, является ли параметр удаления профиля унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|Рестореблоккед|Boolean|Указывает, заблокирована ли область настройки "восстановление" из [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|Апплеиддисаблед|Boolean|Указывает, является ли область настроек Apple ID унаследованной от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|Термсандкондитионсдисаблед|Boolean|Указывает, отключена ли область установки "условия и условия" от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|Таучиддисаблед|Boolean|Указывает, является ли область настроек сенсорного экрана наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|Апплепайдисаблед|Boolean|Указывает, отключена ли область настройки оплаты Apple от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|Зумдисаблед|Boolean|Указывает, является ли область настройки масштаба унаследованной от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|Сиридисаблед|Boolean|Указывает, наследуется ли область настройки Siri от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|Диагностиксдисаблед|Boolean|Указывает, является ли область настройки диагностики неактивной, наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|Дисплайтонесетупдисаблед|Boolean|Указывает, отключен ли экран установки дисплайтоне от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|Приваципанедисаблед|Boolean|Указывает, отключен ли экран конфиденциальности, унаследованный от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|Девиценаметемплате|String|Задает шаблон литерала или имени. Наследуется от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|iTunesPairingMode|[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md).|Указывает режим связывания iTunes. Возможные значения: `disallow`, `allow`, `requiresCertificate`.|
|Манажементцертификатес|Коллекция [манажементцертификатевиссумбпринт](../resources/intune-enrollment-managementcertificatewiththumbprint.md)|Сертификаты управления для конфигуратора Apple|
|Ресторефромандроиддисаблед|Boolean|Указывает, отключено ли восстановление из Android|
|Аваитдевицеконфигуредконфирматион|Boolean|Указывает, должно ли устройство ждать настройки подтверждения.|
|Свойства sharedipadmaximumusercount|Int32|Указывает максимальное количество пользователей, которые могут использовать общий iPad. Относится только к общему режиму iPad.|
|Enablesharedipad к|Boolean|Указывает, следует ли зарегистрировать устройство в режиме, позволяющем использовать сценарии с несколькими пользователями. Применяется только в общих iPad.|
|Компанипорталвпптокенид|String|Если этот параметр установлен, указывает, какой токен VPP должен использоваться для развертывания корпоративного портала с лицензией "на устройство". для задания этого свойства необходимо задать значение "enableAuthenticationViaCompanyPortal".|
|Енаблесинглеаппенроллментмоде|Boolean|Указывает, что устройство включает один режим приложения и применяет блокировку приложений во время регистрации. Значение по умолчанию — false. для задания этого свойства должно быть задано значение "enableAuthenticationViaCompanyPortal" и "Компанипорталвпптокенид".|
|Хомебуттонскриндисаблед|Boolean|Указывает, отключен ли экран "чувствительность к домашней кнопке"|
|Имессажеандфацетимескриндисаблед|Boolean|Указывает, отключен ли экран iMessage и FaceTime|
|Онбоардингскриндисаблед|Boolean|Указывает, отключен ли встроенный экран установки|
|Скринтимескриндисаблед|Boolean|Указывает, отключена ли настройка времени ожидания экрана|
|Симсетупскриндисаблед|Boolean|Указывает, отключен ли экран Симсетуп|
|Софтвареупдатескриндисаблед|Boolean|Указывает, отключено ли обязательное экранное обновление софваре|
|Ватчмигратионскриндисаблед|Boolean|Указывает, отключен ли экран контрольных значений для миграции|

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
  "deviceNameTemplate": "String",
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





